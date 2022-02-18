---
title:  "[Swift] 10950 - A + B"
excerpt: "A+B를 여러 번 출력하는 문제"
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
last_modified_at: 2022-02-18 22:08:38
---

```swift
//
//  10950-a_plus_b.swift
//  Algorithm
//
//  Created by Yujean Cho on 2022/02/17.
//

import Foundation

let testCase = Int(readLine()!)!

var i = 0
while (i < testCase) {
    
    let line = readLine()!
    let lineArr = line.split(separator: " ")
    let a = Int(lineArr[0])!
    let b = Int(lineArr[1])!
    
    print(a+b)
    
    i += 1
}
```