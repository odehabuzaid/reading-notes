
## **HTML Links**

- html links are the defining features of the web , we navigate the web using links , we move from page or you can say a location to another using links . 

we can use links between one site to another and from within the same website to another page in it, also we can use links to move from a section to another section on the same web page . and we can use them to compose an email using emain programs.

we create a link using the `<a>` element and we close it using `</a>` : 

the following link will navigate google in the same browser page we are using.

```html 
<a href="http://www.google.com"></a>
```

the following link will open a page from the same website we are building

```html
<a href="./pages/aboutme.html">
```
 the following link will move the active screen to another section on the page .
 
```html
<a href="#Section-ID"></a>
```

we can use it also to compose a new mail message like this : <

```html 
<a href="mailto:odeh.abuzaid@outlook.com"></a>
```


## **HTML css layout**


CSS Grid Layout is two-dimensional layout system, and has  features that make building complex layouts straightforward.

there is a different types of css layout : 

 * Fixed.
 * Elastic.
 * Fluid.

![css layout](https://i.imgur.com/M1KvRAE.png)

## **javascript Fucntions and Methods**

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

---

## **Pair programming**

in software engineering there is some practices that have proven to dramatically improve the quality of code developers produce like :

  * Iterative loops.
  * Code reviews.
  * Fast feedback.
  * Error checking
  * and linting.

  ![pair programming](https://i.imgur.com/oLWzCi5.png)

  **defintion**

  - Pair programming is an agile software development practice in which two programmers team up at one workstation to maximize efficiency but Pairing at the wrong time can be both time consuming and inefficient. 

   If one is a slow thinker/typer or unfocused it can slow down the other one as well. More talk less coding:

   > You might end up explaining things that would be faster to just code

   
