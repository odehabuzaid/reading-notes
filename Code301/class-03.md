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