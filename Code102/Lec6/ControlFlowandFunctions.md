# Control flow & Functions


## **Control Flow**

the `control flow` is the order in which the computer executes statements in a script.

Code is run in order from the first line in the file to the last line, unless the computer runs across the (extremely frequent) structures that change the control flow, such as conditionals and loops. 

```js 
if (value = something ) {
    promptUser();
} else {
    submitForm();
}
```
- in this case , the code will not continue to the next line it will return to evaluate a new value & so on.

# Functions 

## ** What is a JS function

A  `function` is a block of code that performs a task or calculates a value.
 
it should take some input and return an output where there is some obvious relationship between the input and the output. 

To use a function, you must :  

- define it in the same scope which you will call it.

**Defining functions**

A function definition (declaration) consists of the `function` keyword, followed by:

1- The name of the function.

2- A list of parameters to the function, enclosed in parentheses and separated by commas.

3- The JavaScript statements that define the function, enclosed in curly brackets, {...}.

```js
function name(parameter1, parameter2, parameter3) {
  // code to be executed
}
```

**Example**

### the following function will return the sum of tow variables.

```js
function myFunction(n1, n2) {
  return n1 + n2;   
}
```

### Now this function wont work unless we call it ( **INVOKING** )

```js
console.log(myfunction(2,3))
```
the output for this line will be 

```js
5
```

[**Back**](/../reading-notes/README.md)                     | [**TOP**](#Control-Flow) |