# React Components

Components are the building blocks of React applications.

A component is a reusable piece of user interface.

Instead of writing the same code multiple times, we create components and reuse them.

---

# Functional Components

Modern React uses **functional components**.

Example:

```javascript
function Welcome() {
  return <h1>Hello World</h1>;
}

this component returns a heading 

Using Comonents 

Components can be used inside other components

Exampple:

function welcome()
{
    return <h1>Hello</h1>;
}

fuction App(){
    return(
    <div>
    <welcome />
    </div>
);
}

here the welcome components is used inside app


Reusable Components

components allow code reuse

Example:
Function Card(){
    return( 
        
        <div>
    <h2>Product</h2>
    <p>this is a product card</p>
    )
   

}

using the component multiple times:

Function App(){
    return(
        <div>
        <Card/>
         <Card/>
          <Card/>
        </div>
    );
}

Component Naming Rules

Component names should

*start with a capital letter
*be descriptive

Correct example

function Navbar(){}

Incorrect example

function navbar() {}

react components must start with a capital letter


Example 

function Header(){
    return <h1>my website</h1>
}

function app(){
    return(
        <div>
        <header/>
        <p>welcome to my site </p>
        </div>
    );
}

Common Beginner Mistakes

❌ Forgetting to capitalize component names
❌ Not returning JSX
