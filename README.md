# LeetCode-Question-Number-16

You are given an integer array nums of length n and an integer target.  Find three integers at distinct indices in nums such that the sum is closest to target.  Return the sum of the three integers.  You may assume that each input would have exactly one solution.


# This is the result of the Solution

<img width="1917" height="911" alt="image" src="https://github.com/user-attachments/assets/cbac1716-f246-4e54-9a10-479ca0397d5e" />


# Work Flow

1. Sort the Array: Sort the input array in ascending order and initialize `closest` with the sum of the first three elements.

2. Fix the First Element: Iterate through the array, selecting the first element and skipping duplicates to avoid unnecessary calculations.

3. Apply Pruning: Calculate the minimum and maximum possible sums for the current element. Update `closest` if either sum is nearer to the target, and skip unnecessary iterations.

4. Use Two Pointers: Initialize the left pointer to `i + 1` and the right pointer to the last index. Calculate the sum of the three selected elements.

5. Update the Closest Sum: If the current sum is closer to the target than `closest`, update it. If the sum equals the target, return the target immediately. Otherwise, move the left pointer right if the sum is smaller or the right pointer left if it is larger.

6. Return the Result: Continue until all possible combinations have been checked, then return `closest`, the sum nearest to the target.
