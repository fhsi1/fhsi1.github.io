---
title:  "Two Sum"
excerpt: "#Array #Hash Table"
header:
  teaser: /assets/images/icon/swift.png
toc: true
toc_icon: "check-circle"
toc_sticky: true

categories:
  - Algorithm
tags:
  - Swift
last_modified_at: 2022-08-18 13:29:24
---

## 1. Two Sum

정수 배열 `nums` 과 정수 `target` 이 주어지면 <br>
배열 내에서 합이 `target` 이 되는 두 숫자의 인덱스를 반환하도록 작성하라.<br>

```
Example 1:
    Input: nums = [2,7,11,15], target = 9
    Output: [0,1]
    Explanation: Because nums[0] + nums[1] == 9, we return [0, 1].

Example 2:
    Input: nums = [3,2,4], target = 6
    Output: [1,2]

Example 3:
    Input: nums = [3,3], target = 6
    Output: [0,1]
 

Constraints:
    2 <= nums.length <= 10^4
    -10^9 <= nums[i] <= 10^9
    -10^9 <= target <= 10^9
    Only one valid answer exists.

```

## Solution

```swift
class Solution {
    func twoSum(_ nums: [Int], _ target: Int) -> [Int] {
        for i in 0..<nums.count {
            for j in 1+i..<nums.count {
                if nums[i] + nums[j] == target {
                    return [i, j]
                }
            }
        }
        return []
    }
}
```

이중 `for` 문으로 두 개의 요소의 합이 `target` 이 되는지를 확인하는 방법으로 구현하였다.<br>
`target` 과 일치하는 합을 찾는다면 해당 요소의 인덱스를 넣은 배열을 반환한다.<br>

---
> 📚 Reference <br>
[LeetCode-1-TwoSum](https://leetcode.com/problems/two-sum/)
