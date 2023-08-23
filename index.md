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