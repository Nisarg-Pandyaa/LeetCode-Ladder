# 🔢 Q2. Check Digitorial Permutation

<p align="center">
  <img src="https://img.shields.io/badge/Difficulty-Medium-orange?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Category-Math-blue?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Topic-Permutation-green?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Concept-Factorial-purple?style=for-the-badge"/>
</p>

---

## 📌 [Problem Description (on LeetCode)](https://leetcode.com/contest/weekly-contest-490/problems/check-digitorial-permutation/description/)

You are given an integer `n`.

A number is called **digitorial** if the sum of the factorials of its digits is equal to the number itself.

Your task is to determine whether **any permutation** of `n` (including the original order) forms a digitorial number.

Return `true` if such a permutation exists. Otherwise, return `false`.

---

## 🧠 Definitions

### 🔹 Factorial
The factorial of a non-negative integer `x`, denoted as `x!`, is:
x! = x × (x - 1) × (x - 2) × ... × 1


Special case:


0! = 1

---

### 🔹 Permutation Rules

- A permutation is a rearrangement of all digits of the number.
- The permutation **must not start with zero**.
- Any arrangement that starts with zero is considered **invalid**.

---

## 🧾 Examples

---

### 🟢 Example 1

**Input:**
n = 145


**Output:**

true


**Explanation:**

145 itself is digitorial:


1! + 4! + 5!
= 1 + 24 + 120
= 145
Since at least one permutation (the original number) is digitorial, return `true`.

---

### 🟢 Example 2

**Input:**

n = 10


**Output:**

false


**Explanation:**

For 10:


1! + 0! = 1 + 1 = 2

2 ≠ 10, so it is not digitorial.

The permutation `"01"` is invalid because it starts with zero.

Since no valid permutation forms a digitorial number, return `false`.

---

## 📎 Constraints

- `1 <= n <= 10^9`

---

## 🏷️ Tags

- Mathematics
- Permutations
- Factorial
- Digit Manipulation
- Brute Force / Optimization

---

> 💡 This problem tests mathematical observation, digit manipulation, and permutation validation with constraints.
