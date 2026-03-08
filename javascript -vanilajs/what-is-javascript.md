# What is JavaScript?

JavaScript is a programming language used to make web pages interactive.

While HTML creates the structure and CSS styles the page, JavaScript adds behavior and functionality.

Example of what JavaScript can do:

- handle button clicks
- validate forms
- update content dynamically
- fetch data from servers
- create animations

---

# HTML, CSS, JavaScript Together

Example:

HTML:

```html
<button onclick="sayHello()">Click Me</button>

JavaScript:

function sayHello() {
  alert("Hello World");
}

When the user clicks the button, JavaScript runs the function.


Where JavaScript Runs

JavaScript runs inside the browser.

Modern browsers include a JavaScript engine such as:

Chrome → V8

Firefox → SpiderMonkey

Safari → JavaScriptCore

How to Add JavaScript to a Page

There are three ways to include JavaScript.

Inline JavaScript
<button onclick="alert('Hello')">Click</button>

Internal JavaScript

Inside the <script> tag.

<script>
console.log("Hello World");
</script>
External JavaScript (Recommended)

HTML:

<script src="script.js"></script>

JavaScript file:

console.log("Hello World");

External files keep the code clean and maintainable.

Example

HTML:

<h1 id="title">Hello</h1>
<button onclick="changeText()">Click</button>

JavaScript:

function changeText() {
  document.getElementById("title").innerText = "Welcome!";
}
Common Beginner Mistakes

❌ Mixing too much JavaScript inside HTML
❌ Not separating code into external files