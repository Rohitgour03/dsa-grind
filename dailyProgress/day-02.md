# Day 2 — DSA Journal
**Date:** 10-03-2026  
**Streak:** 2 day 🔥

---

## Problems Solved

| # | Problem | Difficulty | Pattern | Status |
|---|---------|------------|---------|--------|
| 1 | [Best Time to Buy and Sell Stock](https://leetcode.com/problems/best-time-to-buy-and-sell-stock/) | 🟢 Easy | One Pass | ✅ Solved |
| 2 | [Remove duplicates from array](https://leetcode.com/problems/remove-duplicates-from-sorted-array/) | 🟢 Easy | Two Pointers | ✅ Solved |
| 3 | [Rotate Array](https://leetcode.com/problems/rotate-array/) | 🟢 Easy | Reverse | ✅ Solved |

---

## #1 Best Time to Buy and Sell Stock problem

Pattern: One Pass
Time Complexity: O(n)
Space Complexity: O(1)
Key Insight: Greedy pointer maintaining min element seen so far while iterating & having max profit so far
Mistake: calculated the minimum first in one iteration and then max in another iteration - O(2n)

## #2 Remove duplicates from array problem

Pattern: Two Pointers
Time Complexity: O(n)
Space Complexity: O(1)
Key Insight: Use two pointers - one for the current element to replace and one for the next unique element
Mistake: focussed on shifting the numbers which was irrelevant

## #3 Rotate Array problem

Pattern: Reverse
Time Complexity: O(n)
Space Complexity: O(1)
Key Insight: Reversing the array in parts can help in rotating the array
Mistake: Did not think of reversing instead was focusing on rotating/shifting

---

## Key Insight of the Day
> *e.g. Careful use of two pointers can help in solving array problems in O(n) time complexity with O(1) space complexity* 

---

## Pattern Focus Today
**Pattern:** Two Pointers  
**When to reach for it:** When you need to modify the array in-place or when you need to find pairs/triplets/etc in an array
**Template:**
```java
int left = 0;
int right = nums.length - 1;
while (left < right) {
    if (nums[left] + nums[right] == target) {
        return new int[]{left, right};
    } else if (nums[left] + nums[right] < target) {
        left++;
    } else {
        right--;
    }
}
```

---

## Mistakes & Fixes
- **Mistake:** Shifting the numbers instead of using two pointers
- **Fix:** Ask yourself — "do I need to modify the array in-place or when you need to find pairs/triplets/etc in an array?" → Two Pointers

---

## Time Spent
- Total: ~3 Hr
- Problem 1: 1 Hr (First try was brute force - find minimum in one iteration and max in another iteration after the minimum find earlier & then take differece - O(2n))
- Problem 2: 1 Hr (First try was brute force - shifting the numbers - O(n))
- Problem 3: 1 Hr (First try was brute force - shifting the numbers in array - O(n))