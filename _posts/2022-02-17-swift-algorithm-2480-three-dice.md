---
title:  "[Swift] 2480 - 주사위 세 개"
excerpt: "조건에 따라 상금을 계산하는 문제"
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
last_modified_at: 2022-02-17 17:46:45
---

```swift
//
//  2480-ThreeDice.swift
//  Algorithm
//
//  Created by Yujean Cho on 2022/02/16.
//

import Foundation

let line = readLine()!
let lineArr = line.split(separator: " ")

var a = Int(lineArr[0])!
var b = Int(lineArr[1])!
var c = Int(lineArr[2])!

var sameNum = 0
var reward = 0
var maxDice = 0

func isMax(n1:Int, n2:Int, n3:Int) -> Int {
    var max = 0
    
    if ((a > b) && (a > c)) {
        max = a
    } else if ((b > a) && (b > c)) {
        max = b
    } else if ((c > a) && (c > b)) {
        max = c
    }
    return (max)
}

func isSameTwo(n1:Int, n2:Int, n3:Int) -> Int {
    if (n1 == n2) || (n1 == n3) {
        return (n1)
    } else if (n2 == n3) {
        return (n2)
    }
    return (0)
}

if ((a == b) && (b == c) && (c == a)) {
    reward = 10000 + a * 1000
} else if ((a != b) && (b != c) && (c != a)) {
    maxDice = isMax(n1: a, n2: b, n3: c)
    reward = maxDice * 100
} else {
    sameNum = isSameTwo(n1: a, n2: b, n3: c)
    if (sameNum != 0) {
        reward = 1000 + sameNum * 100
    }
}

print(reward)
```