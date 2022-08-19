---
title:  "Best Time to Buy and Sell Stock"
excerpt: "#Array #Dynamic Programming"
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
last_modified_at: 2022-08-19 16:23:24
---

## 121. Best Time to Buy and Sell Stock

`price[i]` 는 `i` 번째 날에 주어진 주식의 가격을 나타낸다.<br>

이익을 최대화할 수 있는 매수 시점과 매도 시점을 구해 <br>
최대 이익을 반환하도록 작성하라.<br>

이익을 얻을 수 없다면 `0` 을 반환한다.<br>

```
Example 1:
    Input: prices = [7,1,5,3,6,4]
    Output: 5
    Explanation: Buy on day 2 (price = 1) and sell on day 5 (price = 6), profit = 6-1 = 5.
    Note that buying on day 2 and selling on day 1 is not allowed because you must buy before you sell.

Example 2:
    Input: prices = [7,6,4,3,1]
    Output: 0
    Explanation: In this case, no transactions are done and the max profit = 0.
 

Constraints:
    1 <= prices.length <= 10^5
    0 <= prices[i] <= 10^4
```

## Solution

```swift
class Solution {
    func maxProfit(_ prices: [Int]) -> Int {
        if prices.isEmpty {
            return 0
        }
        
        var buyIndex = prices[0]
        var profit = 0
        
        for price in prices {
            if price < buyIndex {
                buyIndex = price
            } else if (price - buyIndex) > profit {
                profit = price - buyIndex
            }
        }
        
        return profit
    }
}
```

매개변수 `prices` 가 비어있을 경우 `0` 을 리턴하고 종료한다. <br>

매수시점의 가격을 나타내는 변수 `buyIndex` 를 `prices[0]` 으로 초기화하고,<br>
최대 이익을 연산하여 그 결과값을 담을 변수 `profit` 을 `0` 으로 초기화한다.<br>

`prices` 를 순회하면서 `price` 와 `buyIndex` 를 비교하여 작은 값을 찾는다.<br>
이는 낮은 가격에 구매해야 이익을 많이 볼 수 있기 때문이다.<br>

그리고 `0` 으로 초기화 했었던 `profit` 과 비교하여 `(price - buyIndex)`<br>
즉, 이익연산을 하였을 때 `profit` 보다 크다면 `profit` 에 대입하여 최대 이익을 찾는다. <br>

---
> 📚 Reference <br>
[LeetCode-121-BestTimeToBuyAndSellStock](https://leetcode.com/problems/best-time-to-buy-and-sell-stock/)
