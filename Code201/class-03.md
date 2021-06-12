# Class 3

# **HTML lists**

#### The types of lists that can be used in HTML are :

ul : An unordered list.list items using bullets.
ol : An ordered list. use different schemes of numbers to list items.
dl : A definition list. This arranges items in the same way as they are arranged in a dictionary.

**examples**: 

```html
<h1> Unordered List </h1>
<ul>
  <li>Home</li>
  <li>about</li>
  <li>contact</li>
</ul>

<h1> ordered List </h1>
<ol>
  <li>Home</li>
  <li>about</li>
  <li>contact</li>
  </ol>

<h1> We can nest difrent types of list </h1>

<ol>
  <li>Home</li>
  <li>about
    <ul>
      <li>about us</li>
      <li>about me</li>
    </ul>
  </li>
  <li>contact</li>
</ol>

```

## **HTML Boxes**

box-sizing property allows us to include the padding and border in an element's also total width and height. If you are setting a  box-sizing: border-box; on an element, padding and border are included in the width and height: Both divs are the same size now

<img src="https://i.imgur.com/3JCVnRo.png" width="300" height="250" alt="source : w3schools">


**examples**: 

```css
.div1 {
  width: 300px;
  height: 100px;
  border: 1px solid blue;
}

.div2 {
  width: 300px;
  height: 100px;
  padding: 50px;
  border: 1px solid red;
}
```

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

```js 
while (condition){
 execute code block
}
```
#### Control flow and error handling

JavaScript supports a compact set of statements, specifically control flow statements, that you can use to incorporate a great deal of interactivity in your application. This chapter provides an overview of these statements.   

**Block statement**

which is used to group statements. The block is delimited by a pair of curly brackets:

```js
{
  statement_1;
  statement_2;
  ⋮
  statement_n;
}

<h1> Example </h1>
while (x < 10) {
  x++;
}

```
**Conditional statements**

is a set of commands that executes if a specified condition is true. 

*if...else*

execute a statement if a logical condition is true. Use the optional else clause to execute a statement if the condition is false.


```js
{
if (condition) {
  statement_1;
} else {
  statement_2;
}
}


if (condition_1) {
  statement_1;
} else if (condition_2) {
  statement_2;
} else if (condition_n) {
  statement_n;
} else {
  statement_last;
}

<h1> Best practice </h1>

if (condition) {
  statement_1_runs_if_condition_is_true;
  statement_2_runs_if_condition_is_true;
} else {
  statement_3_runs_if_condition_is_false;
  statement_4_runs_if_condition_is_false;
}

```

*switch*

allows a program to evaluate an expression and attempt to match the expression's value to a case label. If a match is found, the program executes the associated statement.

```js


  case label_1:
    statements_1
    [break;]
  case label_2:
    statements_2
    [break;]
    …
  default:
    statements_def
    [break;]
}

```

[read More](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Control_flow_and_error_handling)


   [**Back**](https://odehabuzaid.github.io/reading-notes/)                     | [**TOP**](#Class-3) |