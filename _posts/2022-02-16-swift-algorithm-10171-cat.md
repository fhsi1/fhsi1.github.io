---
title:  "[Swift] 10171 - 고양이"
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
last_modified_at: 2022-02-16 16:51:25
---

## 🧪 Problem

아래 예제와 같이 고양이를 출력하시오.

### Input

없음

### Output

```shell
\    /\
 )  ( ')
(  /  )
 \(__)|
```

## 💡 Solution

첫 번째 방법으로는 <br>
단순히 `print` 함수를 반복하여 고양이를 출력하는 방법이 있다. <br>

```swift
//
//  10171-Cat.swift
//  Algorithm
//
//  Created by Yujean Cho on 2022/02/13.
//

import Foundation

print("\\    /\\")
print(" )  ( ')")
print("(  /  )")
print(" \\(__)|")
```

한 개의 `\` 를 출력하기 위해서는 두 개를 입력해야 한다. <br>
즉, `\\` 와 같이 입력하면 된다. <br>

---

두 번째 방법으로는 <br>
여러 줄의 문자열을 한 번에 변수로 받아 출력하는 방법이 있다. <br>

```swift
//
//  10171-Cat.swift
//  Algorithm
//
//  Created by Yujean Cho on 2022/02/13.
//

import Foundation

let cat = #"""
\    /\
 )  ( ')
(  /  )
 \(__)|
"""#
print(cat)
```

`"""` 와 같이 큰 따옴표 세 개로 여러 줄의 문자열을 감싸주면 된다. <br>

일반적인 문자만 있는 경우는 따옴표 세 개로 해결이 되지만, <br>
고양이를 출력하기 위해서는 특수기호가 포함되어야 한다. <br>

특수기호를 포함한 여러 줄의 문자열을 변수로 받고 싶다면, <br>
세 개의 큰 따옴표를 감싼 뒤에 `#` 으로 한 번 더 감싸주면 된다. <br>

한 줄의 문자열인 경우에도 특수기호를 포함하고 싶다면, <br>
`#` 을 감싸주면 된다. <br>

> 📚 Reference <br>
[multi-line strings](https://www.hackingwithswift.com/articles/162/how-to-use-raw-strings-in-swift)