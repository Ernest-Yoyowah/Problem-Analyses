# Staircase Pattern Problem

## Problem Analysis

You are given an integer `n` and tasked with printing a staircase pattern with `n` rows. The pattern consists of spaces and hashtags ('#'). Each row has an indentation on the left side, with the number of spaces decreasing from top to bottom, while the number of hashtags increases. The goal is to create a staircase-like pattern.

**Input**

- An integer `n` (1 <= n <= 100), representing the number of rows in the staircase pattern.

**Output**

- Print the staircase pattern with `n` rows to the console.

## Algorithm

1. Define a function `staircase(n)` that takes an integer `n` as a parameter.

2. Initialize a loop that iterates through each row of the staircase pattern:

   - Start the loop with `i = 1` and continue until `i` is less than or equal to `n`.

3. For each row, calculate the number of spaces and hashtags to print:

   - Calculate `spaces` as a string of spaces with a length of `n - i`. This creates left-side indentation for the row.
   - Calculate `hashtags` as a string of `i` hashtags, representing the increasing number of hashtags in the row.

4. Concatenate the `spaces` and `hashtags` strings and print the result to the console using `console.log`.

5. After completing the loop, the function will have printed the entire staircase pattern.

6. To test the function, call it with a specific value of `n`, adjusting the value of `n` to create different-sized staircase patterns.

Here is the algorithm implemented in JavaScript:

```javascript
function staircase(n) {
  for (let i = 1; i <= n; i++) {
    const spaces = " ".repeat(n - i);
    const hashtags = "#".repeat(i);
    console.log(spaces + hashtags);
  }
}
```
