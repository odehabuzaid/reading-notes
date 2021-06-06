>![Jsimg](https://iconape.com/wp-content/files/vr/353405/svg/javascript-js-seeklogo.com.svg)


## **Expressions and operators**

**Expressions**
they are units of code that can be evaluated and resolve to a value. Expressions in JS can be divided in categories.

* Arithmetic expressions
* String expressions
* Primary expressions
* Array and object initializers expressions
* Logical expressions
* Left-hand-side expressions
* Property access expressions
* Object creation expressions
* Function definition expressions
* Invocation expressions

[ReadMore..](https://flaviocopes.com/javascript-expressions/#:~:text=JavaScript%20Expressions%20Expressions%20are%20units%20of%20code%20that,be%20divided%20in%20categories.%20Published%20Mar%2017%2C%202018)

**Operators**
JavaScript has the following types of operators. This section describes the operators and contains information about operator precedence.

* Assignment operators
* Comparison operators
* Arithmetic operators
* Bitwise operators
* Logical operators
* String operators
* Conditional (ternary) operator
* Comma operator
* Unary operators
* Relational operators

[ReadMore..](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators)


## **Loops**

There is many different kinds of loops , like 

- **FOR** 
- **do...while**

but after all they are all doing the same thing which is repeating an action some number of times.

### for statement

> A `for` loop repeats until a specified condition evaluates to false.

```js

for ([initialExpression]; [conditionExpression]; [incrementExpression])
  statement

```

for *example*

```js

function howMany(selectObject) {
  let numberSelected = 0;
  for (let i = 0; i < selectObject.options.length; i++) {
    if (selectObject.options[i].selected) {
      numberSelected++;
    }
  }
  return numberSelected;
}

``` 
### do...while statement

> The `do...while` statement will keep repeating the code within the do block, until a specified condition evaluates to false .

```js

do
  statement
while (condition);

```

for *example*

```js

let i = 0;
do {
  i += 1;
  console.log(i);
} while (i < 5);

``` 

read more about For and do ... while statements [Here](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Loops_and_iteration#for_statement).

[**Back**](https://odehabuzaid.github.io/reading-notes/)                     | [**TOP**](#Expressions-and-operators) |