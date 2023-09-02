# Problem Analysis: Compare Triplets

## Problem Statement

Alice and Bob have each created a problem for HackerRank, and these problems were rated in three categories: problem clarity, originality, and difficulty. The ratings for Alice's problem are given as a triplet `(a[0], a[1], a[2])`, and the ratings for Bob's problem are given as a triplet `(b[0], b[1], b[2])`.

Your task is to compare these ratings and determine who earned more points. You compare the ratings in each category as follows:

- If `a[i]` is greater than `b[i]`, Alice gets 1 point in that category.
- If `a[i]` is less than `b[i]`, Bob gets 1 point in that category.
- If `a[i]` is equal to `b[i]`, neither gets a point in that category.

You need to calculate the total points earned by Alice and Bob separately.

## Input

- Two arrays `a` and `b`, each containing three integers (`a[0]`, `a[1]`, `a[2]`) and (`b[0]`, `b[1]`, `b[2]`) respectively, where:
  - `1 <= a[i], b[i] <= 100` for `i` in the range `[0, 2]`.

## Output

- An array containing two integers, Alice's points and Bob's points, respectively. Alice's points should be the first integer in the array.

## Example

### Input

```plaintext
a = [5, 6, 7]
b = [3, 6, 10]
