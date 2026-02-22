# 🔥 Q4. Count Sequences to K

<p align="center">
  <img src="https://img.shields.io/badge/Difficulty-Hard-red?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Category-Backtracking-blue?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Topic-Dynamic%20Programming-green?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Concept-Rational%20Math-purple?style=for-the-badge"/>
</p>

---

## 📌 [Problem Description (on LeetCode)](https://leetcode.com/contest/weekly-contest-490/problems/count-sequences-to-k/description/)

You are given:

- An integer array `nums`
- An integer `k`

You start with an initial value:
val = 1


You must process the array `nums` from **left to right**.

At each index `i`, you must choose **exactly one** of the following actions:

1. Multiply `val` by `nums[i]`
2. Divide `val` by `nums[i]`
3. Leave `val` unchanged

---

### 🎯 Goal

After processing all elements, `val` is considered equal to `k` **only if its final rational value exactly equals `k`**.

Return the **count of distinct sequences of choices** that result in:


val == k

---

## ⚠️ Important Notes

- Division is **rational (exact)**, not integer division.
- Example:

2 / 4 = 1 / 2


- Each sequence must choose **one operation per element**.
- Different operation choices count as distinct sequences.

---

## 🧾 Examples

---

### 🟢 Example 1

**Input:**

nums = [2, 3, 2]
k = 6
**Output:**

2


**Explanation:**

| Sequence | nums[0] | nums[1] | nums[2] | Final val |
|----------|---------|---------|---------|-----------|
| 1 | Multiply → 2 | Multiply → 6 | Leave | 6 |
| 2 | Leave | Multiply → 3 | Multiply → 6 | 6 |

There are **2 valid sequences**.

---

### 🟢 Example 2

**Input:**

nums = [4, 6, 3]
k = 2
**Output:**

2


**Explanation:**

| Sequence | nums[0] | nums[1] | nums[2] | Final val |
|----------|---------|---------|---------|-----------|
| 1 | Multiply → 4 | Divide → 2/3 | Multiply → 2 | 2 |
| 2 | Leave | Multiply → 6 | Divide → 2 | 2 |

There are **2 valid sequences**.

---

### 🟢 Example 3

**Input:**

nums = [1, 5]
k = 1
**Output:**

3

**Explanation:**

| Sequence | nums[0] | nums[1] | Final val |
|----------|---------|---------|-----------|
| 1 | Multiply → 1 | Leave | 1 |
| 2 | Divide → 1 | Leave | 1 |
| 3 | Leave | Leave | 1 |

There are **3 valid sequences**.

---

## 📎 Constraints

- `1 <= nums.length <= 19`
- `1 <= nums[i] <= 6`
- `1 <= k <= 10^15`

---

## 🏷️ Tags

- Backtracking
- Dynamic Programming
- Combinatorics
- Rational Arithmetic
- State Exploration

---

> 💡 This problem tests combinatorial exploration with rational state transitions and requires careful handling of multiplication and division states.
