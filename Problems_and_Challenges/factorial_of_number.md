# Factorial Calculation Problem

## Problem Description

Given a positive integer `n`, calculate and return its factorial.

## Problem Analysis

- The problem requires calculating the factorial of a given positive integer `n`.

- The algorithm uses a loop to perform the multiplication iteratively.

- The algorithm handles the edge case where `n` is less than 0 by displaying an error message.

- The time complexity of this algorithm is O(n) because it performs a loop that iterates `n` times to calculate the factorial.

- The space complexity is O(1) because it uses a fixed amount of memory to store the variables `n`, `factorial`, and `i`.

- This problem is commonly used as an introductory exercise to practice loops and conditional statements in programming.

### Input

- A positive integer `n` (1 ≤ n ≤ 20).

### Output

- The factorial of `n`.

## Algorithm

1. Start.

2. Read the input integer `n`.

3. Initialize a variable `factorial` to 1. This will be used to store the result.

4. Check if `n` is less than 0.

   - If true, print an error message ("Factorial is not defined for negative numbers.") and stop.
   - If false, proceed to the next step.

5. If `n` is 0, set `factorial` to 1 and go to step 8.

6. If `n` is greater than 0, do the following:

   - Initialize a loop variable `i` to 1.
   - Start a loop that iterates while `i` is less than or equal to `n`.
     - Inside the loop, multiply `factorial` by `i` and assign the result back to `factorial`.
     - Increment `i` by 1.
   - End the loop.

7. Print the value of `factorial` as the result.

8. Stop.
