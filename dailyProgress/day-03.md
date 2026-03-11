# Day 3 — DSA Journal
**Date:** 11-03-2026  
**Streak:** 3 day 🔥

---

## Problems Solved

| # | Problem | Difficulty | Pattern | Status |
|---|---------|------------|---------|--------|
| 1 | [Merge Sorted Array](https://leetcode.com/problems/merge-sorted-array/) | 🟢 Easy | Two Pointers | ✅ Solved |
| 2 | [Majority Element](https://leetcode.com/problems/majority-element/) | 🟢 Easy | Boyer Moore | ✅ Solved |
| 3 | [Reverse a String](https://leetcode.com/problems/reverse-string/) | 🟢 Easy | Two Pointers | ✅ Solved |

---

## #1 Merge Sorted Array problem

Pattern: Two Pointers (Three Pointers)
Time Complexity: O(n)
Space Complexity: O(1)
Key Insight: Start merging from end instead of start
Mistake: Was trying to merge from start

## #2 Majority Element problem

Pattern: Boyer Moore voting algorithm
Time Complexity: O(n)
Space Complexity: O(1)
Key Insight: cancel out the majority votes
Mistake: couldn’t think of this approach

## #3 Reverse a String problem

Pattern: Two Pointers
Time Complexity: O(n)
Space Complexity: O(1)
Key Insight: simple swap from start and end
Mistake: none

---

## Key Insight of the Day
> *Start merging from the end instead of the start when dealing with merging sorted data into pre-allocated arrays to avoid overwriting elements.* 

---

## Pattern Focus Today
**Pattern:** Two Pointers & Boyer Moore  
**When to reach for it:** When dealing with reversing strings, merging arrays, or finding majority elements.
**Template for Two Pointers:**
```java
int left = 0;
int right = arr.length - 1;
while (left < right) {
    // Process, compare, or swap
    left++;
    right--;
}
```

---

## Mistakes & Fixes
- **Mistake:** Was trying to merge from the start.
- **Fix:** Modifying elements from the start of an array where data is already present requires shifting; start from the end instead where there is empty space.
- **Mistake:** Couldn’t think of Boyer Moore approach for majority element.
- **Fix:** Remember the cancel-out logic for elements appearing more than n/2 times.

---

## Time Spent
- Total: ~3 Hr
- Problem 1: 1 Hr 15 min (First try was brute force - merging from start - O(n))
- Problem 2: 1 Hr 15 min (First try was brute force - using hashmap - O(n))
- Problem 3: 15 min