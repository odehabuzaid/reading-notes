# Class 10

## **Control Flow**

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

**debugging**

> Debugging is the process of finding errors. It involves aprocess of deduction.

we can use The console to specify the area in which the error is located, so you can try to find the exact error and there is different types of errors. Each creates
its own error object, which can tell you its line number and gives a description of the error.

**excution context**

JavaScript interpreter uses the concept of execution contexts.There is one global execution context; plus, each function creates a new new execution context. They correspond to variable scope.

EXECUTION CONTEXT  : every statement lives in one of three execution contexts

* Global 
* function
* Eval

VARIABLE SCOPE : 

* GLOBAL SCOPE
If a variable is declared outside a function, it can
be used anywhere because it has global scope.
If you do not use the var keyword when creating
a variable, it is placed in global scope.

* FUNCTION-LEVEL SCOPE
When a variable is declared within a function,
it can only be used within that function. This is
because it has function-level scope.


**Using try-Catch**

`try...catch` statement marks a block of statements to try, and specifies one or more responses should an exception be thrown. 

If an exception is thrown, the `try...catch` statement catches it.

`try` block to succeed—but if it does not, you want control to pass to the `catch` block. If any statement within the `try` block (or in a function called from within the try block) throws an exception, control immediately shifts to the `catch` block. If no exception is thrown in the `try` block, the `catch` block is skipped. The `finally` block executes after the `try and catch ` blocks execute but before the statements following the `try...catch` statement.


```js
openMyFile();
try {
  writeMyFile(theData); // This may throw an error
} catch(e) {
  handleError(e); // If an error occurred, handle it
} finally {
  closeMyFile(); // Always close the resource
}
```

[**Back**](https://odehabuzaid.github.io/reading-notes/)                     | [**TOP**](#Class-10) |

