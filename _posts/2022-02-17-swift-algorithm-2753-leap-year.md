---
title:  "[Swift] 2753 - 윤년"
excerpt: "윤년을 판별하는 문제"
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
last_modified_at: 2022-02-17 17:40:35
---

```swift
//
//  2753-LeapYear.swift
//  Algorithm
//
//  Created by Yujean Cho on 2022/02/16.
//

import Foundation

let input = Int(readLine()!)!

func isLeapYear (year:Int) -> Int {
    if ((year % 4 == 0) && (year % 100 != 0)) || (year % 400 == 0) {
        return (1)
    }
    return (0)
}

let result = isLeapYear(year: input)
print(result)
```