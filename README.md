# Number-Guessing-Game---Python
A simple number guessing game where the user tries to guess a randomly generated integer within a specified range. The game provides feedback on whether the guess is too high or too low and tracks the number of attempts.


# Number Guessing Game

This is a simple command-line number guessing game written in Python. The program generates a random integer between a user-defined range and challenges the user to guess the number within a limited number of attempts.

## How to Play

1. **Input the Range:** The game will first ask you to enter two numbers:
   - A lower bound (starting limit).
   - An upper bound (ending limit).

2. **Guess the Number:** You will have a limited number of chances to guess the randomly generated integer between the lower and upper bounds. The number of chances is determined by the logarithm of the range size (base 2).

3. **Feedback:** After each guess, the program will tell you if your guess is too high or too low. If you guess the correct number, you will be congratulated and the game ends.

4. **Game End:** If you exceed the number of allowed guesses, the game will reveal the correct number and end.

## How It Works

- The game calculates the maximum number of attempts using the formula `round(log2(upper - lower + 1))`, where `upper` and `lower` are the user-defined bounds.
- The random number is generated using Python's `random.randint()` function.
- The game gives feedback based on the user's input and continues until the number is guessed correctly or the attempts are exhausted.

## Example

Enter Lower bound:- 1
Enter Upper bound:- 100
You've only 7 chances to guess the integer!

Guess a number:- 50
You guessed too small!

Guess a number:- 75
You guessed too high!

Guess a number:- 63
Congratulations you did it in 3 tries!


## Requirements

- Python 3.x

## Installation

Clone the repository and run the script using Python:

```bash
git clone https://github.com/roboraees07/number-guessing-game.git
cd number-guessing-game
python guess_number.py

