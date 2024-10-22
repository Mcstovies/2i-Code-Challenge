## 2i-Code-Challenge

I have been give this task from 2i as a code challenge.

In a language of your choice, write a solution for the game that satisfies the following criteria:

    Generates a random number.

    Takes in a guess.

    Returns a string with the guess and whether that guess is lower or higher than the random number. E.g., “You answered 9. The correct answer is higher.”

    If the guess matches the random number, then return a string which confirms this. E.g., “You answered 9. This is the correct answer!”


This challenge (deliberately) does not give any guidance about ranges, input validation, presentation etc., so you are also required to explain any assumptions that you have made. This can be done using comments in the code or in a readme file, or both.

## Overview

This is a simple number guessing game where the player has to guess a random number between 1 and 100 within 10 tries. The game gives feedback on whether the guess was too high, too low, or correct

## How to Play
1. Enter a number between 1 and 100 in the input field.
2. Click the "Submit Guess" button.
3. After each guess, you'll get feedback indication if your guess was correct, too high, or too low
4. You have 10 attempts to guess the correct number. If you run out of attempts or guess correct, the game will end
5. Once the game ends, a "Play Again" button will appear to start a new game

## Explanation of the code

HTML Structure

h1: Display the game title.
input fields: Allows the user to enter a guess and submit it.
div id="feedback": Displays feedback messages like whether the guess was correct or wrong.

JavaScirpt Logic

randomNumber: Generates a random number between 1 and 100 that the user has to guess.

attempts: Tracks the number of guesses the user has made

showMessage(): A helper function that updates the feedback area with a message and
applies a class (like' win' or 'lose') for styling

checkGuess(): This function is triggered when the user submits a guess. It checks if the guess is correct, too hiugh, or too low, and provides feedback accordingly. It also handles when the game is won or lost
gameOver(): Disables input and adds a "Play Again" button when the game is over.

submitButton.addEventListener('click', checkGuess): Sets up an event listener to call the checkGuess() function when the user clicks the "Submit Guess" button.




#### Known Issues

Issue: Initially, the input field and submit button were not disabling when the game ended.

 Solution: The issue was caused by using disable instead of disabled in the code. Changing it to disabled fixed the problem, allowing the game to properly handle game over and create the reset button.



