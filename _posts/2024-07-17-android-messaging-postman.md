---
layout: post
title: "최신 Firebase 인증, 포스트맨에서 알림 테스트하기"
tags: 
    - postman
    - firebase
---

최신 Firebase 인증은 고정 키를 이용하는 게 아니라 OAuth를 사용해 제한시간이 있는 토큰을 사용한다. 

그래서 아래 글을 참고하면 된다.

[Android FCM 전송 테스트with Postman](https://velog.io/@thwjd9393/Android-FCM-%EC%A0%84%EC%86%A1-%ED%85%8C%EC%8A%A4%ED%8A%B8with-Postman)

요약하면 

1. [OAuth Playground](https://developers.google.com/oauthplayground)에서 Firebase Cloud Messaging API v1을 선택하고 그 밑의 https://www.googleapis.com/auth/cloud-platform을 선택 → Authorize APIs 클릭
2. 액세스 허용
3. Exchange authorization code for tokens 클릭
4. 응답에서 access_token 복사.
5. Postman에서 헤더 세팅. Authorization: Bearer {access_token}

메시지 바디는 아래와 같이.

```json
{
    "message": {
        "token": "FCM_TOKEN",
        "notification": {
          "body": "Body of Your Notification in data",
          "title": "Title of Your Notification in data"
        }
    }
}
```
