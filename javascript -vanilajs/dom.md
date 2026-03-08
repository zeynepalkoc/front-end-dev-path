# JavaScript DOM (Document Object Model)

The DOM represents the structure of an HTML document as a tree of objects.

JavaScript can use the DOM to:

- access HTML elements
- modify content
- change styles
- respond to user actions

---

# Accessing HTML Elements

JavaScript can select elements from the page.

Example HTML:

```html
<h1 id="title">Hello</h1>

JavaScript:

let title = document.getElementById("title");

console.log(title);

This selects the element with the id title.

querySelector

querySelector() allows selecting elements using CSS selectors.

Example:

let element = document.querySelector("h1");

Selecting a class:

let element = document.querySelector(".box");

Selecting an id:

let element = document.querySelector("#title");
Changing Text Content

We can modify text using innerText.

Example:

let title = document.getElementById("title");

title.innerText = "Welcome!";

The text inside the element will change.

Changing HTML Content

We can update HTML using innerHTML.

Example:

let box = document.querySelector(".box");

box.innerHTML = "<strong>Hello</strong>";
Changing Styles

JavaScript can also modify CSS styles.

Example:

let title = document.getElementById("title");

title.style.color = "blue";
Example

HTML:

<h1 id="title">Hello</h1>

<button onclick="changeText()">Click</button>

JavaScript:

function changeText() {
  let title = document.getElementById("title");
  title.innerText = "Welcome to JavaScript";
}
Common Beginner Mistakes

❌ Running JavaScript before the HTML loads
❌ Selecting elements that do not exist