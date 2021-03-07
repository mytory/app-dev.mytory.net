---
title: "iOS 푸시 알림, 파이어베이스에 APN 인증서 등록하기"
date: 2019-12-23T22:11:33+09:00
tags: 
    - ios
    - notification
    - firebase
---

아래 설명을 보는 것보다 이 링크를 참고하라: <https://firebase.google.com/docs/cloud-messaging/ios/certs?hl=ko>

아래 설명은 작동은 하지만 복잡하고 매년 키를 갱신해야 하는 반면 위 문서는 간편하고, 매년 키를 갱신할 필요도 없다.

---

iOS의 푸시 알림 등록은 안드로이드보다 훨씬 까다롭다. 매번 아래 동영상을 참고해서 인증서를 생성하고 업로드하고 다운로드하고 다시 업로드해 인증서 등록을 마쳤는데, 그냥 문서로 정리해 두는 편이 좋을 듯해 이번엔 정리를 했다.

{{< youtube PQbEqhKDIZU >}}

거의 혼자 볼 용도로 정리한 것이니, 정리가 덜 돼 있어도 양해 바란다.

1. 키체인 접근 > 인증서 지원 > 인증기관에서 인증서 요청 / 이메일 입력, 이름, 디스크에 저장됨으로.
2. 프로젝트 설정 > Capabilities > Push Notification > On
3. <https://developer.apple.com/account/resources/identifiers/>(Certificates, Identifiers & Profiles > Identifiers)로 이동. 거기서 Push Notifications > Configure > Development SSL Certificate > Create Certificate > 아까 만든 `CertificateSigningRequest.certSigningRequest` 파일 업로드 후 생성된 파일 다운로드(`aps_development.cer`). / Production SSL Certificate에 같은 `CertificateSigningRequest.certSigningRequest` 파일을 업로드해도 된다.
4. 다운로드한 파일 실행하면 키체인 접근에 임포트됨. (분류는 그냥 로그인으로 선택.)
5. 키체인 접근에서 방금 임포트한 키체인을 내보내기 한다. `p12` 확장자가 선택돼 있으면 되고, 파일명은 `forFirebase`라고 한다(`aps.cer`이면 `forFirebaseProduction`이라고 짓자). 키체인 암호를 입력하라고 하는데 입력한다. 빈 값도 된다. 맥의 로그인 암호 입력하라고 하는데 입력해 준다. 그럼 익스포트 된다.
6. 파이어베이스로 이동해서 iOS 프로젝트 선택하고, 설정 > 클라우드 메시징 > APN 인증서 > 개발 APN 인증서 > 업로드. 아까 내보내기 한 `forFirebase.p12` 파일을 업로드한다. (제품 APN 인증서엔 `forFirebaseProduction.p12`를 업로드하면 된다.)

