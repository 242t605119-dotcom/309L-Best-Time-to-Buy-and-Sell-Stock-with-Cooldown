# LeetCode 309 - Best Time to Buy and Sell Stock with Cooldown

## Problem Statement

You are given an array `prices` where `prices[i]` represents the stock price on day `i`.

You may buy and sell stocks, but after selling a stock, you must wait one day before buying again.

Return the maximum profit possible.

## Example 1

### Input

```text
prices = [1,2,3,0,2]
```

### Output

```text
3
```

## Example 2

### Input

```text
prices = [1]
```

### Output

```text
0
```

## Approach

Use **Dynamic Programming** with three states:

* `hold` — maximum profit while holding a stock.
* `sold` — maximum profit after selling a stock.
* `cooldown` — maximum profit while waiting after a sale.

## Algorithm

1. Initialize the three states.
2. For each price, update the `hold`, `sold`, and `cooldown` states.
3. Buying is allowed only when not in the cooldown state.
4. Selling moves the state to `sold`.
5. Return the maximum of `sold` and `cooldown`.

## Time Complexity

`O(n)`

## Space Complexity

`O(1)`

## Key Concepts

* Dynamic Programming
* State Management
* Stock Trading
* Cooldown Constraint

## Language

Python

## LeetCode Details

* **Problem:** 309
* **Title:** Best Time to Buy and Sell Stock with Cooldown
* **Difficulty:** Medium

## Author

**T. Nandhini Reddy**

GitHub: `242t605119-dotcom`
