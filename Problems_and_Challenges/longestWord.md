## Algorithm: Find the Longest Word

1. **Input:** Receive a string as input.

2. **Output:** Return the longest word in the input string.

3. **Initialize** a variable `longestWord` to store the longest word and set it to an empty string initially.

4. **Split** the input string into an array of words. Use the `split` method with a space as the separator to separate words. Let's call this array `words`.

5. **Iterate through words:**

   - Create a loop to go through each word in the `words` array.
   - For each word, check its length using the `length` property.

6. **Compare word lengths:**

   - If the length of the current word is greater than the length of `longestWord`, update `longestWord` with the current word.

7. **Continue** this process for all words in the array.

8. **Result:** After the loop, the variable `longestWord` will store the longest word.

9. **Return** `longestWord` as the result.

### Example:

```javascript
function findLongestWord(str) {
  // Initialize the longest word
  let longestWord = "";

  // Split the string into an array of words
  const words = str.split(" ");

  // Iterate through the words
  for (const word of words) {
    // Check if the current word is longer than the longest word
    if (word.length > longestWord.length) {
      longestWord = word;
    }
  }

  // Return the longest word
  return longestWord;
}

const testString = "The quick brown fox jumped over the lazy dog";
console.log(findLongestWord(testString)); // Should return "jumped"
```
