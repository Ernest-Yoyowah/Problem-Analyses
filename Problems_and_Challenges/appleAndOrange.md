## Problem Analysis

We are given the starting point `s` and ending point `t` of Sam's house, the locations of the apple tree `a` and the orange tree `b`, and the distances at which each apple and orange falls from their respective trees. The problem requires us to determine how many apples and oranges will fall on Sam's house (in the inclusive range `[s, t]`).

## Algorithm

1. Initialize two variables `appleCount` and `orangeCount` to zero. These variables will be used to keep track of the number of apples and oranges that fall on Sam's house.

2. For each apple distance in the array `apples`, calculate the absolute position where the apple will fall by adding the apple distance to the apple tree's location `a`. If this position is within the range `[s, t]`, increment `appleCount`.

3. For each orange distance in the array `oranges`, calculate the absolute position where the orange will fall by adding the orange distance to the orange tree's location `b`. If this position is within the range `[s, t]`, increment `orangeCount`.

4. Print the values of `appleCount` and `orangeCount` on separate lines.

## Pseudocode

```plaintext
function countApplesAndOranges(s, t, a, b, apples, oranges):
    appleCount = 0
    orangeCount = 0

    for each appleDistance in apples:
        applePosition = a + appleDistance
        if s <= applePosition <= t:
            increment appleCount

    for each orangeDistance in oranges:
        orangePosition = b + orangeDistance
        if s <= orangePosition <= t:
            increment orangeCount

    print appleCount
    print orangeCount
```
