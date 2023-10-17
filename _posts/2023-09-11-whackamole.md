---
toc: true
comments: false
layout: post
title: Whack A Mole
description: This is a Game of Whack-A-Mole we edited to make it our own.
type: hacks
courses: { compsci: {week: 3} }
---

<html>
<head>
    <style>
        body {
            font-family: Times, sans-serif;
            text-align: center;
            background-color: #;
        }
        #game-container {
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            height: 80vh;
        }
        #game-board {
            display: grid;
            grid-template-columns: repeat(3, 130px);
            grid-gap: 40px;
        }
        .hole {
            width: 120px;
            height: 120px;
            background-color: #FF6A4D;
            border: 4px solid #4DA6FF;
            border-radius: 50%;
            cursor: pointer;
            position: relative;
        }
        .mole {
            width: 50px;
            height: 50px;
            background-color: #009919;
            border: 3px solid #330000;
            border-radius: 50%;
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
        }
    </style>
</head>
<body>
    <div id="game-container">
        <p>Click on the moles as they appear!</p>
        <div id="game-board">
            <div class="hole" onclick="whackMole(this)"></div>
            <div class="hole" onclick="whackMole(this)"></div>
            <div class="hole" onclick="whackMole(this)"></div>
            <div class="hole" onclick="whackMole(this)"></div>
            <div class="hole" onclick="whackMole(this)"></div>
            <div class="hole" onclick="whackMole(this)"></div>
            <div class="hole" onclick="whackMole(this)"></div>
            <div class="hole" onclick="whackMole(this)"></div>
            <div class="hole" onclick="whackMole(this)"></div>
        </div>
        <p id="message">Score: 0</p>
    </div>
    <script>
        let score = 0;
        let moleInterval;
        function getRandomHole() {
            const holes = document.querySelectorAll('.hole');
            const randomIndex = Math.floor(Math.random() * holes.length);
            return holes[randomIndex];
        }
        function popUpMole() {
            const hole = getRandomHole();
            const mole = document.createElement('div');
            mole.classList.add('mole');
            mole.addEventListener('click', () => {
                whackMole(mole);
            });
            hole.appendChild(mole);
            setTimeout(() => {
                hole.removeChild(mole);
            }, 500);
        }
        function whackMole(mole) {
            if (mole.classList.contains('mole')) {
                mole.parentNode.removeChild(mole);
                score++;
                updateScore();
            }
        }
        function updateScore() {
            document.getElementById('message').textContent = `Score: ${score}`;
        }
        function startGame() {
            score = 0;
            updateScore();
            moleInterval = setInterval(popUpMole, 500);
        }
        startGame();
    </script>
</body>
</html>

