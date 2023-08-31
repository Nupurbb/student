---
toc: true
comments: true
layout: post
title: TCalc
description: Become one with your tools.  They could be more important than code, code, coding.
type: tangibles
courses: { csse: {week: 0}, csp: {week: 0, categories: [4.A]}, csa: {week: 0} }
categories: [C1.4]
---


## Python Calculator
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Simple Calculator</title>
<style>
  body {
    font-family: Arial, sans-serif;
  }
  .calculator {
    width: 300px;
    margin: 0 auto;
    padding: 20px;
    border: 1px solid #ccc;
    border-radius: 5px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
  }
  input[type="text"] {
    width: 100%;
    padding: 10px;
    margin-bottom: 10px;
    border: 1px solid #ccc;
    border-radius: 3px;
  }
  button {
    width: 50px;
    height: 50px;
    font-size: 18px;
    margin: 5px;
  }
</style>
</head>
<body>
<div class="calculator">
  <input type="text" id="result" readonly>
  <button onclick="appendToResult('7')">7</button>
  <button onclick="appendToResult('8')">8</button>
  <button onclick="appendToResult('9')">9</button>
  <button onclick="appendToResult('+')">+</button>
  <br>
  <button onclick="appendToResult('4')">4</button>
  <button onclick="appendToResult('5')">5</button>
  <button onclick="appendToResult('6')">6</button>
  <button onclick="appendToResult('-')">-</button>
  <br>
  <button onclick="appendToResult('1')">1</button>
  <button onclick="appendToResult('2')">2</button>
  <button onclick="appendToResult('3')">3</button>
  <button onclick="appendToResult('*')">*</button>
  <br>
  <button onclick="appendToResult('0')">0</button>
  <button onclick="calculateResult()">=</button>
  <button onclick="clearResult()">C</button>
  <button onclick="appendToResult('/')">/</button>
</div>

<script>
  function appendToResult(value) {
    document.getElementById("result").value += value;
  }

  function calculateResult() {
    const resultField = document.getElementById("result");
    try {
      resultField.value = eval(resultField.value);
    } catch (error) {
      resultField.value = "Error";
    }
  }

  function clearResult() {
    document.getElementById("result").value = "";
  }
</script>
</body>
</html>


<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Graphing Calculator</title>
<script src="https://cdn.plot.ly/plotly-latest.min.js"></script>
<style>
  body {
    font-family: Arial, sans-serif;
  }
  #calculator {
    width: 300px;
    margin: 0 auto;
    padding: 20px;
    border: 1px solid #ccc;
    border-radius: 5px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
  }
  input[type="text"] {
    width: 100%;
    padding: 10px;
    margin-bottom: 10px;
    border: 1px solid #ccc;
    border-radius: 3px;
  }
  button {
    width: 50px;
    height: 50px;
    font-size: 18px;
    margin: 5px;
  }
  #graph {
    margin-top: 20px;
  }
</style>
</head>
<body>
<div id="calculator">
  <input type="text" id="expression" placeholder="Enter an expression">
  <button onclick="plotGraph()">Plot</button>
</div>
<div id="graph"></div>
<script>
  function plotGraph() {
    const expression = document.getElementById("expression").value;
    const graphDiv = document.getElementById("graph");
    
    try {
      const x = [];
      const y = [];
      for (let i = -10; i <= 10; i += 0.5) {
        x.push(i);
        y.push(eval(expression.replace("x", i)));
      }

      const data = [{ x, y, type: 'scatter', mode: 'lines' }];
      const layout = { title: 'Graph', xaxis: { title: 'x' }, yaxis: { title: 'y' } };
      Plotly.newPlot(graphDiv, data, layout);
    } catch (error) {
      graphDiv.innerHTML = "<p>Error: Invalid expression</p>";
    }
  }
</script>
</body>
</html>

<script>
const secretNumber = Math.floor(Math.random() * 100) + 1;
let attempts = 0;

function checkGuess() {
  const guess = parseInt(document.getElementById("guessInput").value);
  attempts++;

  if (guess === secretNumber) {
    document.getElementById("result").textContent = `Congratulations! You guessed the number ${secretNumber} in ${attempts} attempts.`;
  } else if (guess < secretNumber) {
    document.getElementById("result").textContent = "Try higher!";
  } else {
    document.getElementById("result").textContent = "Try lower!";
  }
}
</script>

</details>