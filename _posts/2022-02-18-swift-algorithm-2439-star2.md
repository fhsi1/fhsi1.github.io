---
title:  "[Swift] 2439 - 별 찍기 2"
excerpt: "별을 찍는 문제 2"
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
last_modified_at: 2022-02-18 22:17:08
---

```swift
//
//  2439-star2.swift
//  Algorithm
//
//  Created by Yujean Cho on 2022/02/17.
//

import Foundation

let num = Int(readLine()!)!

for i in 0..<num {
    var output = ""
    for _ in 1..<num - i {
        output.append(" ")
    }
    
    for _ in 0...i {
        output.append("*")
    }
    print(output)
}
```