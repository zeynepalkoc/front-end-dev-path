# React Props

## What are Props?

Props (short for properties) are used to pass data from one component to another.

Props allow components to become dynamic and reusable.

# Example

Example component:

```javascript
function Welcome(props) {
  return <h1>Hello {props.name}</h1>;
}
````

usage:

function App()
{
    return <welcome name="zeynep" />;

}

output
Hello zeynep

passing multiple props

you can pass multiple props to a component

Example

function User(props) {
    return (
        <div>
        <h2>(props.name)</h2>
        <p>(props.age</p>
        </div>
    );
}

usage 

<User name="Zeynep age="22" />


Destructuring Props

props can also be destructured

Example:

function User(name, age){
    return(
        <div>
        <h2>(name)</h2>
        <p>(age)</p>
        </div>
    );
}


Common Beginner Mistakes
❌ Trying to modify props
❌ Forgetting to pass props

Props are read-only.
