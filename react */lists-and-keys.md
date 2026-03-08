# React Lists and Keys

## What are Lists in React?

In React, lists are used to render multiple items dynamically.

Lists are usually created by looping through arrays.

Example use cases:

- todo lists
- product lists
- user lists


# Using map() to Render Lists

React uses the `map()` function to render lists.

Example:

```javascript
function App() {

  const fruits = ["Apple", "Banana", "Orange"];

  return (
    <ul>
      {fruits.map((fruit) => (
        <li>{fruit}</li>
      ))}
    </ul>
  );
}

Keys in React

React requires a key for each item in a list.

Keys help React identify which items changed.

Example:

function App() {

  const fruits = ["Apple", "Banana", "Orange"];

  return (
    <ul>
      {fruits.map((fruit, index) => (
        <li key={index}>{fruit}</li>
      ))}
    </ul>
  );
}

Example
function App() {

  const users = [
    {id:1, name:"name1},
    {id:2, name:"name2"},
    {id:3, name:"name2"}
  ];

  return (
    <ul>
      {users.map((user) => (
        <li key={user.id}>
          {user.name}
        </li>
      ))}
    </ul>
  );
}


Common Beginner Mistakes

❌ Forgetting the key attribute
❌ Using non-unique keys