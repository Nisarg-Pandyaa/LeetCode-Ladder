# 🔁 [Q3. Minimum Operations to Make Array Parity Alternating](https://leetcode.com/contest/biweekly-contest-177/problems/minimum-operations-to-make-array-parity-alternating/description/)

<p align="center">
  <img src="https://img.shields.io/badge/Platform-LeetCode-orange?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Difficulty-Medium-yellow?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Category-Arrays-blue?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Topic-Greedy%20%26%20Parity-purple?style=for-the-badge"/>
</p>

---

## 📌 Problem Statement

You are given an integer array `nums`.


---

## 🔍 Definition

An array is called **parity alternating** if for every index `i` where:


0 ≤ i < n - 1


The elements `nums[i]` and `nums[i + 1]` have **different parity**  
(one is even and the other is odd).

An array of length `1` is always considered parity alternating.

---

## ⚙️ Operation

In one operation, you may choose any index `i` and:

- Increase `nums[i]` by 1  
OR  
- Decrease `nums[i]` by 1  

---

## 🎯 Return

Return an integer array `answer` of length 2:

- `answer[0]` → Minimum number of operations required to make the array parity alternating.
- `answer[1]` → Minimum possible value of:


max(nums) - min(nums)


taken over all arrays that:

- Are parity alternating  
- Can be obtained using exactly `answer[0]` operations  

---

## 🧾 Examples

### 🟢 Example 1

**Input**

nums = [-2, -3, 1, 4]


**Output**

[2, 6]


**Explanation**

Operations performed:

1. Increase `nums[2]` by 1 → `[-2, -3, 2, 4]`
2. Decrease `nums[3]` by 1 → `[-2, -3, 2, 3]`

The array becomes parity alternating.

Range:

max - min = 3 - (-3) = 6


---

### 🟢 Example 2

**Input**

nums = [0, 2, -2]


**Output**

[1, 3]


**Explanation**

Operation:

- Decrease `nums[1]` by 1 → `[0, 1, -2]`

Now parity alternating.

Range:

1 - (-2) = 3


---

### 🟢 Example 3

**Input**

nums = [7]


**Output**

[0, 0]


**Explanation**

No operations required.

Range:

7 - 7 = 0


---

## 📎 Constraints

- `1 ≤ nums.length ≤ 10^5`
- `-10^9 ≤ nums[i] ≤ 10^9`

---

## 🏷️ Tags

- Arrays
- Greedy
- Parity Logic
- Optimization
- Simulation

---

> 💡 This problem combines parity pattern enforcement with optimization over value range under minimum-operation constraints.
