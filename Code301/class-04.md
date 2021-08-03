## React Forms

1. What is a ‘Controlled Component’?

its a `component` where form data is `handled by a React component`. 
unlike the uncontrolled components, where form data is `handled by the DOM itself`.

2. Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.

it depends on alot of things, 
Mainly it depends on what that state is used for in our app.
and if that update affect the results of what depending on the value of that state.

for example : in lab 3 , ...  the results of the search must be narrowed down and displayed `every time the user enters or removes a character from the input`

3. How do we target what the user is entering if we have an event handler on an input field?

`VALUE`

## Ternary Operator 
1. Why would we use a ternary operator?

`SHORTER syntax in case of simple condition`

2. Rewrite the following statement using a ternary statement:

```js
x===y ? console.log(true) : console.log(false)

```