---
title:  "Swift로 문제풀기 기본 세팅"
excerpt: "Xcode 환경 세팅"
header:
  teaser: /assets/images/icon/swift.png
toc: true
toc_sticky: true

categories:
  - Algorithm
tags:
  - 백준
  - swift
last_modified_at: 2022-02-14 17:27:21
---

최근, Swift 문법 공부를 시작하면서 <br>
Algorithm 문제도 같이 풀면 <br>
많은 도움이 될 것 같다는 생각을 하게 되었다. <br>

Xcode 에서 Swift 문제풀기를 위한 <br>
기본적인 환경설정을 해보고자 한다. <br>

## Xcode 새 프로젝트 생성하기

![Xcode_Create_New_project](https://github.com/fhsi1/fhsi1.github.io/blob/master/assets/images/swfit-algorithm-xcode/Xcode_Create_New_Project.png?raw=true)

## 프로젝트 템플릿 선택하기

![Choose_MacOS_Command_line_Tool](https://github.com/fhsi1/fhsi1.github.io/blob/master/assets/images/swfit-algorithm-xcode/Choose_MacOS_Command_Line_Tool.png?raw=true)

창 상단의 Multiplatform 을 macOS 로 선택하면 <br>
Command Line Tool 이 보인다. <br>

> ❓ 문제를 풀면서 input value 를 받아야하기 때문에 <br>
  Command Line Tool 을 선택해 준다. <br>

## 프로젝트 이름 설정하기

![Set_Project_Name](https://github.com/fhsi1/fhsi1.github.io/blob/master/assets/images/swfit-algorithm-xcode/Set_Project_Name.png?raw=true)

프로젝트 이름을 설정하면, 다음과 같이 생성이 완료된다. <br>

![Done_Project_Create](https://github.com/fhsi1/fhsi1.github.io/blob/master/assets/images/swfit-algorithm-xcode/Done_Project_Create.png?raw=true)

## main 열기

![Open_Main](https://github.com/fhsi1/fhsi1.github.io/blob/master/assets/images/swfit-algorithm-xcode/Open_Main.png?raw=true)

왼쪽의 main.swift 를 열면 <br>
아래와 같이 기본적인 코드가 생성되어 있다. <br>

![Hello_World!](https://github.com/fhsi1/fhsi1.github.io/blob/master/assets/images/swfit-algorithm-xcode/Hello_World.png?raw=true)

Xcode 창 오른쪽 상단의 ▶️ 버튼을 누르면 코드를 실행할 수 있다. <br>
결과는 아래의 오른쪽 콘솔창으로 확인할 수 있다. <br>

## 기본 설정 완료 및 문제풀기

다음은 백준 1000번 문제 a+b 를 구현한 것이다.

![a_plus_b](https://github.com/fhsi1/fhsi1.github.io/blob/master/assets/images/swfit-algorithm-xcode/a_plus_b.png?raw=true)

input value 는 readLine 함수로 받을 수 있고, <br>
split 함수를 이용하여 띄어쓰기를 기준으로 값을 분리하여 사용했다.

```swift
let line = readLine()!
let lineArr = line.split(separator: " ")
```

문제는 main.swift 파일에서 풀고 <br>
다 푼 문제는 새로운 파일을 생성해서 옮기는 방식으로 하고 있다.

main.swift 파일만 <br>
Xcode 창의 오른쪽에 있는 Target Membership 을 체크해두고 <br>
나머지는 체크를 해제시켜서 <br>
main.swift 파일만 실행되도록 하였다. <br>

문제를 다 풀고 새로운 파일을 생성할 때 <br>
Target Membership 을 체크 해제하고 생성할 수도 있다. <br>

---

> 📚 Reference <br>
[Swift로 알고리즘 풀기 전 기본 세팅](https://velog.io/@ssionii/Swift%EB%A1%9C-%EC%95%8C%EA%B3%A0%EB%A6%AC%EC%A6%98-%ED%92%80%EA%B8%B0-%EC%A0%84-%EA%B8%B0%EB%B3%B8-%EC%84%B8%ED%8C%85)