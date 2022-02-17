---
title:  "[Swift] 14681 - 사분면 고르기"
excerpt: "점이 어느 사분면에 있는지 알아내는 문제"
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
last_modified_at: 2022-02-17 17:42:19
---

```swift
//
//  14681-Quadrant.swift
//  Algorithm
//
//  Created by Yujean Cho on 2022/02/16.
//

import Foundation

let x = Int(readLine()!)!
let y = Int(readLine()!)!

if (x > 0) && (y > 0) {
    print(1)
} else if (x < 0) && (y > 0) {
    print(2)
} else if (x < 0) && (y < 0) {
    print(3)
} else if (x > 0) && (y < 0) {
    print(4)
}
```