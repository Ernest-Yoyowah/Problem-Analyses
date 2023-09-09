# Problem Analysis

You have been given a problem to swap the values of two integer variables `a` and `b`
. This is a common algorithm for swapping the values of two variables.

# Algorithm

1. **Initialize** two integer variables `a` and `b` with the values `1` and `2`, respectively.
2. **Create** an integer variable `temp` and initialize it to `0`. This variable will be used to temporarily store one of the values during the swap.
3. **Swap** the values of `a` and `b` using the `temp` variable:
   - Assign the value of `a` to `temp`.
   - Assign the value of `b` to `a`.
   - Assign the value of `temp` (which was the original value of `a`) to `b`.
4. **Print** the values of `a` and `b` after the swap.

# Pseudocode

```plaintext
// Initialize variables
a = 1
b = 2
temp = 0

// Swap Variables
temp = a
a = b
b = temp

// Print the swapped values
Print "The value of a is " + a + " and the value of b is " + b
