# 2i-Code-Challenge

I have been give this task from 2i as a code challenge.

In a language of your choice, write a solution for the game that satisfies the following criteria:

    Generates a random number.

    Takes in a guess.

    Returns a string with the guess and whether that guess is lower or higher than the random number. E.g., “You answered 9. The correct answer is higher.”

    If the guess matches the random number, then return a string which confirms this. E.g., “You answered 9. This is the correct answer!”


This challenge (deliberately) does not give any guidance about ranges, input validation, presentation etc., so you are also required to explain any assumptions that you have made. This can be done using comments in the code or in a readme file, or both.

#### Overview

This is a simple number guessing game where the player has to guess a random number between 1 and 100 within 10 tries. The game gives feedback on whether the guess was too high, too low, or correct

#### How to Play
1. Enter a number between 1 and 100 in the input field.
2. Click the "Submit Guess" button.
3. After each guess, you'll get feedback indication if your guess was correct, too high, or too low
4. You have 10 attempts to guess the correct number. If you run out of attempts or guess correct, the game will end
5. Once the game ends, a "Play Again" button will appear to start a new game



First test of code. The guessing part of the code works but when I get a 'Game Over' message the game doesn't reset

Figured out problem "submitButton.disable = true" was written as "submitButton.disabled = true"

Explanation