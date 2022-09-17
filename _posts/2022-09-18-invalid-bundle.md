---
layout: post
title: "에러 해결. Invalid bundle. Because your app supports Multitasking on iPad, you need to include the LaunchScreen.storyboard launch storyboard file"
tags: 
    - ios
    - apple
---

**Product > Archive**를 실행하니까 이런 에러가 났다. LaunchScreen 파일이 꼭 있어야 한다는 건데, 나는 있는데 뭐지...

> Invalid bundle. Because your app supports Multitasking on iPad, you need to include the LaunchScreen.storyboard launch storyboard file in your com.xxx.xxx bundle. Use UILaunchScreen instead if the app’s MinimumOSVersion is 14 or higher and you prefer to configure the launch screen without storyboards. For details, see: https://developer.apple.com/documentation/bundleresources/information_property_list/uilaunchstoryboardname (ID: 963167c4-f233-42b9-8c17-14c372e2b484)

번역하면 이렇다.

> 잘못된 번들입니다. 앱이 iPad에서 멀티태스킹을 지원하기 때문에 com.xxx.xxx 번들에 LaunchScreen.storyboard 시작 스토리보드 파일을 포함해야 합니다. 앱의 MinimumOSVersion이 14 이상이고 스토리보드 없이 시작 화면을 구성하려는 경우 대신 UILaunchScreen을 사용하십시오. 자세한 내용은 https://developer.apple.com/documentation/bundleresources/information_property_list/uilaunchstoryboardname(ID: 963167c4-f233-42b9-8c17-14c372e2b484)을 참조하십시오.

안내된 링크로 들어가 보니 `.storyboard` 확장자를 떼라는 이야기가 있었다.

> Specify the name of the storyboard file without the filename extension. For example, if the filename of your storyboard is LaunchScreen.storyboard, specify "LaunchScreen" as the value for this key.

> 파일 이름 확장자가 없는 스토리보드 파일의 이름을 지정합니다. 예를 들어 스토리보드의 파일 이름이 LaunchScreen.storyboard인 경우 이 키의 값으로 "LaunchScreen"을 지정합니다.

그래서 Info.plist 파일을 열어서 아래처럼 확장자를 뗐다.

```xml
<key>UILaunchStoryboardName</key>
<string>LaunchScreen</string>
```

원래는 아래처럼 확장자가 붙어 있었다.

```xml
<key>UILaunchStoryboardName</key>
<string>LaunchScreen.storyboard</string>
```

이러니 해결됐다.

