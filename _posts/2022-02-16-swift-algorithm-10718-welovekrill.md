---
title:  "[Swift] 10718 - We Love Krill"
excerpt: "주어진 예제처럼 출력하는 문제"
header:
  teaser: /assets/images/icon/swift.png
toc: true
toc_icon: "check-circle"
toc_sticky: true

categories:
  - Algorithm
tags:
  - 백준
  - Swift
last_modified_at: 2022-02-16 16:45:00
---

## 🧪 Problem

ACM-ICPC 인터넷 예선, Regional, 그리고 World Finals까지 이미 2회씩 진출해버린 kriii는 미련을 버리지 못하고 왠지 모르게 올해에도 파주 World Finals 준비 캠프에 참여했다.

대회를 뜰 줄 모르는 지박령 kriii를 위해서 격려의 문구를 출력해주자.

### Input

없음

### Output

```shell
강한친구 대한육군
강한친구 대한육군
```

## 💡 Solution

`print` 함수를 두 번 쓰는 방법과 한 번 쓰는 방법을 생각해보았다.<br>

```swift
//
//  10718-WeLoveKriii.swift
//  Algorithm
//
//  Created by Yujean Cho on 2022/02/13.
//

import Foundation

print("강한친구 대한육군")
print("강한친구 대한육군")
```

```swift
//
//  10718-WeLoveKriii.swift
//  Algorithm
//
//  Created by Yujean Cho on 2022/02/13.
//

import Foundation

print("강한친구 대한육군\n강한친구 대한육군")
```

제출 결과, `print` 함수를 한 번만 쓰는 것이 코드의 길이가 더 짧았지만,<br>
메모리나 속도는 동일했다. <br>