# React Hooks

## What are Hooks?

Hooks are special functions in React that allow you to use state and other React features inside functional components.

Before Hooks, many features required class components.


---

# Common React Hooks

Some commonly used React hooks are:

- useState
- useEffect
- useContext
- useRef


# useState Hook

`useState` is used to store and update state in a component.

Example:

```javascript
import { useState } from "react";

function Counter() {

  const [count, setCount] = useState(0);

  return (
    <button onClick={() => setCount(count + 1)}>
      {count}
    </button>
  );
}

useEffect Hook

useEffect is used to perform side effects in React components.

Examples:

fetching data

updating the DOM

timers

Example:

import { useEffect } from "react";

function App() {

  useEffect(() => {
    console.log("Component mounted");
  }, []);

  return <h1>Hello</h1>;
}

Example
import { useState, useEffect } from "react";

function Timer() {

  const [count, setCount] = useState(0);

  useEffect(() => {
    console.log("Count changed");
  }, [count]);

  return (
    <button onClick={() => setCount(count + 1)}>
      {count}
    </button>
  );
}
Common Beginner Mistakes

❌ Using Hooks outside components
❌ Forgetting dependency arrays in useEffect

Hooks must always be used inside React components.