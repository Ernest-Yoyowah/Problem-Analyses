# Beautiful Days at the Movies

## Problem Analysis

The task is to determine the number of beautiful days within a given range \([i, j]\) where a day is considered beautiful if the absolute difference between the day and its reverse is evenly divisible by a given integer \(k\).

### Input

- \(i\): Starting day of the range.
- \(j\): Ending day of the range.
- \(k\): An integer.

### Output

- The number of beautiful days in the range \([i, j]\).

## Algorithm

1. Initialize a variable `beautifulDayCount` to 0 to keep track of the number of beautiful days.
2. Iterate through each day in the range \([i, j]\).
   - Convert the day to a string.
   - Reverse the string.
   - Convert the reversed string back to an integer.
   - Calculate the absolute difference between the original day and its reverse.
   - Check if the absolute difference is evenly divisible by \(k\).
     - If true, increment `beautifulDayCount`.
3. Return the final count of beautiful days.

## Pseudocode

`function beautifulDays(i, j, k):
    beautifulDayCount = 0
    for day in range(i, j + 1):
        reversedDay = parseInt(reverseString(day.toString()), 10)
        absoluteDifference = abs(day - reversedDay)
        if absoluteDifference % k == 0:
            beautifulDayCount++
    return beautifulDayCount`
