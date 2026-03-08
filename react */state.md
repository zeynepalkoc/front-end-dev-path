 # React State

## What is State?

State is a built-in object in React that stores data which can change over time.

When the state changes, React automatically re-renders the component.


# useState Hook

In modern React, we use the **useState hook** to manage state.

Example:

```javascript
import { useState } from "react";

function Counter() {

  const [count, setCount] = useState(0);

  return (
    <div>
      <h1>{count}</h1>
    </div>
  );
}

Updating State

State can be updated using the setter function

Example

import { useState} from "react";
function Counter()
{
    const [ count, setCount]= useState(0);

    return(
        <div>
        <h1>{count}</h1>
        <button onclick={() =setCount(count +1)}>
        ıncrease
        </button>

        </div>
    );
}

Example
import { useState } from "react";

function App() {

  const [name, setName] = useState("Zeynep");

  return (
    <div>
      <h1>Hello {name}</h1>

      <button onClick={() => setName("Developer")}>
        Change Name
      </button>
    </div>
  );
}

Common Beginner Mistakes

❌ Trying to change state directly

Wrong:

count = count + 1

Correct:

setCount(count + 1)