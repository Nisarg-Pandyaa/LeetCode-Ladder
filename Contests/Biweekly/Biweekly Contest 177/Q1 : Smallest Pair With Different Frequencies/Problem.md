# 🔎 [Q1. Smallest Pair With Different Frequencies](https://leetcode.com/contest/biweekly-contest-177/problems/smallest-pair-with-different-frequencies/)

<p align="center">
  <img src="https://img.shields.io/badge/Platform-LeetCode-orange?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Difficulty-Easy-green?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Category-Hashing-blue?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Topic-Frequency%20Counting-purple?style=for-the-badge"/>
</p>

---

## 📌 Problem Statement

You are given an integer array `nums`.

Consider all pairs of **distinct values** `x` and `y` from `nums` such that:

- `x < y`
- `x` and `y` have **different frequencies** in `nums`

Among all such pairs:

1. Choose the pair with the **smallest possible value of `x`**.
2. If multiple pairs have the same `x`, choose the one with the **smallest possible value of `y`**.

Return an integer array:


[x, y]


If no valid pair exists, return:


[-1, -1]


---

## 📖 Definitions

The **frequency** of a value `x` is the number of times it appears in the array.

---

## 🧾 Examples

### 🟢 Example 1

**Input**

nums = [1,1,2,2,3,4]


**Output**

[1,3]


**Explanation**

- Frequency of 1 → 2  
- Frequency of 2 → 2  
- Frequency of 3 → 1  
- Frequency of 4 → 1  

Smallest value is `1` (frequency = 2).  
The smallest value greater than `1` with a different frequency is `3` (frequency = 1).  

So the answer is `[1, 3]`.

---

### 🟢 Example 2

**Input**

nums = [1,5]


**Output**

[-1,-1]


**Explanation**

Both values have the same frequency (1).  
No valid pair exists.

---

### 🟢 Example 3

**Input**

nums = [7]


**Output**

[-1,-1]


**Explanation**

Only one value exists in the array.  
No valid pair can be formed.

---

## 📎 Constraints

- `1 ≤ nums.length ≤ 100`
- `1 ≤ nums[i] ≤ 100`

---

## 🏷️ Tags

- Hash Map
- Frequency Counting
- Sorting
- Implementation

---

> 💡 This problem tests frequency analysis and careful pair selection under ordering constraints.
