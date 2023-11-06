**Problem Analysis:**

- Maria's goal is to monitor her basketball performance during each season.
- She wants to determine how many times she breaks her records for the most and least points scored.
- Records are considered broken when the current game's score surpasses the previous maximum or minimum score.

**Algorithm:**

1. Initialize `min_score` and `max_score` with the score from the first game.
2. Initialize `min_record_count` and `max_record_count` as 0.
3. Iterate through the game scores, starting from the second game:
   - If the current score is less than `min_score`, update `min_score` and increment `min_record_count`.
   - If the current score is greater than `max_score`, update `max_score` and increment `max_record_count`.
4. Return the result as an array: `[max_record_count, min_record_count]`.
