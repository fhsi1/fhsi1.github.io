---
title:  "Swift Playground 만들기"
excerpt: "Xcode 환경 세팅"
header:
  teaser: /assets/images/icon/swift.png
toc: true
toc_icon: "check-circle"
toc_sticky: true

categories:
  - Algorithm
tags:
  - Swift
last_modified_at: 2022-02-25 18:20:21
---

Swift 문법 공부를 하면서, <br>
간단하게 테스트를 해보고 싶을 때, <br>
**Playground** 를 활용하면 좋을 것 같다는 생각을 하게 되었다. <br>

Xcode 에서 **Playground** 를 만들어 보고자 한다. <br>

## Xcode 상단바에서 Playground 생성 찾기

Xcode 를 열고, <br>
상단바에서 `File > New > Playground` 순서로 클릭하면 <br>
Playground 를 생성할 수 있다. <br>

단축키로는, `⌥⇧⌘N` 로 가능하다.<br>

## Playground template 선택하기

![Choose_Playground_Template](https://github.com/fhsi1/fhsi1.github.io/blob/master/assets/images/swift-playground/Choose_Playground_Template.png?raw=true)

상단바에서 Playground 생성을 찾아 클릭하고 나면,<br>
위와 같이 template 를 고르는 창이 나온다.<br>

본인의 목적에 맞게 골라주면 되고, <br>
간단하게 테스트를 해보려는 목적이라면 **Blank** 를 골라주면 된다.<br>

## Playground 이름 정하기

![Set_Playground_Name_Path](https://github.com/fhsi1/fhsi1.github.io/blob/master/assets/images/swift-playground/Set_Playground_Name_Path.png?raw=true)

Playground 이름과 경로를 원하는대로 지정해주면 된다.<br>

## Playground 생성 완료

![Playground_Default](https://github.com/fhsi1/fhsi1.github.io/blob/master/assets/images/swift-playground/Playground_Default.png?raw=true)

위와 같이, Playground 가 생성 완료되었다.<br>

코드 왼쪽의 파란색 실행 버튼을 누르면 코드 한 줄을 실행할 수 있고,<br>
Xcode 창 하단의 실행 버튼을 누르면 전체 코드를 실행할 수 있다.<br>
(창 하단의 실행 버튼을 누른 경우, 실행 중이라면 위와 같이 네모 모양이 된다.) <br>

## Playground 사용해보기

Playground 를 생성했으니, 한 번 사용해보도록 하자.<br>

```swift
for i in 0...99 {
    i
}
```

`0` 부터 `99` 까지 `i` 를 증가시키는 반복문을 추가해보았다. <br>

![Use_Playground](https://github.com/fhsi1/fhsi1.github.io/blob/master/assets/images/swift-playground/Use_Playground.png?raw=true)

실행 버튼을 누르고 오른쪽 부분을 보면, <br>
`(100 times)` 라고 실행 결과를 볼 수 있다. <br>
그 부분에 마우스를 올리면 눈 모양이 나오는데, <br>
다음과 같이, 실행 결과를 시각적으로 볼 수 있다. <br>

![Use_Playground_for](https://github.com/fhsi1/fhsi1.github.io/blob/master/assets/images/swift-playground/Use_Playground_for.png?raw=true)

---

> 📚 Reference <br>
[Playground 사용해보기](https://devxoul.gitbooks.io/ios-with-swift-in-40-hours/content/Chapter-1/playground.html)