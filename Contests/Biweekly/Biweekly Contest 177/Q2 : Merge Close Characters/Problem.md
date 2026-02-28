# 🔗 [Q2. Merge Close Characters](https://leetcode.com/contest/biweekly-contest-177/problems/merge-close-characters/)

<p align="center">
  <img src="https://img.shields.io/badge/Platform-LeetCode-orange?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Difficulty-Medium-yellow?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Category-Strings-blue?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Topic-Simulation%20%26%20Two%20Pointers-purple?style=for-the-badge"/>
</p>

---

## 📌 Problem Statement

You are given:

- A string `s` consisting of lowercase English letters  
- An integer `k`

---

## 🔍 Definition

Two equal characters in the current string `s` are considered **close** if:


distance between their indices ≤ k


---

## 🔄 Merge Rule

- When two equal characters are close,  
  the **right one merges into the left one**.
- Merges happen **one at a time**.
- After each merge, the string updates.
- Continue until no more merges are possible.

---

## ⚠️ Merge Priority

If multiple merges are possible:

1. Choose the pair with the **smallest left index**.
2. If multiple pairs share the same left index,  
   choose the pair with the **smallest right index**.

---

## 🎯 Return

Return the final string after performing all valid merges.

---

## 🧾 Examples

### 🟢 Example 1

**Input**

s = "abca", k = 3


**Output**

"abc"


**Explanation**

- Characters `'a'` at indices `0` and `3`  
- Distance = `3 - 0 = 3 ≤ k`  

Merge right `'a'` into left `'a'`:


"abc"


No further merges possible.

---

### 🟢 Example 2

**Input**

s = "aabca", k = 2


**Output**

"abca"


**Explanation**

- `'a'` at indices `0` and `1` → merge  
- String becomes `"abca"`

Now `'a'` at indices `0` and `3`  
Distance = `3`, which is greater than `k`  

No further merges.

---

### 🟢 Example 3

**Input**

s = "yybyzybz", k = 2


**Output**

"ybzybz"


**Explanation**

1. `'y'` at indices `0` and `1` → merge → `"ybyzybz"`
2. `'y'` at indices `0` and `2` → merge → `"ybzybz"`

No more valid merges remain.

---

## 📎 Constraints

- `1 ≤ s.length ≤ 100`
- `1 ≤ k ≤ s.length`
- `s` contains only lowercase English letters

---

## 🏷️ Tags

- Strings
- Simulation
- Two Pointers
- Greedy Selection
- Implementation

---

> 💡 This problem tests careful simulation with priority-based merging and dynamic string updates.
