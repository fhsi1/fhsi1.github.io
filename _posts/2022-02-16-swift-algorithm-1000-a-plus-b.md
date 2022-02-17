---
title:  "[Swift] 1000 - A + B"
excerpt: "두 수를 입력받고 합을 출력하는 문제"
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
last_modified_at: 2022-02-16 16:55:47
---

```swift
//
//  1000-a_plus_b.swift
//  Algorithm
//
//  Created by Yujean Cho on 2022/02/13.
//

import Foundation

let line = readLine()!
let lineArr = line.split(separator: " ")
let a = Int(lineArr[0])!
let b = Int(lineArr[1])!
print(a+b)
```