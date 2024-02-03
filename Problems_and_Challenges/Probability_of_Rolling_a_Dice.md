# Problem Analysis: Probability of Rolling a Dice

## Problem Statement

We want to calculate the probability of each possible outcome when rolling a standard six-sided dice. The dice has six faces numbered from 1 to 6, and we want to determine the likelihood of rolling each of these numbers.

## Algorithm

1. Initialize an array `frequency` of size 6 to store the count of each possible outcome (1 to 6). Initialize all elements of `frequency` to 0.

2. Create a variable `totalRolls` and set it to the total number of rolls you want to simulate.

3. Repeat the following steps `totalRolls` times:
   a. Generate a random number between 1 and 6 (inclusive) to simulate a dice roll.
   b. Increment the corresponding element in the `frequency` array by 1 based on the outcome of the roll.

4. Calculate the probability of each outcome by dividing the count in each element of the `frequency` array by `totalRolls`. This will give us the probability of rolling each number from 1 to 6.

5. Display the probabilities for each outcome.

## Pseudocode

```cpp
#include <iostream>
#include <cstdlib>
#include <ctime>

int main() {
    // Initialize an array to store the frequency of each outcome
    int frequency[6] = {0};

    // Set the total number of rolls
    int totalRolls = 1000; // You can change this as needed

    // Seed the random number generator
    std::srand(std::time(0));

    // Simulate dice rolls
    for (int i = 0; i < totalRolls; ++i) {
        int roll = (std::rand() % 6) + 1; // Generate a random number between 1 and 6
        frequency[roll - 1]++; // Increment the corresponding element in the array
    }

    // Calculate and display probabilities
    std::cout << "Probability of Rolling Each Number:\n";
    for (int i = 0; i < 6; ++i) {
        double probability = static_cast<double>(frequency[i]) / totalRolls;
        std::cout << "Number " << (i + 1) << ": " << probability << std::endl;
    }

    return 0;
}
