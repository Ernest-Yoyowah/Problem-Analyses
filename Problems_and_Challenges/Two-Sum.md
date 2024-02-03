# Problem Analysis: Two Sum

## Problem Statement
Given an array of integers `nums` and an integer `target`, you need to return indices of the two numbers such that they add up to the `target`.

You may assume that each input would have exactly one solution, and you may not use the same element twice.

## Input
- `nums`: An array of integers representing the numbers.
- `target`: An integer representing the target sum.

## Output
- An array of two integers representing the indices of the two numbers that add up to the target.

## Approach
The problem requires finding two numbers in the `nums` array that sum up to the given `target`. To solve this efficiently, we can use a hash map to store the indices of numbers we have encountered so far. We'll iterate through the array, and for each number, we'll calculate its complement (the value needed to achieve the target sum) and check if it exists in the hash map. If it does, we've found the solution; otherwise, we'll add the current number and its index to the hash map.

## Pseudocode
```plaintext
function twoSum(nums, target):
    numIndices = new Map()   // Map to store {number: index} pairs

    for i = 0 to nums.length - 1:
        num = nums[i]
        complement = target - num

        if numIndices.has(complement):
            return [numIndices.get(complement), i]

        numIndices.set(num, i)

    return []
