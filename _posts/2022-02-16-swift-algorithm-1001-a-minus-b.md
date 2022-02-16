---
title:  "[Swift] 1001 - A - B"
excerpt: "두 수를 입력받고 뺄셈을 한 결과를 출력하는 문제"
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
last_modified_at: 2022-02-16 16:57:40
---

```swift
//
//  1001-a_minus_b.swift
//  Algorithm
//
//  Created by Yujean Cho on 2022/02/14.
//

import Foundation

let line = readLine()!
let lineArr = line.split(separator: " ")
let a = Int(lineArr[0])!
let b = Int(lineArr[1])!
print(a-b)
```