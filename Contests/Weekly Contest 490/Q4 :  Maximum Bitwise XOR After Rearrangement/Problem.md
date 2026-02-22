# 💥 Q3. Maximum Bitwise XOR After Rearrangement

<p align="center">
  <img src="https://img.shields.io/badge/Difficulty-Medium-orange?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Category-Bit Manipulation-blue?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Topic-Greedy Strategy-green?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/String-Binary-purple?style=for-the-badge"/>
</p>

---

## 📌 [Problem Description (on LeetCode)](https://leetcode.com/contest/weekly-contest-490/problems/maximum-bitwise-xor-after-rearrangement/submissions/1927006120/)

You are given two binary strings `s` and `t`, each of length `n`.

- You may **rearrange the characters of `t` in any order**.
- The string `s` must remain unchanged.

Your task is to return a binary string of length `n` representing the **maximum integer value** obtainable by taking the **bitwise XOR** of:
s XOR rearranged(t)


---

## 🧠 Key Observations

- Rearrangement is allowed **only for `t`**.
- The result must be a **binary string**.
- The objective is to maximize the resulting integer value.
- Larger binary values are determined by higher bits (leftmost bits first).

---

## 🧾 Examples

---

### 🟢 Example 1

**Input:**

s = "101"
t = "011"
**Output:**

"110"


**Explanation:**

One optimal rearrangement of `t` is:


"011"


Bitwise XOR:

101
XOR 011

110
"110" is the maximum possible result.

---

### 🟢 Example 2

**Input:**

s = "0110"
t = "1110"


**Output:**

"1101"


**Explanation:**

One optimal rearrangement of `t` is:
"1011"


Bitwise XOR:

0110
XOR 1011

1101


"1101" is the maximum possible result.

---

### 🟢 Example 3

**Input:**

s = "0101"
t = "1001"
**Output:**

"1111"


**Explanation:**

One optimal rearrangement of `t` is:


"1010"


Bitwise XOR:

0101
XOR 1010

1111

"1111" is the maximum possible result.

---

## 📎 Constraints

- `1 <= n == s.length == t.length <= 2 × 10^5`
- `s[i]` and `t[i]` are either `'0'` or `'1'`.

---

## 🏷️ Tags

- Bit Manipulation
- Greedy
- Strings
- Rearrangement
- Optimization

---

> 💡 This problem tests greedy thinking and understanding of how binary XOR contributes to maximizing integer values.
