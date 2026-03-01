# 🎮 Q1. Find the Score Difference in a Game

<p align="center">
  <img src="https://img.shields.io/badge/Difficulty-Medium-orange?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Category-Simulation-blue?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Data%20Structure-Array-green?style=for-the-badge"/>
</p>

---

## [📌 Problem Description (on LeetCode)](https://leetcode.com/contest/weekly-contest-490/problems/find-the-score-difference-in-a-game/description/)

You are given an integer array `nums`, where:

- `nums[i]` represents the points scored in the **i-th game**.
- There are exactly **two players**:
  - The **first player** (initially active)
  - The **second player** (initially inactive)

The games are processed sequentially from index `0` to `n - 1`.

---

## 🎯 Game Rules

For each game `i`, apply the following rules **in order**:

1. If `nums[i]` is **odd**, the active and inactive players swap roles.
2. In every **6th game** (i.e., game indices `5, 11, 17, ...`), the active and inactive players swap roles.
3. The **active player** plays the i-th game and gains `nums[i]` points.

---

## 🧮 Return

Return the **score difference**, defined as:

First Player’s Total Score − Second Player’s Total Score

---

## 🧾 Examples

### Example 1

**Input:**
nums = [1, 2, 3]


**Output:**

0

**Explanation:**

- Game 0: Points are odd → swap → second player gains 1  
- Game 1: No swap → second player gains 2  
- Game 2: Points are odd → swap → first player gains 3  

Final Scores:
- First Player = 3  
- Second Player = 3  

Score Difference = `3 - 3 = 0`

---

### Example 2

**Input:**
nums = [2, 4, 2, 1, 2, 1]


**Output:**

4

**Explanation:**

- Games 0–2: First player gains `2 + 4 + 2 = 8`
- Game 3: Points are odd → swap → second player gains 1
- Game 4: No swap → second player gains 2
- Game 5:
  - Points are odd → swap
  - 6th game → swap again
  - Second player gains 1

Final Scores:
- First Player = 8  
- Second Player = 4  

Score Difference = `8 - 4 = 4`

---

### Example 3

**Input:**
nums = [1]


**Output:**

-1


**Explanation:**

- Game 0: Points are odd → swap → second player gains 1  

Final Scores:
- First Player = 0  
- Second Player = 1  

Score Difference = `0 - 1 = -1`

---

## 📎 Constraints

- `1 <= nums.length <= 1000`
- `1 <= nums[i] <= 1000`

---

## 🏷️ Tags

- Array
- Simulation
- Implementation
- State Tracking

---

> 💡 This problem tests careful rule interpretation and sequential simulation logic.
