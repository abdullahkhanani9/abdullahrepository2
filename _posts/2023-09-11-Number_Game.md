---
toc: true
comments: false
layout: post
title: Number Guess Game
description: This is a number guessing game in whiched we edited the colors, the values, and the text.
type: hacks
courses: { compsci: {week: 3} }
---

<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <style>
        body {
            font-family: Times, sans-serif;
            text-align: center;
            background-color: #AAFF99;
        }
        #game-container {
            margin: 0 auto;
            width: 500px;
            padding: 10px;
            background-color: #FF6A4D;
            box-shadow: 1px 30px 15px #0000B3;
        }
    </style>
</head>
<body>
    <div id="game-container">
        <p>Guess a number between 1 and 50:</p>
        <input type="text" id="guess" placeholder="Enter your guess">
        <button id="submit">Submit Guess</button>
        <p id="message"></p>
    </div>
    <script>
        // Generate a random number between 1 and 50
        const randomNumber = Math.floor(Math.random() * 50) + 1;
        const guessInput = document.getElementById('guess');
        const submitButton = document.getElementById('submit');
        const message = document.getElementById('message');
        let attempts = 0;
        submitButton.addEventListener('click', () => {
            const userGuess = parseInt(guessInput.value);
            attempts++;
            if (isNaN(userGuess) || userGuess < 1 || userGuess > 50) {
                message.textContent = 'Please enter a valid number between 1 and 50.';
            } else if (userGuess === randomNumber) {
                message.textContent = `Congratulations! You guessed the number ${randomNumber} correctly in ${attempts} attempts.`;
                submitButton.disabled = true;
                guessInput.disabled = true;
            } else if (userGuess < randomNumber) {
                message.textContent = 'Your number is too low.';
            } else {
                message.textContent = 'Your number is too high.';
            }
            guessInput.value = '';
            guessInput.focus();
        });
    </script>
</body>
</html>