# JavaScript Functions

Functions are blocks of code designed to perform a specific task.

They allow us to reuse code instead of writing the same logic multiple times.

Example:

```javascript
function sayHello() {
  console.log("Hello World");
}

To run the function:

sayHello();

Output:

Hello World
Function Structure

A basic function consists of:

the function keyword

a function name

parentheses ()

curly braces {}

Example:

function greet() {
  console.log("Welcome!");
}
Function Parameters

Functions can receive inputs called parameters.

Example:

function greetUser(name) {
  console.log("Hello " + name);
}

Calling the function:

greetUser("Zeynep");

Output:

Hello Zeynep
Returning Values

Functions can return values using the return keyword.

Example:

function add(a, b) {
  return a + b;
}

Using the function:

let result = add(5, 3);

console.log(result);

Output:

8
Arrow Functions

Modern JavaScript also supports arrow functions.

Example:

const greet = () => {
  console.log("Hello");
};

Arrow functions are commonly used in modern JavaScript frameworks like React.

Example
function multiply(a, b) {
  return a * b;
}

let result = multiply(4, 5);

console.log(result);

Output:

20
Common Beginner Mistakes

❌ Forgetting to call the function
❌ Forgetting the return keyword when needed