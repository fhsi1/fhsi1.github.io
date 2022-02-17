---
title:  "[Swift] 2525 - 오븐 시계"
excerpt: "범위가 더 넓은 시간 계산 문제"
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
last_modified_at: 2022-02-17 17:45:39
---

```swift
//
//  2525-OvenClock.swift
//  Algorithm
//
//  Created by Yujean Cho on 2022/02/16.
//

import Foundation

let time = readLine()!
let timeItTakes = Int(readLine()!)!
let timeArr = time.split(separator: " ")

var a = Int(timeArr[0])!
var b = Int(timeArr[1])!

b += timeItTakes
while (b >= 60) {
    a += 1
    b -= 60
}
while (a >= 24) {
    a -= 24
}

print("\(a) \(b)")
```