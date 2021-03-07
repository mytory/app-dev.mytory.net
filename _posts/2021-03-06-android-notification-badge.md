---
layout: post
title: "안드로이드. 여러 런처에서, 앱이 백그라운드 상태일 때도 일관되게 알림 배지 표시하기"
tags: 
    - android
    - notification
---

안드로이드 앱 아이콘에 알림 배지를 표시하는 것은 까다롭다.

안드로이드 구버전에는 알림 배지 기능이 없었는데, 그래서 여러 런처에서 알아서 앱 아이콘 알림 배지 기능을 구현한 모양이다. 이런 것까지 파편화돼 있을 줄은 몰랐다.

안드로이드 8(오레오, API 26)부터는 운영체제 단에서 알림 배지를 지원한다. 그러나 우리가 흔히 아는 숫자 배지가 아니다. 알림이 있다는 표시만 되는 배지다. 배지가 보이면 길게 눌러 알림 내용을 확인한다. (아래 이미지는 [안드로이드 문서](https://developer.android.com/training/notify-user/badges)를 캡쳐한 것이다.)

![](/assets/2021/android-notification-badge-doc.png)

다행히 이 기본 배지는 알림을 표시하기 위해 따로 코딩이 필요 없다. 따라서 패스.

## 여러 런처에 대응하는 라이브러리

여러 런처에 대응하기 위해서는 라이브러리를 사용하는 게 제일 편하다. 나는 [ShortcutBadger](https://github.com/leolin310148/ShortcutBadger) ver1.1.22를 사용했다. 자세한 사용법은 라이브러리의 문서를 참고하면 되겠다.

## 앱이 백그라운드에 있을 때 푸시 알림 카운트 수정하기

가장 골치아팠던 게 앱이 백그라운드에 있을 때 푸시 알림 카운트를 수정하는 것이었다. 앱이 실행중일 때는 알림이 오면 `FirebaseMessagingService`의 `onMessageReceived` 메서드의 코드가 실행됐는데, 앱이 백그라운드에 있을 때는 그렇지 않았던 것이다.

**비밀은 FCM json 호출에 있다.** 호출시 `notification` 키값을 빼고 알림을 호출하면 `onMessageReceived` 메서드가 호출된다(!). 아래 예시처럼 말이다. 그냥 `data` 키값에 데이터만 넣어서 호출한다.

``` json
{
    "data": {
        "badge": "1",
        "data_srno": "14513",
        "data_type": "ALARM",
        "data_msg": "",
        "title": "System Alarm",
        "message": "zms1"
    },
    "registration_ids": [
        "...:APA91bE2WmYoT-Fcgvumn7hk2MmLQiRuUrKPUNPOaPCe_EFts8zWWsqjzMKMHHH7inpGXXaY3R1Rq0kUC4O_jTvB6f3Au-77XjNSUdlg9JTjlsoevpABovBofWmLf9UZxOUoC0Hzhnh1"
    ]
}
```


## 대체 설명은 문서 어디에?

우선 안드로이드 운영체제 자신이 지금 우리가 하는 일에는 관심이 없다는 점을 알자. 푸시 알림을 받으면 알림 배지에 표시되는 숫자를 갱신하기 위해 코드를 실행한다는 게 안드로이드 입장에서는 기본 개념이 아닌 것이다.

다만 알림이 왔을 때 뭔가 코드를 실행하려면 어떻게 하지? 하는 것에 대한 답이 될 만한 문서의 내용이 있긴 한데, 안드로이드 문서가 아니라 파이어베이스 문서에서 찾을 수 있다.

[다음 파이어베이스 공식 문서](https://firebase.google.com/docs/cloud-messaging/android/receive?hl=ko)를 해독해 보자. 표를 보면 된다.

![](/assets/2021/firebase-message-doc.png)

앱이 포그라운드(Foreground) 상태에 있을 때, 즉 실행중일 때는 `onMessageReceived` 메서드가 세 경우 모두 실행된다고 설명돼 있다.

그리고 백그라운드 상태일 때 알림(`notification` 키)은 작업 표시줄로 가고 데이터(`data` 키)는 `onMessageReceived`로 간다는 식으로 설명이 돼 있는데... 내 경험으로는 아니다.

`notification` 키가 있는 경우, 작업 표시줄만 갱신되고 끝난다. `data`는 알림을 터치해야 처리된다. 따라서 코드도 실행되지 않고 앱 배지는 갱신되지 않는다. **코드가 실행되려면 `notification` 키가 없어야 한다.** 위에 내가 예시로 적어 둔 코드처럼 말이다.


