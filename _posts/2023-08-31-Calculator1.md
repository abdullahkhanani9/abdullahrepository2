---
toc: true
comments: false
layout: post
title: Calculator
description: This calculator is my version of the calculator from the Slack Message.
type: hacks
courses: { compsci: {week: 2} }
---

<head>
    <title>Mini Calculator</title>
</head>
<body>
    <div>
        <input type="text" id="display" readonly>
    </div>
    <div>
        <button onclick="clearDisplay()">C</button>
        <button onclick="appendToDisplay('7')">7</button>
        <button onclick="appendToDisplay('8')">8</button>
        <button onclick="appendToDisplay('9')">9</button>
        <button onclick="appendToDisplay('+')">+</button>
    </div>
    <div>
        <button onclick="appendToDisplay('4')">4</button>
        <button onclick="appendToDisplay('5')">5</button>
        <button onclick="appendToDisplay('6')">6</button>
        <button onclick="appendToDisplay('-')">-</button>
    </div>
    <div>
        <button onclick="appendToDisplay('1')">1</button>
        <button onclick="appendToDisplay('2')">2</button>
        <button onclick="appendToDisplay('3')">3</button>
        <button onclick="appendToDisplay('*')">*</button>
    </div>
    <div>
        <button onclick="appendToDisplay('0')">0</button>
        <button onclick="appendToDisplay('.')">.</button>
        <button onclick="calculate()">=</button>
        <button onclick="appendToDisplay('/')">/</button>
    </div>
    <script>
        function clearDisplay() {
            document.getElementById('display').value = '';
        }
        function appendToDisplay(value) {
            document.getElementById('display').value += value;
        }
        function calculate() {
            try {
                document.getElementById('display').value = eval(document.getElementById('display').value);
            } catch (error) {
                document.getElementById('display').value = 'Error';
            }
        }
    </script>
</body>
