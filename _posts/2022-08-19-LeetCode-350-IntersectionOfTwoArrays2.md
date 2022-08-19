---
title:  "Intersection of Two Arrays II"
excerpt: "#Array #Hash Table #Two Pointers"
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
last_modified_at: 2022-08-19 16:08:45
---

## 350. Intersection of Two Arrays II

주어진 두 개의 정수 배열 `nums1` 과 `nums2` 의 <br>
교집합 배열을 반환하도록 작성하라.<br>

결과의 각 요소는 두 배열에 표시되는 횟수만큼 모두 나타나야한다. <br>

```
Example 1:
    Input: nums1 = [1,2,2,1], nums2 = [2,2]
    Output: [2,2]

Example 2:
    Input: nums1 = [4,9,5], nums2 = [9,4,9,8,4]
    Output: [4,9]
    Explanation: [9,4] is also accepted.
 

Constraints:
    1 <= nums1.length, nums2.length <= 1000
    0 <= nums1[i], nums2[i] <= 1000
```

## Solution

```swift
class Solution {
    func intersect(_ nums1: [Int], _ nums2: [Int]) -> [Int] {
        var res: [Int] = []
        
        var nums2 = nums2
        for num in nums1 {
            if nums2.contains(num) {
                res.append(num)
                nums2.remove(at: nums2.firstIndex(of: num)!)
            }
        }
        
        return res
    }
}
```

`nums1` 의 요소를 `num` 로 순회하면서 `nums2` 에 포함하고 있는지 확인한다.<br>
포함하고 있다면 `num` 을 결과로 반환할 배열 `res` 에 넣어준다.<br>

`nums2` 에 `num` 이 들어있는지 확인을 완료했으므로,<br>
확인한 `nums2` 내의 `num` 요소를 삭제해주어야 한다.<br>

---
> 📚 Reference <br>
[LeetCode-350-IntersectionOfTwoArrays2](https://leetcode.com/problems/intersection-of-two-arrays-ii/)
