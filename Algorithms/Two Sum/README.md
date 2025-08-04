# 🧮 LeetCode 1. Two Sum – Easy

> [🔗 View on LeetCode](https://leetcode.com/problems/two-sum)

## 📝 Problem Description

Given an array of integers `nums` and an integer `target`, return **indices of the two numbers** such that they add up to `target`.

- You may assume that each input would have **exactly one solution**.
- You may **not use the same element twice**.
- You can return the answer in **any order**.

---

## 💡 Examples

### Example 1:
Input: nums = [2,7,11,15], target = 9
Output: [0,1]

Explanation: nums[0] + nums[1] = 2 + 7 = 9

shell
Copy
Edit

### Example 2:
Input: nums = [3,2,4], target = 6
Output: [1,2]

shell
Copy
Edit

### Example 3:
Input: nums = [3,3], target = 6
Output: [0,1]

yaml
Copy
Edit

---

## 🔒 Constraints
- `2 <= nums.length <= 10⁴`
- `-10⁹ <= nums[i] <= 10⁹`
- `-10⁹ <= target <= 10⁹`
- **Only one valid answer exists**

---

## ✅ Solution – Java

```java
class Solution {
    public int[] twoSum(int[] nums, int target) {
        int[] arr = new int[2];
        for (int i = 0; i < nums.length; i++) {
            for (int j = i + 1; j < nums.length; j++) {
                if (nums[i] + nums[j] == target) {
                    arr[0] = i;
                    arr[1] = j;
                    return arr;
                }
            }
        }
        return arr; // fallback, though LeetCode guarantees one solution
    }
}
````
---
##📊 Submission Stats
✅ All 63/63 testcases passed

🕓 Runtime: 33 ms — Beats 48.66%

🧠 Memory: 44.62 MB — Beats 95.50%

📅 Submitted by: Sachin MR on Sep 16, 2024, 11:15 PM
---
## 🤝 Want to Contribute?

Found a better solution? Want to improve time/space complexity or add a different language?

✅ Create a Pull Request — I accept:

- Clean solutions in any programming language
- Optimized or faster versions of existing code
- Well-commented code or visual explanations
- Additional test cases
- Bug fixes or logic improvements

All valid contributions are welcome and you will get full credit in the commit and PR history.

Let's build a helpful LeetCode community together!

Happy Coding and Keep Solving!  
— Sachin MR
