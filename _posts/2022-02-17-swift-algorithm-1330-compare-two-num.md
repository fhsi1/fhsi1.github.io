---
title:  "[Swift] 1330 - 두 수 비교하기"
excerpt: "두 수를 비교한 결과를 출력하는 문제"
header:
  teaser: /assets/images/icon/swift.png
toc: false
toc_icon: "check-circle"
toc_sticky: true

categories:
  - Algorithm
tags:
  - 백준
  - Swift
last_modified_at: 2022-02-17 17:37:06
---

```swift
//
//  1330-CompareTwoNum.swift
//  Algorithm
//
//  Created by Yujean Cho on 2022/02/16.
//

import Foundation

let line = readLine()!
let lineArr = line.split(separator: " ")
let a = Int(lineArr[0])!
let b = Int(lineArr[1])!

if a > b {
    print(">")
} else if a < b {
    print("<")
} else {
    print("==")
}
```