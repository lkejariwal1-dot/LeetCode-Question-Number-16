# LeetCode-Question-Number-16
You are given an integer array nums of length n and an integer target.  Find three integers at distinct indices in nums such that the sum is closest to target.  Return the sum of the three integers.  You may assume that each input would have exactly one solution.

# This is the result of the Solution
<img width="1917" height="911" alt="image" src="https://github.com/user-attachments/assets/cbac1716-f246-4e54-9a10-479ca0397d5e" />

# Work Flow
1. We first fix a index in the list.
2. Then apply the 2-pointer method.
3. First pointer will point at the index+1 value.
4. Last pointer will point at the last index of list.
5. If the sum of these 3 index is less than the target, pointer 1 will shift ahead by 1, If the sum is greater than the target, last pointer will shift behind by 1, If the sum is equal to target, append the list in the result.
6. After iterating the whole list return the result.
