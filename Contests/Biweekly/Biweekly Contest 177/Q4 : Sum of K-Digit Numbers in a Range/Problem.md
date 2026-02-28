# 🔢 [Q4. Sum of K-Digit Numbers in a Range](https://leetcode.com/contest/biweekly-contest-177/problems/sum-of-k-digit-numbers-in-a-range/)

<p align="center">
  <img src="https://img.shields.io/badge/Platform-LeetCode-orange?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Difficulty-Hard-red?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Category-Mathematics-blue?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Topic-Combinatorics%20%26%20Modular%20Arithmetic-purple?style=for-the-badge"/>
</p>

---

## 📌 Problem Statement

You are given three integers:


l, r, k


---

## 🔍 Task

Consider all possible integers consisting of **exactly `k` digits**, where:

- Each digit is chosen independently  
- Each digit lies in the inclusive range:


[l, r]


If `0` is included in the range, **leading zeros are allowed**.

---

## 🎯 Return

Return the **sum of all such valid numbers**.

Since the result may be very large, return it modulo:


10^9 + 7


---

## 🧾 Examples

### 🟢 Example 1

**Input**

l = 1, r = 2, k = 2


**Output**

66


**Explanation**

All possible 2-digit numbers using digits in `[1,2]`:


11, 12, 21, 22


Total sum:

11 + 12 + 21 + 22 = 66


---

### 🟢 Example 2

**Input**

l = 0, r = 1, k = 3


**Output**

444


**Explanation**

All valid 3-digit combinations:


000, 001, 010, 011, 100, 101, 110, 111


Without leading zeros they represent:


0, 1, 10, 11, 100, 101, 110, 111


Total sum = 444

---

### 🟢 Example 3

**Input**

l = 5, r = 5, k = 10


**Output**

555555520


**Explanation**

Only possible number:


5555555555


Return:

5555555555 % (10^9 + 7) = 555555520


---

## 📎 Constraints

- `0 ≤ l ≤ r ≤ 9`
- `1 ≤ k ≤ 10^9`

---

## 🏷️ Tags

- Mathematics
- Combinatorics
- Modular Arithmetic
- Fast Exponentiation
- Number Construction

---

> 💡 This problem requires mathematical observation about digit contribution per position combined with modular exponentiation for very large `k`.
