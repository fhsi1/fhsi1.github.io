---
title:  "[Swift] 9498 - 시험 성적"
excerpt: "시험 점수를 성적으로 바꾸는 문제"
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
last_modified_at: 2022-02-17 17:39:20
---

```swift
//
//  9498-ExamScore.swift
//  Algorithm
//
//  Created by Yujean Cho on 2022/02/16.
//

import Foundation

let score = Int(readLine()!)!

switch score {
case 90...100:
    print("A")
case 80...89:
    print("B")
case 70...79:
    print("C")
case 60...69:
    print("D")
default:
    print("F")
}
```