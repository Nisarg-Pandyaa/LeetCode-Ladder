# ✂️ [Q1. Trim Trailing Vowels](https://leetcode.com/contest/weekly-contest-491/problems/trim-trailing-vowels/description/)

<p align="center">
  <img src="https://img.shields.io/badge/Platform-LeetCode-orange?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Difficulty-Easy-green?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Category-Strings-blue?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Topic-Two%20Pointers%20%26%20Simulation-purple?style=for-the-badge"/>
</p>

---

## 📌 Problem Statement

You are given a string `s` consisting of lowercase English letters.

Return the string obtained after **removing all trailing vowels** from `s`.

---

## 🔤 Vowels

The vowels are:


a, e, i, o, u


Only trailing vowels (at the end of the string) should be removed.

---

## 🎯 Task

- Remove consecutive vowels from the end of the string.
- Stop when a consonant is encountered.
- Return the resulting string.

---

## 🧾 Examples

### 🟢 Example 1

**Input**

s = "idea"


**Output**

"id"


**Explanation**

Trailing vowels `"e"` and `"a"` are removed.

---

### 🟢 Example 2

**Input**

s = "day"


**Output**

"day"


**Explanation**

The string does not end with a vowel, so no changes are made.

---

### 🟢 Example 3

**Input**

s = "aeiou"


**Output**

""


**Explanation**

All characters are trailing vowels, so the entire string is removed.

---

## 📎 Constraints

- `1 ≤ s.length ≤ 100`
- `s` contains only lowercase English letters

---

## 🏷️ Tags

- Strings
- Two Pointers
- Simulation
- Implementation

---

> 💡 This problem tests simple reverse traversal and vowel checking logic.
