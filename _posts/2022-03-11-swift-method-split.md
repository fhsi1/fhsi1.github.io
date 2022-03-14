---
title:  "split"
excerpt: "split(separator:maxSplits:omittingEmptySubsequences:)"
header:
  teaser: /assets/images/icon/swift.png
toc: true
toc_icon: "check-circle"
toc_sticky: true

categories:
  - iOS
tags:
  - Swift
last_modified_at: 2022-03-11 02:49:02
---

# ✨ split(separator:maxSplits:omittingEmptySubsequences:)
> Returns the longest possible subsequences of the collection, in order, around elements equal to the given element.

➡ 주어진 요소와 동일한 요소를 중심으로, 가능한 가장 긴 부분 수열을 순서대로 반환한다.

## Declaration
```swift
func split(separator: Character, maxSplits: Int = 
	Int.max, omittingEmptySubsequences: Bool = true) -> 
	[Substring]
```

## Parameters
### separator
> The element that should be split upon.

➡ 분할하고자 하는 요소

### maxSplits
> The maximum number of times to split the collection, or one less than the number of subsequences to return. <br>
> If `maxSplits + 1` subsequences are returned, the last one is a suffix of the original collection containing the remaining elements. <br>
> `maxSplits` must be greater than or equal to zero. <br>
> The default value is `Int.max`. <br>

➡ 컬렉션을 분할할 수 있는 최대 횟수, 또는 반환하는 수열의 수보다 1회 적은 수 <br>
➡ `maxSplit + 1` 부분 수열이 반환되면, 마지막 요소는 나머지 요소가 포함된 원본 컬렉션의 접미사이다. <br>
➡ `Int.max` 는 `0` 보다 크거나 같아야 한다. <br>
➡ 기본값은 `Int.max` 이다. <br>

### omittingEmptySubsequences
> If `false`, an empty subsequence is returned in the result for each consecutive pair of `separator` elements in the collection and for each instance of `separator` at the start or end of the collection. <br>
> If `true`, only nonempty subsequences are returned. <br>
> The default value is `true`. <br>

➡ `false` 일 경우, `seperaotr` 의 인스턴스마다 결과에 빈 부분 수열을 반환한다. <br>
➡ `true` 일 경우, 비어있지 않은 수열만 반환된다. <br>
➡ 기본값은 `true` 이다. <br>

## Return Value
> An array of subsequences, split from this collection’s elements.

➡ 해당 컬렉션의 요소에서 분할된 부분 수열 배열

---

> 📚 Reference <br>
[split](https://developer.apple.com/documentation/swift/string/2894564-split)