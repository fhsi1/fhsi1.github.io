---
title:  "readLine"
excerpt: ""
header:
  teaser: /assets/images/icon/swift.png
toc: true
toc_icon: "check-circle"
toc_sticky: true

categories:
  - iOS
tags:
  - Swift
last_modified_at: 2022-03-11 00:29:26
---

# ✨ readLine(strippingNewline:)
> Returns a string read from standard input through the end of the current line or until EOF is reached.

➡ 표준 입력에서 **현재 줄 끝까지** 또는 **EOF 에 도달할 때까지** 읽은 문자열을 반환한다.

> cf. **EOF** [ End Of File ] <br>
> 파일의 끝 <br>
> 데이터 소스로부터 더 이상 읽을 수 있는 데이터가 없음을 나타낸다.<br>

## Declaration
```swift
func readLine(strippingNewline: Bool = true) ->
	String?
```

## Parameters
### strippingNewline
> If true, newline characters and character combinations are stripped from the result; <br>
> otherwise, newline characters or character combinations are preserved. <br>
> The default is true. <br>

➡ true 이면, 개행 문자와 문자 조합이 제거된다. <br>
➡ 그렇지 않으면, 개행 문자 또는 문자 조합이 유지된다. <br>
➡ 기본 값은 true 이다. <br>

## Return Value
> The string of characters read from standard input. <br>
> If EOF has already been reached when readLine() is called, the result is nil.<br>

➡ 표준 입력에서 읽은 문자열이다. <br>
➡ `readLine()` 이 호출될 때 `EOF` 에 이미 도달했다면, 결과값은 `nil` 이다.

---

> 📚 Reference <br>
[readLine](https://developer.apple.com/documentation/swift/1641199-readline/)