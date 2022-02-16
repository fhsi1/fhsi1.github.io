---
title:  "[Swift] 10869 - 사칙연산"
excerpt: "모든 연산 문제"
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
last_modified_at: 2022-02-16 17:08:20
---

```swift
//
//  10869-ArithmeticOperation.swift
//  Algorithm
//
//  Created by Yujean Cho on 2022/02/14.
//

import Foundation

let line = readLine()!
let lineArr = line.split(separator: " ")
let a = Int(lineArr[0])!
let b = Int(lineArr[1])!
print(a+b)
print(a-b)
print(a*b)
print(a/b)
print(a%b)
```