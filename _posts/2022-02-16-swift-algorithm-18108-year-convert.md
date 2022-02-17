---
title:  "[Swift] 18108 - 1998년생인 내가 태국에서는 2541년생?!"
excerpt: "식을 직접 세워서 계산하는 문제"
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
last_modified_at: 2022-02-16 17:13:41
---

```swift
//
//  18108-YearConvert.swift
//  Algorithm
//
//  Created by Yujean Cho on 2022/02/15.
//

import Foundation

var input = Int(readLine()!)!

print(input - 544 + 1)
```

```swift
//
//  18108-YearConvert.swift
//  Algorithm
//
//  Created by Yujean Cho on 2022/02/15.
//

import Foundation

var input = Int(readLine()!)!

func convert(year:Int) -> Int {
    return (year - 544 + 1)
}

let result = convert(year: input)
print(result)
```