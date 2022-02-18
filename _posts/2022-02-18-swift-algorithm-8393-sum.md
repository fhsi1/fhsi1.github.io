---
title:  "[Swift] 8393 - 합"
excerpt: "1부터 N까지의 합을 구하는 문제"
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
last_modified_at: 2022-02-18 22:08:53
---

```swift
//
//  8393-Sum.swift
//  Algorithm
//
//  Created by Yujean Cho on 2022/02/17.
//

import Foundation

let num = Int(readLine()!)!

var sum = 0
for i in 0...num {
    sum += i
}

print(sum)
```