---
title:  "[Swift] 10430 - 나머지"
excerpt: "네 개의 계산식을 계산하는 문제"
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
last_modified_at: 2022-02-16 17:17:57
---

```swift
//
//  10430-Remainder.swift
//  Algorithm
//
//  Created by Yujean Cho on 2022/02/15.
//

import Foundation

let input = readLine()!
let lineArr = input.split(separator: " ")
let a = Int(lineArr[0])!
let b = Int(lineArr[1])!
let c = Int(lineArr[2])!

print((a + b) % c)
print(((a % c) + (b % c)) % c)
print((a * b) % c)
print(((a % c) * (b % c)) % c)
```