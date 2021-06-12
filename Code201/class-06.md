# Class 6

## **Problem Domain**

> the Hardest part of programming 
- John Sonmez

we must understand the complete picture in a problem domain so we can deliver a code that solve the problem , & if there was missing parts or incomplete information about the problem domain which will lead to incomplete solution.

in the real world , problem domain can be extreamly complicated and difficult to understand.

as a programmer , if you were handled a full specifications and a use case diagrams like the ones in the waterfall approach . it would make the coding easier so the problem will ne solved faster, because as a programmer you were handed the problem domain in details which make it more understandable. 


**Understanding the problem Domain**

to understand problem domain easier , its recommended to cut ou the cases and narrow the focus on the problem domain part by part, deviding the problem domain to parts & understanding them separately makes a full problem domain understanding.




## **Object Literals**

its a comma-separated list of name-value pairs wrapped inn curly braces. they encapsulate data and enclosing it in a small package . 

which will minimize the global variables count on our code .

the following is an example of Object literal use in javascript

```js 
let myObject = {
    name: 'Some Name as a string',
    age: 30,
    active : false
};
```

- the values can be of any data type ,
- arrays , functions also nested object literals can be a value of an object literal.

```js
let  banner = {
    images: ["smile.gif", "grim.gif", "frown.gif", "bomb.gif"],
    position: {
        x: 40,
        y: 300
    },
    onSwap: function() { 
        // code here
    }
};
```

## **Document Object Model**

the `DOM` is a platform & an interface gives programs and scripts a dynamic access to the content and the structure or the style of a document.

in HTML `DOM` Defines : 

    - the html elements as objects.
    - the properties of all html elements.
    - the methods to access all html elements.
    - the events for all html elements.

so the `DOM` is a standard for the way of getting , modify , adding or even removing HTML elements of a loaded web page in the browser.

>![Jsimg](https://www.optimizesmart.com/wp-content/uploads/2014/05/HTML-DOM-Tree.jpg)



[**Back**](https://odehabuzaid.github.io/reading-notes/)                     | [**TOP**](##Problem-Domain) |



