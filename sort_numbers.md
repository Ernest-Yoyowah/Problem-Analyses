# Problem Analysis

We need to create a program that takes 5 numbers as input from the user and sorts them in ascending order.

## Algorithm

1. **Start**
2. Initialize an array of `numbers` of size 5 to store the input numbers.
3. **Input:** Ask the user to enter 5 numbers one by one and store them in the `numbers` array.
4. **Sorting:** Use the bubble sort algorithm to sort the `numbers` array in ascending order.
   - Iterate through the array from 0 to 3 (i.e., for `i` from 0 to 3):
     - For each iteration of `i`, iterate through the array from 0 to 3 - `i` (i.e., for `j` from 0 to 3 - `i`):
       - If `numbers[j]` is greater than `numbers[j + 1]`, swap `numbers[j]` and `numbers[j + 1]`.
   - Repeat the above steps until the array is sorted.
5. **Output:** Print the sorted `numbers` array.
6. **End**

## Pseudocode

```plaintext
Start

Initialize an integer array numbers[5]

For i = 0 to 4:
    Input: Prompt the user to enter a number and store it in numbers[i]

For i = 0 to 3:
    For j = 0 to 3 - i:
        If numbers[j] > numbers[j + 1]:
            Swap numbers[j] and numbers[j + 1]

Output: Print "Numbers in ascending order: "
For i = 0 to 4:
    Print numbers[i], " "

End
```
