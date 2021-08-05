## React Docs - thinking in React

* How would you break a mock into a component heirarchy?
 
`rendering boxes around components and subcomponent in the mock and name them all`

* What is the single responsibility principle and how does it apply to components?

`its a computer-programming principle that states that every module, class or function in a computer program should have responsibility over a single part of that program's functionality, and it should encapsulate that part`

* What does it mean to build a ‘static’ version of your application?

` don’t use state at all `

* Once you have a static application, what do you need to add?

`responsibility`

* What are the three questions you can ask to determine if something is state?

`1. Is it passed in from a parent via props?`

`2. Does it remain unchanged over time? `

`3. Can you compute it based on any other state or props in your component?`



* How can you identify where state needs to live?

``` 
Identify every component that renders something based on that state.
Find a common owner component (a single component above all the components that need the state in the hierarchy).
Either the common owner or another component higher up in the hierarchy should own the state. 

```