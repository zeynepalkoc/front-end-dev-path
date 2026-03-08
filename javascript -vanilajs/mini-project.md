# JavaScript Mini Project: Counter App

In this mini project, we will build a simple **counter application** using JavaScript.

Concepts used in this project:

- variables
- functions
- DOM manipulation
- events

---

# Project Goal

Create a counter that can:

- increase the number
- decrease the number
- reset the counter

---

# HTML Structure

```html
<!DOCTYPE html>
<html>

<head>
<title>Counter App</title>
</head>

<body>

<h1>Counter</h1>

<h2 id="count">0</h2>

<button id="increase">Increase</button>
<button id="decrease">Decrease</button>
<button id="reset">Reset</button>

<script src="script.js"></script>

</body>

</html>

JavaScript Code

Create a file called script.js.

let count = 0;

let countDisplay = document.getElementById("count");

let increaseBtn = document.getElementById("increase");
let decreaseBtn = document.getElementById("decrease");
let resetBtn = document.getElementById("reset");

increaseBtn.addEventListener("click", function() {
  count++;
  countDisplay.innerText = count;
});

decreaseBtn.addEventListener("click", function() {
  count--;
  countDisplay.innerText = count;
});

resetBtn.addEventListener("click", function() {
  count = 0;
  countDisplay.innerText = count;
});

How It Works

The application:

stores the counter value in a variable

listens for button clicks

updates the number on the page

Example

User clicks Increase

0 → 1 → 2 → 3

User clicks Decrease

3 → 2 → 1

User clicks Reset

0
