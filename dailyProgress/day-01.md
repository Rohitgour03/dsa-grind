# Day 1 — DSA Journal
**Date:** 09-03-2026  
**Streak:** 1 day 🔥

---

## Problems Solved

| # | Problem | Difficulty | Pattern | Status |
|---|---------|------------|---------|--------|
| 1 | [Two Sum](https://leetcode.com/problems/two-sum/) | 🟢 Easy | HashMap Lookup | ✅ Solved |

---

## #1 Two Sum problem

Pattern: Hashmap lookup for complement
Time Complexity: O(n)
Space Complexity: O(n)
Key Insight: HashMap is the go-to for pair-finding
Mistake: Did not think of Hashmap first

---

## Key Insight of the Day
> *e.g. "Most array problems that ask for pairs/complements → think HashMap O(1) lookup, not nested loops O(n²)"*

---

## Pattern Focus Today
**Pattern:** HashMap Lookup  
**When to reach for it:** When you need to check existence or find complement in O(1)  
**Template:**
```java
Map<Integer, Integer> map = new HashMap<>();
for (int i = 0; i < nums.length; i++) {
    int complement = target - nums[i];
    if (map.containsKey(complement)) return new int[]{map.get(complement), i};
    map.put(nums[i], i);
}
```

---

## Mistakes & Fixes
- **Mistake:** Tried brute force O(n²) first, didn't think HashMap is the go-to for pair-finding
- **Fix:** Ask yourself — "do I need to look up something I've already seen?" → HashMap

---

## Time Spent
- Total: ~1 Hr
- Problem 1: 1 Hr (First try was brute force - finding each pair to check if sum equals target - O(n²))