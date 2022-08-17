---
title:  "217. Contains Duplicate"
excerpt: "#Array #Hash Table #Sorting"
header:
  teaser: /assets/images/icon/swift.png
toc: true
toc_icon: "check-circle"
toc_sticky: true

categories:
  - Algorithm
tags:
  - Swift
last_modified_at: 2022-08-17 14:29:26
---

# 217. Contains Duplicate

주어진 정수 배열 `nums` 에 같은 값이 두 번 이상 나타나면 `true` 를 반환하고 <br>
모든 요소가 고유한 값이라면 `false` 를 반환하도록 작성하라.<br>

```
Example 1:
  Input: nums = [1,2,3,1]
  Output: true
  
Example 2:
  Input: nums = [1,2,3,4]
  Output: false

Example 3:
    Input: nums = [1,1,1,3,3,4,3,2,4,2]
    Output: true
 

Constraints:
  1 <= nums.length <= 10^5
  -109 <= nums[i] <= 10^9
```

## Solution

```swift
class Solution {
    func containsDuplicate(_ nums: [Int]) -> Bool {
        return Set(nums).count != nums.count
    }
}
```

입력값으로 들어온 `nums` 를 중복이 없도록 `Set` 으로 감싸주었을 때의 요소 개수와 <br>
원본 입력값 `nums` 의 요소 개수가 일치하는지를 비교하였다. <br>

---
> 📚 Reference <br>
[LeetCode-217-ContainsDuplicate](https://leetcode.com/problems/contains-duplicate/)
