## Problem Analysis

The problem is to create a C++ program that accepts a student's name and their score as input and then calculates and displays their grade based on the following criteria:
- If the score is between 80 and 100, the grade is 'A'.
- If the score is between 70 and 79, the grade is 'B'.
- If the score is between 60 and 69, the grade is 'C'.
- If the score is between 50 and 59, the grade is 'D'.
- If the score is less than 50, the grade is 'F'.

## Algorithm

1. Declare two variables: `score` (float) and `name` (string) to store the student's name and score.
2. Prompt the user to enter the student's name.
3. Read and store the student's name.
4. Prompt the user to enter the student's score.
5. Read and store the student's score.
6. Use conditional statements to determine the grade based on the score:
   - If `score` is between 80 and 100, set `grade` to 'A'.
   - Else if `score` is between 70 and 79, set `grade` to 'B'.
   - Else if `score` is between 60 and 69, set `grade` to 'C'.
   - Else if `score` is between 50 and 59, set `grade` to 'D'.
   - Else, set `grade` to 'F'.
7. Display the student's name, score, and grade.

## Pseudocode

```plaintext
// Declare Variables
score: float
name: string

// Accept User Inputs
output "Student Name: "
input name
output "Enter Score: "
input score

// Process score into grade
if score >= 80 and score <= 100:
    output "Student Name:", name, "Score:", score, "Grade: A"
elif score >= 70 and score <= 79:
    output "Student Name:", name, "Score:", score, "Grade: B"
elif score >= 60 and score <= 69:
    output "Student Name:", name, "Score:", score, "Grade: C"
elif score >= 50 and score <= 59:
    output "Student Name:", name, "Score:", score, "Grade: D"
elif score < 50:
    output "Student Name:", name, "Score:", score, "Grade: F"
else:
    output "Invalid"
