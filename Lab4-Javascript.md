>![Jsimg](https://iconape.com/wp-content/files/vr/353405/svg/javascript-js-seeklogo.com.svg)

# Introduction

**Javascript** is a programming language was initially created by Brenden Eich to make “web pages alive”. The programs in this language are called scripts.  It is most commonly known as a client-side scripting language. 

**Javascript** helps to do Web Application Development and make dynamic and interactive webpages by implementing custom client-side scripts. Javascript is basically the English Language of programming. It isn’t quite used by everyone, everywhere but it is still has a significant presence in the industry.

- Easily accessible
- Make the website more interactive
- User friendly

**Javascript** is used by almost 95% of websites due to its user-friendly and client-side scripts. Due to its easy accessibility, it is used for various Web applications.

# JavaScript Besics

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

## **Examples**

*Assign* values to variables and add them together:
```js
var x = 5;         // assign the value 5 to x
var y = 2;         // assign the value 2 to y
var z = x + y;     // assign the value 7 to z (5 + 2)
```

**Control flow**

> The control flow is the order in which the computer executes statements in a script.

*Code* is run in order from the first line in the file to the last line, unless the computer runs across the (extremely frequent) structures that change the control flow, such as conditionals and loops. 

to control the order of excuting statements we use 

* Block
* break
* continue
* Empty
* if...else
* switch
* throw
* try...catch

## **Examples**

**Block statement**

The most basic statement is a block statement, which is used to group statements. The block is delimited by a pair of curly brackets:
```js
{
  statement_1;
  statement_2;
  ⋮
  statement_n;
}
```
**Block statements** are commonly used with control flow statements (if, for, while).
```js
while (x < 10) {
  x++;
}
```

**Conditional statements**
A **conditional statement** is a set of commands that executes if a specified condition is true. JavaScript supports two conditional statements: if...else and switch.

*if...else statement*
Use the if statement to execute a statement if a logical condition is true. Use the optional else clause to execute a statement if the condition is false.

An if statement looks like this:

```js
if (condition) {
  statement_1;
} else {
  statement_2;
}
```

Here, the condition can be any expression that evaluates to true or false. (See Boolean for an explanation of what evaluates to true and false.)

If condition evaluates to true, statement_1 is executed. Otherwise, statement_2 is executed. statement_1 and statement_2 can be any statement, including further nested if statements.

You can also combine the statements using else if:

```js
if (condition_1) {
  statement_1;
} else if (condition_2) {
  statement_2;
} else if (condition_n) {
  statement_n;
} else {
  statement_last;
}
```

In the case of multiple conditions, only the first logical condition which evaluates to true will be executed. To execute multiple statements, group them within a block statement ({ … }).

[ReadMore..](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Control_flow_and_error_handling)


** 



