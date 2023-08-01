## Kaun Banega Crorepati - Python Game Documentation

This is a Python implementation of the popular TV show "Kaun Banega Crorepati" (Who Wants to Be a Millionaire). In this game, the player answers multiple-choice questions and wins cash prizes for each correct answer. The game provides lifelines to the player to help them with difficult questions. The player can use four lifelines: Audience Poll, Fifty-Fifty, Double Dip, and Flip the Question.

### Requirements

- Python 3.x
- matplotlib library (`pip install matplotlib`)
- pandas library (`pip install pandas`)

### How to Play

1. Run the Python script in your terminal or any Python environment.
2. The game will welcome you and ask for your name.
3. The game will present you with multiple-choice questions one by one.
4. Choose the correct option by entering the option number (1, 2, 3, or 4).
5. You can use lifelines by pressing '9':
   - Audience Poll: See the audience's percentage distribution for each option.
   - Fifty-Fifty: Remove two incorrect options, leaving only one correct and one incorrect option.
   - Double Dip: Get two chances to answer the question.
   - Flip the Question: Skip the current question and get a new one.
6. You can quit the game anytime by pressing '0'.
7. The game will display your winning amount based on the number of correct answers.

### Code Explanation

The code begins with importing the required libraries and setting up the questions, options, and correct answers. The game proceeds in a while loop, asking questions one by one and offering lifelines if needed. The game keeps track of the number of correct answers and calculates the total winning amount. The game continues until the player quits or answers all 16 questions correctly.

### Function Definitions

1. `lifeline(ran, opts, op)`: This function allows the player to use lifelines and calls the respective lifeline functions.
2. `audience(ran, opts)`: This function displays the audience poll for the current question and prompts the player to answer or use another lifeline.
3. `fifty(ran, op)`: This function implements the Fifty-Fifty lifeline by removing two incorrect options.
4. `doubleDip(ran)`: This function implements the Double Dip lifeline, which allows the player to answer a question twice.
5. `flip()`: This function represents the Flip the Question lifeline and is not implemented in the current code.
6. `amount(correct_ans)`: This function calculates and prints the winning amount based on the number of correct answers.

### Note

The code provided is a basic implementation of the game and may have limitations or potential improvements. You can further enhance it by adding more questions, adding a timer for each question, displaying graphics for the lifelines, or creating a GUI for a better user experience.
