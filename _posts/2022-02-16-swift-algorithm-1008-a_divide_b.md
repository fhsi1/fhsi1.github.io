---
title:  "[Swift] 1008 - A / B"
excerpt: "나눗셈 문제"
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
  - I/O and arithmetic
last_modified_at: 2022-02-16 17:04:05
---


```swift
//
//  1008-a_divide_b.swift
//  Algorithm
//
//  Created by Yujean Cho on 2022/02/14.
//

import Foundation

let line = readLine()!
let lineArr = line.split(separator: " ")
let a = Double(lineArr[0])!
let b = Double(lineArr[1])!
print(a/b)
```