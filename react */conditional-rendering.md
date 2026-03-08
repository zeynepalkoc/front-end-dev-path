# React Conditional Rendering

## What is Conditional Rendering?

Conditional rendering allows React to display different content depending on certain conditions.

Example situations:

- user logged in / not logged in
- loading state
- showing or hiding components


---

# Using if Statement

Example:

```javascript
function App() {

  const isLoggedIn = true;

  if (isLoggedIn) {
    return <h1>Welcome back</h1>;
  }

  return <h1>Please log in</h1>;
}

if Kullanımı

Burada:

isLoggedIn

değeri true ise farklı, false ise farklı içerik gösterilir.

Ternary Operator

The ternary operator is commonly used in React.

Example:

function App() {

  const isLoggedIn = true;

  return (
    <div>
      {isLoggedIn ? <h1>Welcome</h1> : <h1>Please log in</h1>}
    </div>
  );
}

Conditional Rendering with &&

React also allows conditional rendering using &&.

Example:

function App() {

  const isAdmin = true;

  return (
    <div>
      {isAdmin && <h1>Admin Panel</h1>}
    </div>
  );
}

Example
import { useState } from "react";

function App() {

  const [loggedIn, setLoggedIn] = useState(false);

  return (
    <div>

      {loggedIn ? <h1>Dashboard</h1> : <h1>Login Page</h1>}

      <button onClick={() => setLoggedIn(!loggedIn)}>
        Toggle
      </button>

    </div>
  );
}

Common Beginner Mistakes

❌ Using complex conditions inside JSX
❌ Forgetting curly braces {}