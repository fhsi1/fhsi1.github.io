---
title:  "[Swift] 2588 - 곱셈"
excerpt: "빈 칸에 들어갈 수는?"
header:
  teaser: /assets/images/icon/swift.png
toc: true
toc_icon: "check-circle"
toc_sticky: true

categories:
  - Algorithm
tags:
  - 백준
  - Swift
last_modified_at: 2022-02-16 17:20:55
---

```swift
//
//  2588-Multiplication.swift
//  Algorithm
//
//  Created by Yujean Cho on 2022/02/16.
//

import Foundation

let input1 = Int(readLine()!)!
let input2 = Int(readLine()!)!

func seperate(input1:Int, input2:Int) -> Int {
    var one:Int
    var ten:Int
    var hund:Int
    
    one = input2 % 10
    ten = input2 % 100 - one
    hund = input2 % 1000 - (ten + one)
    
    print(input1 * one)
    print(input1 * ten / 10)
    print(input1 * hund / 100)
    
    return (input1 * input2)
}

let result = seperate(input1:input1, input2:input2)

print(result)
```