---
title: 'Firebase Cloud Messaging API(V1) 키 만들기'
layout: post
tags: 
    - fcm
    - firebase
description: 서비스 계정 관리 > 이메일 클릭 > 키 탭 > 키 추가 > 새 키 만들기 > 만들기 > json
---

원래 FCM(Firebase Cloud Messaging)은 API 키만 가지고 메시지를 보낼 수 있게 돼 있었는데, 최근에 OAuth2를 사용하는 것으로 변경이 됐다. 서버에서 푸시 메시지를 보낼 때 보안이 더 강화됐는데, 대신에 좀더 복잡하게 됐다.

서버에서 OAuth2 인증을 하고 키를 얻으려면 키로 사용하는 json 파일을 생성하고 다운받아야 한다. 가끔만 사용하는 것이므로 메모용으로 적어 둔다.

우선 파이어베이스 클라우드 메시징 탭에서 **서비스 계정**을 클릭한다. 아래 이미지를 참고한다.

![](/assets/2022/firebase-cloud-messaging-api(v1)-1.png)

서비스 계정을 클릭하면 구글 클라우드 서비스로 이동하게 된다. 구글이 API를 전부 이동시킬 생각인가 보다.

여기서 이메일을 클릭한다. 아래 이미지 참고.

![](/assets/2022/firebase-cloud-messaging-api(v1)-2.png)

그러면 나오는 페이지에서 **키** 탭으로 이동한 뒤 **키 추가**를 선택하고 **새 키 만들기**를 누른다. 아래 이미지 참고.

![](/assets/2022/firebase-cloud-messaging-api(v1)-3.jpg)

여기에서 json을 선택하면 끝난다.

![](/assets/2022/firebase-cloud-messaging-api(v1)-4.png)

그러면 json 파일이 다운로드된다.

이제 서버에 이 키를 안전한 위치에 저장한 뒤 사용하면 된다. 사용하는 방법은 언어별 auth library를 찾아 보면 되는데, PHP는 [google-auth-library-php](https://github.com/googleapis/google-auth-library-php)를 참고하면 된다.

참고로, 예제 코드에 `$scopes` 설정이 나오는데, FCM의 경우 scope는 `https://www.googleapis.com/auth/firebase.messaging`다.
