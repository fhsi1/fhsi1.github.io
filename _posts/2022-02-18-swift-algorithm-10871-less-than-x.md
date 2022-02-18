---
title:  "[Swift] 10871 - X보다 작은 수"
excerpt: "for와 if를 같이 쓰는 문제"
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
last_modified_at: 2022-02-18 22:18:28
---

```swift
//
//  10871-LessThanX.swift
//  Algorithm
//
//  Created by Yujean Cho on 2022/02/17.
//

import Foundation

let firstLine = readLine()!
let firstLineArr = firstLine.split(separator: " ")

let secondLine = readLine()!
var secondLineArr = secondLine.split(separator: " ")

for i in secondLineArr {
    if Int(i)! < Int(firstLineArr[1])! {
        print(i, terminator: " ")
    }
}
```