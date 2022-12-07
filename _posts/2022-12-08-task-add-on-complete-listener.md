---
layout: post
title: "[자바/안드로이드] Task onCompleteListener 사용법"
tags: 
    - java
    - android
---

간단히 예제 코드 저장용으로 작성한 글입니다. 

```java
FirebaseMessaging firebaseMessaging = FirebaseMessaging.getInstance();
Task<Void> subscribeToTopicTask = firebaseMessaging.subscribeToTopic("basic");
subscribeToTopicTask.addOnCompleteListener(new OnCompleteListener<Void>() {
    @Override
    public void onComplete(@NonNull Task<Void> task) {
        Log.i(TAG, "subscribeToTopic basic completed.");
    }
});
```

## 상황

안드로이드에서 파이어베이스에 토픽 구독을 시킨 다음에 그걸 저장하려고 했습니다. 당연히 토픽 구독이 성공을 해야 저장을 할 수 있습니다.

토픽 구독은 백그라운드(스레드)에서 진행되므로 별도로 리스너를 넣어 줘야 합니다. IDE의 파라미터를 참고했더니 Exeutor를 넣으라고 하는데 써 본 적도 없고 API로는 헷갈렸습니다. 

예제를 찾아 보니 `OnCompleteListner`라는 인터페이스가 있었습니다. 이걸 구현하면 되는 거였네요. 파라미터에서 익명 클래스로 구현해도 되는 거였습니다. 두 번 쓸 거면 이름 있는 클래스로 하면 되겠죠.

예제 코드는 어렵지 않으니 한 번 살펴 보세요.