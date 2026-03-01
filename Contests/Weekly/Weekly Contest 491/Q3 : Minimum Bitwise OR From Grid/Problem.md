# 🔢 [Q3. Minimum Bitwise OR From Grid](https://leetcode.com/contest/weekly-contest-491/problems/minimum-bitwise-or-from-grid/)

<p align="center">
  <img src="https://img.shields.io/badge/Platform-LeetCode-orange?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Difficulty-Medium-yellow?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Category-Bit%20Manipulation-blue?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Topic-Greedy%20%26%20Bitwise%20OR-purple?style=for-the-badge"/>
</p>

---

## 📌 Problem Statement

You are given a 2D integer array `grid` of size `m × n`.

You must select **exactly one integer from each row** of the grid.

Return the **minimum possible bitwise OR** of the selected integers.

---

## 🎯 Task

- Choose one element from every row.
- Compute the bitwise OR (`|`) of the chosen elements.
- Minimize the resulting value.

---

## 🧾 Examples

### 🟢 Example 1

**Input**

grid = [[1,5],[2,4]]


**Output**

3


**Explanation**

Choose:
- `1` from the first row  
- `2` from the second row  


1 | 2 = 3


This is the minimum possible result.

---

### 🟢 Example 2

**Input**

grid = [[3,5],[6,4]]


**Output**

5


**Explanation**

Choose:
- `5` from the first row  
- `4` from the second row  


5 | 4 = 5


This is the minimum possible result.

---

### 🟢 Example 3

**Input**

grid = [[7,9,8]]


**Output**

7


**Explanation**

Only one row exists.  
Choosing `7` produces the minimum OR.

---

## 📎 Constraints

- `1 ≤ m == grid.length ≤ 10^5`
- `1 ≤ n == grid[i].length ≤ 10^5`
- `m * n ≤ 10^5`
- `1 ≤ grid[i][j] ≤ 10^5`

---

## 🏷️ Tags

- Bit Manipulation
- Greedy
- Matrix
- Optimization
- Combinatorics

---

> 💡 The challenge is to minimize the accumulated OR across rows while respecting the one-choice-per-row constraint.
