---
title:  "Maximum Subarray"
excerpt: "#Array #Divide and Conquer"
header:
  teaser: /assets/images/icon/swift.png
toc: true
toc_icon: "check-circle"
toc_sticky: true

categories:
  - Algorithm
tags:
  - Swift
last_modified_at: 2022-08-17 19:05:36
---

## 53. Maximum Subarray

주어진 정수 배열 `nums` 에서 연속적인 하위 배열의 합 중<br>
가장 큰 값을 구하도록 작성하라.<br>

하위 배열은 연속적인 배열이다. <br>

```
Example 1:
    Input: nums = [-2,1,-3,4,-1,2,1,-5,4]
    Output: 6
    Explanation: [4,-1,2,1] has the largest sum = 6.

Example 2:
    Input: nums = [1]
    Output: 1

Example 3:
    Input: nums = [5,4,-1,7,8]
    Output: 23


Constraints:
    1 <= nums.length <= 10^5
    -10^4 <= nums[i] <= 10^4
```

## Solution

```swift
class Solution {
    func maxSubArray(_ nums: [Int]) -> Int {
        var nums = nums
        for index in 1..<nums.count {
            if nums[index - 1] > 0 {
                nums[index] += nums[index - 1]
            }
        }
        return nums.max() ?? 0
    }
}
```

입력값으로 들어온 `nums` 를 지역변수 `nums` 에 받아 초기화하였다.<br>

연속적인 하위 배열 중에서 가장 큰 값을 구하면 되기 때문에<br>
`nums[index - 1]` 이 양수인지 확인하는 조건을 추가하였다.<br>
양수라면 값을 더해 `nums[index]` 에 넣어준다.

반복문을 모두 돌고 나면 연산이 끝난 배열 `nums` 가 되었을 것이다.<br>
배열의 최댓값이 문제에서 요구한 값이 된다.<br>

---
> 📚 Reference <br>
[LeetCode-53-MaximumSubarray](https://leetcode.com/problems/maximum-subarray/)
