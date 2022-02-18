---
title:  "[Swift] 2438 - 별 찍기 1"
excerpt: "별을 찍는 문제 1"
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
last_modified_at: 2022-02-18 22:15:59
---

```swift
//
//  2438-star1.swift
//  Algorithm
//
//  Created by Yujean Cho on 2022/02/17.
//

import Foundation

let num = Int(readLine()!)!

for i in 1...num {
    for _ in 1...i {
        print("*", terminator: "")
    }
    print("")
}
```