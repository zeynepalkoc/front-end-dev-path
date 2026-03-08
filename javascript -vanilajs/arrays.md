# JavaScript Arrays

Arrays are used to store multiple values in a single variable.

Example:

```javascript
let fruits = ["Apple", "Banana", "Orange"];

Here, the variable fruits contains three values.

Accessing Array Elements

Array elements are accessed using their index.

Indexes start from 0.

Example:

let fruits = ["Apple", "Banana", "Orange"];

console.log(fruits[0]);

Output:

Apple

Example:

console.log(fruits[1]);

Output:

Banana
Array Length

The length property returns the number of items in an array.

Example:

let fruits = ["Apple", "Banana", "Orange"];

console.log(fruits.length);

Output:

3
Adding Elements

We can add elements using push().

Example:

let fruits = ["Apple", "Banana"];

fruits.push("Orange");

console.log(fruits);

Result:

["Apple", "Banana", "Orange"]
Removing Elements

We can remove the last element using pop().

Example:

let fruits = ["Apple", "Banana", "Orange"];

fruits.pop();

console.log(fruits);

Result:

["Apple", "Banana"]
Looping Through Arrays

We can loop through arrays using a for loop.

Example:

let fruits = ["Apple", "Banana", "Orange"];

for (let i = 0; i < fruits.length; i++) {
  console.log(fruits[i]);
}

Output:

Apple
Banana
Orange
Example
let skills = ["HTML", "CSS", "JavaScript"];

skills.push("React");

console.log(skills);

Output:

["HTML", "CSS", "JavaScript", "React"]
Common Beginner Mistakes

❌ Forgetting that array indexing starts from 0
❌ Accessing an index that does not exist

Example mistake:

console.log(fruits[10]);

This returns undefined.