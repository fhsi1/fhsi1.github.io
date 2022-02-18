---
title:  "[Swift] 2739 - 구구단"
excerpt: "구구단을 출력하는 문제"
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
last_modified_at: 2022-02-18 22:06:01
---

```swift
//
//  2739-MultiplicationTable.swift
//  Algorithm
//
//  Created by Yujean Cho on 2022/02/17.
//

import Foundation

let input = Int(readLine()!)!

let table = #"""
\#(input) * 1 = \#(input * 1)
\#(input) * 2 = \#(input * 2)
\#(input) * 3 = \#(input * 3)
\#(input) * 4 = \#(input * 4)
\#(input) * 5 = \#(input * 5)
\#(input) * 6 = \#(input * 6)
\#(input) * 7 = \#(input * 7)
\#(input) * 8 = \#(input * 8)
\#(input) * 9 = \#(input * 9)
"""#

print(table)

```