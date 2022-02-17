---
title:  "[Swift] 10998 - A × B"
excerpt: "곱셈 문제"
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
last_modified_at: 2022-02-16 17:00:57
---

```swift
//
//  10998-a_multiple_b.swift
//  Algorithm
//
//  Created by Yujean Cho on 2022/02/14.
//

import Foundation

let line = readLine()!
let lineArr = line.split(separator: " ")
let a = Int(lineArr[0])!
let b = Int(lineArr[1])!
print(a*b)
```