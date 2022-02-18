---
title:  "[Swift] 2557 - Hello World!"
excerpt: "Hello World!를 출력하시오."
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
last_modified_at: 2022-02-16 16:43:30
---

## 🧪 Problem

Hello World!를 출력하시오.

### Input

없음

### Output

```shell
Hello World!
```

## 💡 Solution

```swift
//
//  2557-HelloWorld.swift
//  Algorithm
//
//  Created by Yujean Cho on 2022/02/13.
//

import Foundation

print("Hello World!")
```

### 📖 print

```swift
func print(_ items: Any..., separator: String = " ", terminator: String = "\n")
```

**print** 함수는 단순히 하나의 인자를 받는 것 뿐만 아니라, <br>
여러가지 인자를 받을 수 있다. <br>

`terminator` 인자에 `"\n"` 이 기본으로 할당되어 있어, <br>
`terminator` 를 지정하지 않을 때 자동으로 개행이 포함된다. <br>

> 📚 Reference <br>
[print](https://developer.apple.com/documentation/swift/1541053-print)