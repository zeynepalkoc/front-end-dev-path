# JavaScript Objects

Objects are used to store data in **key-value pairs**.

They allow us to group related information together.

Example:

```javascript
let user = {
  name: "Zeynep",
  age: 22,
  profession: "Developer"
};

Here:

name, age, profession → keys

"Zeynep", 22, "Developer" → values

Accessing Object Properties

We can access object values using dot notation.

Example:

let user = {
  name: "Zeynep",
  age: 22
};

console.log(user.name);

Output:

Zeynep
Bracket Notation

We can also use brackets.

Example:

console.log(user["age"]);

Output:

22
Adding Properties

We can add new properties to an object.

Example:

let user = {
  name: "Zeynep"
};

user.city = "Istanbul";

console.log(user);

Result:

{
  name: "Zeynep",
  city: "Istanbul"
}
Updating Properties

Object values can be updated.

Example:

let user = {
  age: 22
};

user.age = 23;

console.log(user.age);

Output:

23
Example
let product = {
  name: "Laptop",
  price: 1500,
  brand: "Apple"
};

console.log(product.name);
console.log(product.price);

Output:

Laptop
1500
Common Beginner Mistakes

❌ Using arrays instead of objects for structured data
❌ Forgetting quotes around string values