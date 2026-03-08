# Asynchronous JavaScript

JavaScript is single-threaded, which means it executes one task at a time.

However, some operations take time, such as:

- fetching data from an API
- loading files
- waiting for user input

Asynchronous JavaScript allows these tasks to run without blocking the rest of the program.

---

# setTimeout

`setTimeout` runs a function after a specified delay.

Example:

```javascript
setTimeout(function() {
  console.log("Hello after 2 seconds");
}, 2000);


Explanation:

2000 milliseconds = 2 seconds

Callback Functions

A callback is a function passed into another function to be executed later.

Example:

function greet(name, callback) {
  console.log("Hello " + name);
  callback();
}

function sayBye() {
  console.log("Goodbye!");
}

greet("Zeynep", sayBye);

Output:

Hello Zeynep
Goodbye!
Fetch API

fetch() is used to get data from servers.

Example:

fetch("https://jsonplaceholder.typicode.com/users")
  .then(response => response.json())
  .then(data => console.log(data));

This retrieves data from an API.

Async / Await

Modern JavaScript uses async and await for cleaner asynchronous code.

Example:

async function getUsers() {

  let response = await fetch("https://jsonplaceholder.typicode.com/users");

  let data = await response.json();

  console.log(data);

}

getUsers();

This syntax makes asynchronous code easier to read.

Example
async function getPost() {

  let response = await fetch("https://jsonplaceholder.typicode.com/posts/1");

  let post = await response.json();

  console.log(post.title);

}

getPost();
Common Beginner Mistakes

❌ Forgetting to use await
❌ Not handling errors in async code