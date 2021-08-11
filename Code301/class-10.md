## Call Stack

1. What is a ‘call’?

`invocation (call)`

2. How many ‘calls’ can happen at once?

`one call`

3. What does LIFO mean?

`Last In First Out `

4. Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.

```
function calledLast(){
 console.log(('calledLast'))
}

function calledSecond(){
  calledLast();
}

function calledFIrst(){
  calledSecond();
}

calledFIrst();

```

4. What causes a Stack Overflow?

`when there is a recursive function without an exit point. The browser (hosting environment) has a maximum stack call that it can accomodate before throwing a stack error.`

## JavaScript error messages

1. What is a ‘refrence error’?

`use a variable that is not yet declared`

2. What is a ‘syntax error’?

`code syntax mistakes`

3. What is a ‘range error’?

`invalid length call`

4. What is a ‘tyep error’?

`accessing a property in an undefined type of variable`

5. What is a breakpoint?

`debugging a statement in your code in the line you want to break.`

6. What does the word ‘debugger’ do in your code?

`detecting existing and potential errors`
