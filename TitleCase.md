# Problem Analysis and Algorithm: Title Case a Sentence

## Problem Description

The task is to write a function that takes a sentence as input and returns the sentence with the first letter of each word capitalized and the rest of the letters in lowercase. However, articles (a, an, the), coordinating conjunctions (and, but, for, nor, or, so, yet), and prepositions (in, of, on, with) should remain in lowercase, unless they are the first word in the sentence.

## Problem Analysis

To solve this problem, we need to perform the following steps:

1. Split the input sentence into an array of words.
2. Loop through each word in the array:
   - If the word is the first word in the sentence or is not one of the exceptions (articles, conjunctions, or prepositions), capitalize the first letter and make the rest of the word lowercase.
   - If the word is not the first word in the sentence and is one of the exceptions, keep it in lowercase.
3. Join the modified words back into a sentence.
4. Return the title-cased sentence as the result.

## Algorithm

1. Create an array called `exceptions` that contains the words "a," "an," "the," "and," "but," "for," "nor," "or," "so," "yet," "in," "of," "on," and "with."

2. Define the `titleCase` function that takes a sentence as input.

3. Split the input sentence into an array of words using the space character as the separator. Store the array in a variable called `words`.

4. Create a `for` loop to iterate through each word in the `words` array. Use an index variable `i` to keep track of the current word.

5. For each word in the array:

   - Check if it is the first word in the sentence (i.e., `i === 0`) or if it is not one of the exceptions. If so, capitalize the first letter of the word using `.charAt(0).toUpperCase()` and make the rest of the word lowercase using `.slice(1).toLowerCase()`.
   - If the word is not the first word in the sentence and is one of the exceptions, keep it in lowercase.

6. Join the modified words back into a sentence using the space character as the separator. This can be done using the `.join(" ")` method.

7. Return the title-cased sentence as the result.

## Example

```javascript
function titleCase(sentence) {
  const exceptions = [
    "a",
    "an",
    "the",
    "and",
    "but",
    "for",
    "nor",
    "or",
    "so",
    "yet",
    "in",
    "of",
    "on",
    "with",
  ];

  const words = sentence.split(" ");

  for (let i = 0; i < words.length; i++) {
    const word = words[i];
    if (i === 0 || !exceptions.includes(word.toLowerCase())) {
      words[i] = word.charAt(0).toUpperCase() + word.slice(1).toLowerCase();
    } else {
      words[i] = word.toLowerCase();
    }
  }

  return words.join(" ");
}

const testSentence = "the quick brown fox jumps over the lazy dog";

console.log(titleCase(testSentence)); // Should return "The Quick Brown Fox Jumps Over the Lazy Dog "
```
