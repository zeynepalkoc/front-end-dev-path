# JavaScript Variables

Variables are used to store data values.

They allow us to save information and use it later in our program.

Example:

```javascript
let name = "Zeynep";

In this example:

let → variable keyword

name → variable name

"Zeynep" → stored value

Types of Variable Declarations

JavaScript has three ways to declare variables:

var

let

const

var

var was used in older JavaScript.

Example:

var age = 25;

However, var is not recommended in modern JavaScript.

let

let is used for variables that can change.

Example:

let score = 10;

score = 20;

The value can be updated.

const

const is used for variables that should not change.

Example:

const pi = 3.14;

Trying to change it will cause an error.

Example:

const pi = 3.14;

pi = 4;

This will produce an error.

Variable Naming Rules

Good variable names should:

be descriptive

use camelCase

Examples:

let userName = "Ali";
let totalPrice = 100;

Bad examples:

let x = 10;
let a = "name";
Example
let firstName = "Zeynep";
let age = 22;

console.log(firstName);
console.log(age);

Output:

Zeynep
22
Common Beginner Mistakes

❌ Using var instead of let or const
❌ Choosing unclear variable names