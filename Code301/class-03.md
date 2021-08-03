# lists and keys

* What does .map() return? 

`elements of given iterable array`

* If I want to loop through an array and display each value in JSX, how do I do that in React?

```js
Console.log(array.map(element => element))

```
* Each list item needs a unique `key`.

* What is the purpose of a key? 
`create a relationship between the component and the DOM element`

# The Spread Operator

* What is the spread operator?
It takes in an iterable and expands it into individual elements.

*List 4 things that the spread operator can do.
-Copying an array
-Inserting the elements of one array into another
-Array to arguments
-expand the array 

Give an example of using the spread operator to combine two arrays.

```js
let males = ['hasan', 'ali', 'sanad'];
let females = ['salma', 'noor', 'nidaa', ...males];
```

Give an example of using the spread operator to add a new item to an array.

```js
let females = ['salma', 'noor', 'nidaa', ...males];
```
Give an example of using the spread operator to combine two objects into one.

```js
let males = ['hasan', 'ali', 'sanad'];
let females = ['salma', 'noor', 'nidaa', ...males];
let all = {...males,...females};
```

# Passing data between components

* In the video, what is the first step that the developer does to pass functions between components?

`declear a function in the parent scoop and pass it as a prop to the child`

* in your own words, what does the increment function do?

`it takes a name on its args ,declear a variable called `ppl`

loop the state using the map method. 

lookup that name using the mapped element ` p `, 

using that element : if the value of the key 'name' equals the name givin in the parameters 

update the key named 'count' value of to that element 

THEN return the element `p` to the `ppl` object.

after map finish set the state object : `people` value from new updated 'ppl'

* How can you pass a method from a parent component into a child component?

`as a prop` and we can `export` it from the parent and `import` it inside the childern 

* How does the child component invoke a method that was passed to it from a parent component?

calling the prop that allready sent as `this.prop.functionName`
import it and call it like any method / property decleared inside child class. 

## Things I want to know more about
Bootstrap grid layout 

