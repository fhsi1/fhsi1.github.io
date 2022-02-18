---
title:  "[Swift] 10172 - 개"
excerpt: "주어진 예제처럼 출력하는 문제"
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
last_modified_at: 2022-02-16 16:53:29
---

## 🧪 Problem

아래 예제와 같이 개를 출력하시오.

### Input

없음

### Output

```shell
|\_/|
|q p|   /}
( 0 )"""\
|"^"`    |
||_/=\\__|
```

## 💡 Solution

앞서 풀었던 문제인 [고양이](https://fhsi1.github.io/algorithm/swift-algorithm-10171-cat/) 에서 두 번째로 다뤘던 방법으로 해결해 보았다.

```swift
//
//  10172-Dog.swift
//  Algorithm
//
//  Created by Yujean Cho on 2022/02/13.
//

import Foundation

let dog = #"""
|\_/|
|q p|   /}
( 0 )"""\
|"^"`    |
||_/=\\__|
"""#
print(dog)
```

> 📚 Reference <br>
[multi-line strings](https://www.hackingwithswift.com/articles/162/how-to-use-raw-strings-in-swift)