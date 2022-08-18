---
title:  "Merge Sorted Array"
excerpt: "#Array #Two Pointers #Sorting"
header:
  teaser: /assets/images/icon/swift.png
toc: true
toc_icon: "check-circle"
toc_sticky: true

categories:
  - Algorithm
tags:
  - Swift
  - LeetCode
last_modified_at: 2022-08-18 14:08:33
---

## 88. Merge Sorted Array

정렬되지 않은 두 개의 정수 배열 `nums1`, `nums2` 이 주어지고 <br>
각 배열의 요소 수를 나타내는 두 정수 `m`, `n` 이 주어질 것이다.<br>

`nums1` 과 `nums2` 를 내림차순으로 정렬된 단일 배열로 병합하도록 작성하라.<br>

최종적으로 정렬된 배열은 함수에 의해 반환되는 것이 아니라 `nums1` 에 저장되어야 한다. <br>

```
Example 1:
    Input: nums1 = [1,2,3,0,0,0], m = 3, nums2 = [2,5,6], n = 3
    Output: [1,2,2,3,5,6]
    Explanation: The arrays we are merging are [1,2,3] and [2,5,6].
    The result of the merge is [1,2,2,3,5,6] with the underlined elements coming from nums1.

Example 2:
    Input: nums1 = [1], m = 1, nums2 = [], n = 0
    Output: [1]
    Explanation: The arrays we are merging are [1] and [].
    The result of the merge is [1].

Example 3:
    Input: nums1 = [0], m = 0, nums2 = [1], n = 1
    Output: [1]
    Explanation: The arrays we are merging are [] and [1].
    The result of the merge is [1].
    Note that because m = 0, there are no elements in nums1. The 0 is only there to ensure the merge result can fit in nums1.


Constraints:
    nums1.length == m + n
    nums2.length == n
    0 <= m, n <= 200
    1 <= m + n <= 200
    -10^9 <= nums1[i], nums2[j] <= 10^9
```

## Solution

```swift
class Solution {
    func merge(_ nums1: inout [Int], _ m: Int, _ nums2: [Int], _ n: Int) {
        var res: [Int] = [Int]()
        
        if m > 0 {
            for i in 0..<m {
            res.append(nums1[i])
            }
        }
        
        if n > 0 {
            for i in 0..<n {
            res.append(nums2[i])
            }
        }
        
        nums1 = res.sorted(by: <)
    }
}
```

`nums1` 을 `m` 만큼 `nums2` 를 `n` 만큼 `res` 배열에 넣고 <br>
오름차순으로 정렬하도록 구현하였다. <br>

`nums1` 을 `inout` 으로 mutable 하게 준 부분을 잘 활용하면 좋을 것 같다..😅<br>

---
> 📚 Reference <br>
[LeetCode-88-MergeSortedArray](https://leetcode.com/problems/merge-sorted-array/)
