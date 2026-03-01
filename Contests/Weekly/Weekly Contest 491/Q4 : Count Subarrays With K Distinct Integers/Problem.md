# 📊 [Q4. Count Subarrays With K Distinct Integers](https://leetcode.com/contest/weekly-contest-491/problems/count-subarrays-with-k-distinct-integers/)

<p align="center">
  <img src="https://img.shields.io/badge/Platform-LeetCode-orange?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Difficulty-Hard-red?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Category-Arrays-blue?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Topic-Sliding%20Window%20%26%20Hashing-purple?style=for-the-badge"/>
</p>

---

## 📌 Problem Statement

You are given:

- An integer array `nums`
- Two integers `k` and `m`

Return the number of subarrays such that:

1. The subarray contains **exactly `k` distinct integers**.
2. Each distinct integer in the subarray appears **at least `m` times**.

---

## 🔍 Definition

A **subarray** is a contiguous, non-empty sequence of elements within an array.

---

## 🎯 Task

Count all valid subarrays that satisfy:

- Exactly `k` distinct elements  
- Every distinct element has frequency ≥ `m`

---

## 🧾 Examples

### 🟢 Example 1

**Input**

nums = [1,2,1,2,2], k = 2, m = 2


**Output**

2


**Explanation**

Valid subarrays:

| Subarray | Distinct | Frequency |
|----------|----------|-----------|
| [1,2,1,2] | {1,2} → 2 | {1:2, 2:2} |
| [1,2,1,2,2] | {1,2} → 2 | {1:2, 2:3} |

Total = **2**

---

### 🟢 Example 2

**Input**

nums = [3,1,2,4], k = 2, m = 1


**Output**

3


**Explanation**

Valid subarrays:

| Subarray | Distinct | Frequency |
|----------|----------|-----------|
| [3,1] | {3,1} → 2 | {3:1, 1:1} |
| [1,2] | {1,2} → 2 | {1:1, 2:1} |
| [2,4] | {2,4} → 2 | {2:1, 4:1} |

Total = **3**

---

## 📎 Constraints

- `1 ≤ nums.length ≤ 10^5`
- `1 ≤ nums[i] ≤ 10^5`
- `1 ≤ k, m ≤ nums.length`

---

## 🏷️ Tags

- Arrays
- Sliding Window
- Hash Map
- Two Pointers
- Frequency Counting

---

> 💡 This problem combines distinct element tracking with frequency constraints inside a sliding window framework.
