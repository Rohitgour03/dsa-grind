# Day N — DSA Journal
**Date:** YYYY-MM-DD  
**Streak:** N 🔥

---

## Problems Solved

| # | Problem | Difficulty | Pattern | Status |
|---|---------|------------|---------|--------|
| 1 | [Two Sum](https://leetcode.com/problems/two-sum/) | 🟢 Easy | HashMap Lookup | ✅ Solved |
| 2 | [Best Time to Buy Stock](https://leetcode.com/problems/best-time-to-buy-and-sell-stock/) | 🟢 Easy | Sliding Window | ✅ Solved |

---

## #1 Two Sum problem

Pattern: pattern in the problem
Time Complexity:
Space Complexity:
Key Insight:
Mistake:

## #2 Best time to buy and sell stock

Pattern: pattern in the problem
Time Complexity:
Space Complexity:
Key Insight:
Mistake:

## Key Insight of the Day
> One-liner that captures today's "aha moment" — this is what you post on socials.

*e.g. "Most array problems that ask for pairs/complements → think HashMap O(1) lookup, not nested loops O(n²)"*

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
- **Mistake:** Tried brute force O(n²) first, forgot HashMap is the go-to for pair-finding
- **Fix:** Ask yourself — "do I need to look up something I've already seen?" → HashMap

---

## Time Spent
- Total: ~45 min
- Problem 1: 20 min (struggled with off-by-one in index return)
- Problem 2: 25 min (clean solve)