# Multiple-Choice Quiz Game Instructions

## Instructions

### 1. Set Up Your Data

- **Data Structure:** Use a list of dictionaries to store each question along with its options and the correct answer. This is given to you in the `questions.py` file.

### 2. Load the Questions

- **Import The Questions:** Import the questions from `questions.py`.
- **Assign Data:** Assign the provided list of dictionaries to a variable in your script.

### 3. Initialize the Score

- **Variable:** Create a variable `score` and set it to `0`.

### 4. Iterate Through the Questions

- **Loop:** Use a `for` loop to iterate over each question in the dataset.
- **Steps Inside the Loop:**

  **Display the Question and Options:**

  - Print the question.
  - Display the multiple-choice options with corresponding letters (e.g., A, B, C, D).

  **Get User Input:**

  - Prompt the user to enter the letter corresponding to their answer.
  - Ensure the input is case-insensitive.

  **Validate Input:**

  - Check if the input is one of the valid option letters.
  - If not, prompt the user again until a valid input is received.

  **Check the Answer:**

  - Compare the user's input with the correct answer.
  - **If correct:**
    - Increment the `score` and provide positive feedback.
  - **If incorrect:**
    - Provide the correct answer. and decrement the score.

### 5. Display the Final Score

- **After the Loop:** Print the user's total score out of the total number of questions.
- **Ending the game** End the game wither when a user reached a score of 10 or when he got a negative score.
- **Optional:** Provide a percentage score or a grade based on the total score.
- **Optional:** prompt the user to decide on the game rules such as the total answers he needs to get right or use it as a timed test.

### 6. Optional Enhancements

- **Randomization: (Optional)**

  - Shuffle the question order using the `random` module.
  - Shuffle the options for each question.

- **Timing: (Optional)**

  - Add a timer to limit how long a user can take to answer each question.

- **Scoring System:**

  - Deduct points for incorrect answers.
  - Award bonus points for quick responses.

- **Feedback:**
  - After each question, provide an explanation for the correct answer.
