---
title: "SF Symbols 아이콘을 iOS12 이하에서도 사용하기"
tags: 
    - ios
    - icon
---

[SF Symbols](https://developer.apple.com/design/human-interface-guidelines/sf-symbols/overview/)는 애플이 내놓은 아이콘 세트다. 그런데 iOS13부터 지원하고 그 이하에서는 지원을 하지 않는다. iOS13 이상을 대상으로는 아래처럼 사용할 수 있다.

iOS13부터 지원한다는 건 XCode에서 이미지 이름만으로 SF Symbols의 아이콘을 불러올 수 있다는 말이다. 

![](/images/2020/how-to-use-sf-symbols-on-ios13.png)

우측 패널의 Image 쪽에서 SF Symbols의 이름을 써서 `<` 아이콘을 불러 왔다.

## iOS12 이하에서 SVG 내보내기해서 사용하기? 안 된다.

그런데 SF Symbols에는 SVG Export(<kbd>⌘</kbd> + <kbd>E</kbd>) 기능이 있다. 이 SVG 파일을 사용하면 될까? 해 보니 안 됐다. 이렇게 Export한 아이콘을 사용해 보니 iOS12에서 이 아이콘이 보이지 않았다는 말이다.

왜 그런 것일까? SF Symbols에서 내보내는 SVG 파일에는 9가지 굵기와 세 가지 크기가 있다. 브라우저에서 이 SVG 파일을 열어 보면 아래 이미지처럼 나오는 것을 확인할 수 있다. 아마도 최신 버전의 SVG 포맷이거나 애플의 SVG 포맷 둘 중의 하나일 텐데, 여하간 iOS12는 이걸 해석하지 못한다.

![](/images/2020/sf-symbols-svg.png)

그래서 결국은 위에 있는 27개의 아이콘 중 하나를 png로 변환해서 사용해야 한다. 

## Happy Coding으로 png로 변환

SF Symbols를 PNG로 쉽게 변환하게 도와 주는 프로그램이 있다. [HappyCoding](https://happycoding.app/)이라는 프로그램이다. 여러가지 기능이 있는데 그중 SF Symbols 아이콘을 png로 변환해 주는 기능이 있다.

우선 프로젝트를 추가한 뒤 연다. 

![](/images/2020/happycoding1.png) 

사이드바에서 Assets를 클릭하고, 아래쪽의 네모 네 개짜리 아이콘을 누른다. 

![](/images/2020/happycoding2.png) 

그러면 아래와 같이 아이콘들이 나온다.

![](/images/2020/happycoding3.png) 

아이콘의 사이즈를 조정하고 원하는 아이콘을 고른 뒤 아이콘을 더블클릭하거나 우측 하단의 Import를 누르면 프로젝트의 Assets로 아이콘의 PNG가 임포트된다. 

간혹 임포트되지 않는 경우가 있는데, 버그인 것 같다. 그럴 때는 그냥 사이즈 조절 같은 것을 하지 말고 임포트를 하면 작동한다. 

사이즈는 임포트 후에도 조절할 수 있다. 아래 이미지 참고.

![](/images/2020/happycoding4.png)

**아이콘으로 사용할 거라면 색상을 변경할 필요는 없다.** 아이콘으로 사용하는 경우에는 Xcode에서 기본적으로 Shiny Blue 색상으로 덮어쓰기 때문이다. 아이콘 색상을 설정하고 싶다면 Tint를 설정하면 된다. (코드로 하려면 `button.tintColor = .systemIndigo` 같은 식으로 하면 작동한다고 한다. 즉, 틴트컬러는 버튼 객체의 속성이다.)
