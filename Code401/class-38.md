
# Class 38

*  [Conditional Rendering](#Conditional-Rendering)
*  [Lists & Keys](#Lists-&-Keys)
*  [Forms](#Forms)
*  [Lifting State](#Lifting-State)
*  [Composition vs Inheritance](#Composition-vs-Inheritance)
*  [Thinking in React](#Thinking-in-React)
# Conditional Rendering
In React, you can create distinct components that encapsulate behavior you need. Then, you can render only some of them, depending on the state of your application. Conditional rendering in React works the same way conditions work in JavaScript.

## Conditionally
-   If Component.
-   IIFE.
-   Variable.
-   Render Function.
-   Component.
-   Ternary.
-   The And Operator.
-   What if the Component Needs to Hide Itself?


### Constant declaration

ES6 introduced the `const` keyword, which cannot be redeclared or reassigned, but is not immutable.

ES6

```js
const CONST_IDENTIFIER = 0 // constants are uppercase by convention
```


### Arrow functions

The arrow function expression syntax is a shorter way of creating a function expression. Arrow functions do not have their own `this`, do not have prototypes, cannot be used for constructors, and should not be used as object methods.

ES5

```js
function func(a, b, c) {} // function declaration
var func = function (a, b, c) {} // function expression
```

ES6

```js
let func = (a) => {} // parentheses optional with one parameter
let func = (a, b, c) => {} // parentheses required with multiple parameters
```

### Implicit returns

The `return` keyword is implied and can be omitted if using arrow functions without a block body.

ES5

```js
function func(a, b, c) {
  return a + b + c
}
```

ES6

```js
let func = (a, b, c) => a + b + c // curly brackets must be omitted
```

### Method definition shorthand

The `function` keyword can be omitted when assigning methods on an object.

ES5

```js
var obj = {
  a: function (c, d) {},
  b: function (e, f) {},
}
```

ES6

```js
let obj = {
  a(c, d) {},
  b(e, f) {},
}
```

```js
obj.a() // call method a
```

### Destructuring (object matching)

Use curly brackets to assign properties of an object to their own variable.

```js
var obj = {a: 1, b: 2, c: 3}
```

ES5

```js
var a = obj.a
var b = obj.b
var c = obj.c
```

ES6

```js
let {a, b, c} = obj
```


### Array iteration (looping)

A more concise syntax has been introduced for iteration through arrays and other iterable objects.

```js
var arr = ['a', 'b', 'c']
```

ES5

```js
for (var i = 0; i < arr.length; i++) {
  console.log(arr[i])
}
```

ES6

```js
for (let i of arr) {
  console.log(i)
}
```

### Default parameters

Functions can be initialized with default parameters, which will be used only if an argument is not invoked through the function.

ES5

```js
var func = function (a, b) {
  b = b === undefined ? 2 : b
  return a + b
}
```

ES6

```js
let func = (a, b = 2) => {
  return a + b
}
```

```js
func(10) // returns 12
func(10, 5) // returns 15
```

### Spread syntax

Spread syntax can be used to expand an array.

ES6

```js
let arr1 = [1, 2, 3]
let arr2 = ['a', 'b', 'c']
let arr3 = [...arr1, ...arr2]

console.log(arr3) // [1, 2, 3, "a", "b", "c"]
```

Spread syntax can be used for function arguments.

ES6

```js
let arr1 = [1, 2, 3]
let func = (a, b, c) => a + b + c

console.log(func(...arr1)) // 6
```

### Classes/constructor functions

ES6 introducess the `class` syntax on top of the prototype-based constructor function.

ES5

```js
function Func(a, b) {
  this.a = a
  this.b = b
}

Func.prototype.getSum = function () {
  return this.a + this.b
}

var x = new Func(3, 4)
```

ES6

```js
class Func {
  constructor(a, b) {
    this.a = a
    this.b = b
  }

  getSum() {
    return this.a + this.b
  }
}

let x = new Func(3, 4)
```

```js
x.getSum() // returns 7
```

### Inheritance

The `extends` keyword creates a subclass.

ES5

```js
function Inheritance(a, b, c) {
  Func.call(this, a, b)

  this.c = c
}

Inheritance.prototype = Object.create(Func.prototype)
Inheritance.prototype.getProduct = function () {
  return this.a * this.b * this.c
}

var y = new Inheritance(3, 4, 5)
```

ES6

```js
class Inheritance extends Func {
  constructor(a, b, c) {
    super(a, b)

    this.c = c
  }

  getProduct() {
    return this.a * this.b * this.c
  }
}

let y = new Inheritance(3, 4, 5)
```

```js
y.getProduct() // 60
```


### Modules - export/import

Modules can be created to export and import code between files.

index.html

```html
<script src="export.js"></script>
<script type="module" src="import.js"></script>
```

export.js

```js
let func = (a) => a + a
let obj = {}
let x = 0

export {func, obj, x}
```

import.js

```js
import {func, obj, x} from './export.js'

console.log(func(3), obj, x)
```

### Promises/Callbacks

Promises represent the completion of an asynchronous function. They can be used as an alternative to chaining functions.

ES5 callback

```js
function doSecond() {
  console.log('Do second.')
}

function doFirst(callback) {
  setTimeout(function () {
    console.log('Do first.')

    callback()
  }, 500)
}

doFirst(doSecond)
```

ES6 Promise

```js
let doSecond = () => {
  console.log('Do second.')
}

let doFirst = new Promise((resolve, reject) => {
  setTimeout(() => {
    console.log('Do first.')

    resolve()
  }, 500)
})

doFirst.then(doSecond)
```

An example below using `XMLHttpRequest`, for demonstrative purposes only FETCH API.

ES5 callback

```js
function makeRequest(method, url, callback) {
  var request = new XMLHttpRequest()

  request.open(method, url)
  request.onload = function () {
    callback(null, request.response)
  }
  request.onerror = function () {
    callback(request.response)
  }
  request.send()
}

makeRequest('GET', 'https://url.json', function (err, data) {
  if (err) {
    throw new Error(err)
  } else {
    console.log(data)
  }
})
```
[Fetch API](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API)

ES6 Promise

```js
function makeRequest(method, url) {
  return new Promise((resolve, reject) => {
    let request = new XMLHttpRequest()

    request.open(method, url)
    request.onload = resolve
    request.onerror = reject
    request.send()
  })
}

makeRequest('GET', 'https://url.json')
  .then((event) => {
    console.log(event.target.response)
  })
  .catch((err) => {
    throw new Error(err)
  })
```

Source : [View on GitHub](https://github.com/taniarascia/es6)






# Lists & Keys
Keys help React distinguish items in a list. It helps React manage the changed items, new items added, or items removed from the list. We can output lists JavaScript arrays and the map() function.

key is used to identify unique elements, so that between 2 render passes React knows if an element is a new thing or an updated thing. Remember that React diffs each render to determine what actually changed in the DOM.


## Rendering a Component

```js
const element = <div />;
```

elements can also represent user-defined components:

```js
const element = <Welcome name="Sara" />;
```

When React sees an element representing a user-defined component, it passes JSX attributes and children to this component as a single object. We call this object “props”.

```js
function Welcome(props) {  
    return <h1>Hello, {props.name}</h1>;
}

const element = <Welcome name="Sara" />;ReactDOM.render(
  element,
  document.getElementById('root')
);
```
## State and Lifecycle

Lifecycle methods are special methods built-in to React, used to operate on components throughout their duration in the DOM. For example, when the component mounts, renders, updates, or unmounts. You already know the most important lifecycle method, the render method.
    
    State is a plain JavaScript object used by React to represent an information about the component's current situation. It's managed in the component.


## Handling Events

Handling events with React elements is very similar to handling events on DOM elements. There are some syntax differences:

-   React events are named using camelCase, rather than lowercase.
-   With JSX you pass a function as the event handler, rather than a string.

```html
<button onclick="activateLasers()">
  Activate Lasers
</button>
```

React

```html
<button onClick={activateLasers}>  Activate Lasers </button>

```

Another difference is that you cannot return `false` to prevent default behavior in React. You must call `preventDefault` explicitly. For example, with plain HTML, to prevent the default form behavior of submitting, you can write:

```html
<form onsubmit="console.log('You clicked submit.'); return false">
  <button type="submit">Submit</button>
</form>
```

In React

```js
function Form() {
  function handleSubmit(e) {
    e.preventDefault();    console.log('You clicked submit.');
  }

  return (
    <form onSubmit={handleSubmit}>
      <button type="submit">Submit</button>
    </form>
  );
}
```



# Forms
    React-hook-form is a library that helps you validate forms in React. React-hook-form is a minimal library without any other dependencies. It is performant and straightforward to use, requiring developers to write fewer lines of code than other form libraries.


# Lifting State 
`sharing state`

moving it up to the closest common ancestor of the components that need it. This is called “lifting state up”. We will remove the local state from the TemperatureInput and move it into the Calculator instead.

# Composition vs Inheritance
development pattern based on React's original component model where we build components from other components using explicit defined props or the implicit children prop.

# Thinking in React