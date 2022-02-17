---
title:  "[Swift] 2884 - 알람 시계"
excerpt: "시간 계산 문제"
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
last_modified_at: 2022-02-17 17:44:31
---

```swift
//
//  2884-Alarm.swift
//  Algorithm
//
//  Created by Yujean Cho on 2022/02/16.
//

import Foundation

let time = readLine()!
let timeArr = time.split(separator: " ")

var h = Int(timeArr[0])!
var m = Int(timeArr[1])!


m -= 45
while (m < 0) {
    h -= 1
    m += 60
}
while (h < 0) {
    h += 24
}
while (h >= 24) {
    h -= 24
}

print("\(h) \(m)")
```