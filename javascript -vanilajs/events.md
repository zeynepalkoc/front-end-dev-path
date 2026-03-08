# JavaScript Events

Events are actions that occur in the browser.

JavaScript can detect these actions and respond to them.

Examples of events:

- clicking a button
- typing in an input field
- moving the mouse
- submitting a form

---

# Click Event

One of the most common events is the **click event**.

Example HTML:

```html
<button id="btn">Click Me</button>

JavaScript:

let button = document.getElementById("btn");

button.addEventListener("click", function() {
  alert("Button clicked!");
});

When the user clicks the button, the alert appears.

Event Listener

The addEventListener() method allows us to listen for events.

Syntax:

element.addEventListener("event", function);

Example:

button.addEventListener("click", function() {
  console.log("Button clicked");
});
Input Event

The input event detects when the user types in a field.

Example HTML:

<input type="text" id="name">

JavaScript:

let input = document.getElementById("name");

input.addEventListener("input", function() {
  console.log(input.value);
});

This prints the typed text in the console.

Example

HTML:

<h1 id="title">Hello</h1>

<button id="btn">Change Text</button>

JavaScript:

let button = document.getElementById("btn");

button.addEventListener("click", function() {
  document.getElementById("title").innerText = "Text Changed!";
});
Common Beginner Mistakes

❌ Forgetting to select the element before adding the event
❌ Using incorrect event names