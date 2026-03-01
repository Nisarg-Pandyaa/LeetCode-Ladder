# 💰 [Q2. Minimum Cost to Split into Ones](https://leetcode.com/contest/weekly-contest-491/problems/minimum-cost-to-split-into-ones/description/)

<p align="center">
  <img src="https://img.shields.io/badge/Platform-LeetCode-orange?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Difficulty-Medium-yellow?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Category-Mathematics-blue?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Topic-Dynamic%20Programming%20%26%20Greedy-purple?style=for-the-badge"/>
</p>

---

## 📌 Problem Statement

You are given an integer `n`.

In one operation, you may split an integer `x` into two positive integers `a` and `b` such that:


a + b = x


The cost of this operation is:


a * b


---

## 🎯 Task

Return the **minimum total cost** required to split the integer `n` into exactly `n` ones.

---

## 🧾 Examples

### 🟢 Example 1

**Input**

n = 3


**Output**

3


**Explanation**

One optimal sequence of operations:

| x | a | b | a + b | a * b | Cost |
|---|---|---|-------|-------|------|
| 3 | 1 | 2 | 3 | 2 | 2 |
| 2 | 1 | 1 | 2 | 1 | 1 |

Total minimum cost:


2 + 1 = 3


---

### 🟢 Example 2

**Input**

n = 4


**Output**

6


**Explanation**

One optimal sequence:

| x | a | b | a + b | a * b | Cost |
|---|---|---|-------|-------|------|
| 4 | 2 | 2 | 4 | 4 | 4 |
| 2 | 1 | 1 | 2 | 1 | 1 |
| 2 | 1 | 1 | 2 | 1 | 1 |

Total minimum cost:


4 + 1 + 1 = 6


---

## 📎 Constraints

- `1 ≤ n ≤ 500`

---

## 🏷️ Tags

- Mathematics
- Dynamic Programming
- Greedy Strategy
- Recursion
- Divide and Conquer

---

> 💡 This problem explores optimal splitting strategies to minimize cumulative multiplication cost.
