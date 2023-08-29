---
layout: default
title: Student blog
---


## Nupurs Page 

- Freeform Picture: 
<img src="https://github.com/nighthawkcoders/student/assets/128272483/e7aed228-6b0e-4efd-bc62-c246a98a8ae8"
width="300"
height="500"
/>

## About ME
Hi, My name is Nupur and I am a 10th grader at DNHS.

-  I love to spend my free time listening to music, like Taylor Swift. I love to read books and watch tv. I also love to play tennis and play on the Varsity team at DNHS.

- Homework Requirements: I have 3 hours of homework every day, about 45 minutes from each class. For some classes I need to be doing my homework my self to focus but some classes I can do it while I talk to others and colloborate. 
- 
## Partner/Collab
- Me and Sreeja are partners for APCSP. We have known each other for a long time through tennis and are very good friends. We are excited work toghther this trimester to learn new things and have an agile growth mindset.

## Fun Facts
 - Fun Facts about me: I have traveled to 6 continents. My favorite vacation/destination I have been to is New Zealand. I love to bake cookies and brownies. I have an older sister.My favorite animal is a panda.
 
 <img src="https://github.com/nighthawkcoders/student/assets/128272483/55ecbe78-ea81-47fc-b658-ecb4180229e5"
 width="500" height="300"
 />


## Tennis
- I have been playing tennis ever since I was 7 years old and it is still one of my favorite things to do with my time. When I was younger I played alot more of singles at tournaments but now transitioning into high school tennis, I play more doubles. This year is my second year at the Varisty tennis team at Del Norte and I am very excited for a fun season with my teamates!
<img src="https://github.com/nighthawkcoders/student/assets/128272483/fa738dec-c102-48ee-aacb-98b41408d4cc"
 width="500" height="300"
 />

## Problems




## Schedule
<html>
<table>
  <tr>
    <th>period</th>
    <th>Class</th>
    <th>Teacher</th>
  </tr>
  <tr>
    <td>1</td>
    <td>APCSP</td>
    <td>Mr. Mortenson</td>
  </tr>
  <tr>
    <td>2</td>
    <td>AP BIO</td>
    <td>Mrs. P</td>
  </tr>
  <tr>
    <td>3</td>
    <td>Ap Calc</td>
    <td>Mrs. Nydam</td>
  </tr>
  <tr>
    <td>4</td>
    <td>APES</td>
    <td>Mr. Hendricks</td>
  </tr>
  <tr>
    <td>5</td>
    <td>Offroll</td>
    <td>Mr. Giame</td>
  </tr>
</table>
<html>






## Number Guessing Game
<details>
<summary>Click to play the game</summary>

<div id="game-container">
  <p>Welcome to the Number Guessing Game!</p>
  <p>Try to guess the secret number between 1 and 100.</p>
  <input type="number" id="guessInput" placeholder="Enter your guess">
  <button onclick="checkGuess()">Submit Guess</button>
  <p id="result"></p>
</div>

## Challenges We Faced:
- Making the make command work: the command was periodically working and not that reliable to use so instead we started using bundle exec jekyll serve but after reinstalling the new make command it started working again
- Also another challenge we faced was making sure that all the commands were installed because a lot of times the commands kept showing errors despite being continously installed 
- to fix this we rebooted the computer and cleaned up our vs code and it ended up working after that
- Another issue was that my partner was on windows and I was using a mac which made it difficult for us to help each other but we became more familiar with each other's laptops.
- BUT with an AGILE MINDSET and the idea that nothing is too difficult to achieve we persevered through all the issues we faced. 

## Python Calculator
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Simple Calculator</title>
<style>
  /* Add your CSS styling here */
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
  /* Add your CSS styling here */
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