# React Event Handling

## What is Event Handling?

Event handling allows React components to respond to user actions.

Examples of events:

- clicking a button
- typing in an input field
- submitting a form

---

# Click Events

React handles click events using `onClick`.

Example:

```javascript
function App() {

  function handleClick() {
    alert("Button clicked!");
  }

  return (
    <button onClick={handleClick}>
      Click Me
    </button>
  );
}
Input Events

React can detect user input using onChange.

Example:

function App() {

  function handleChange(event) {
    console.log(event.target.value);
  }

  return (
    <input type="text" onChange={handleChange} />
  );
}


Example
import { useState } from "react";

function App() {

  const [name, setName] = useState("");

  function handleChange(event) {
    setName(event.target.value);
  }

  return (
    <div>
      <input type="text" onChange={handleChange} />

      <h1>Hello {name}</h1>
    </div>
  );
}

Common Beginner Mistakes

❌ Writing onClick="handleClick()" like HTML
❌ Forgetting curly braces in JSX

Correct:

onClick={handleClick}