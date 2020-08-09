# Online Readings

## [The Call Stack defined on MDN](https://developer.mozilla.org/en-US/docs/Glossary/Call_stack)

**Call Stack**
* Call stack - a mechanism for an interpreter to keep track of its place in a script that calls multiple functions.
  - When a script calls a function, the interpreter adds it to the call stack and then starts carrying out the function.
  - Any functions that are called by that function are added to the call stack further up, and run where their calls are reached.
  - When the current function is finished, the interpreter takes it off the stack and resumes execution where it left off in the last code listing.
  - If the stack takes up more space than it had assigned to it, it results in a "stack overflow" error.
* Start with an empty Call Stack, and then whenever we invoke a function, it is automatically added to the Call Stack. Once the function has executed all of its code, it is automatically removed from the Call Stack. Ultimately, the Stack is empty again. 

## [Understanding the JavaScript Call Stack](https://medium.freecodecamp.org/understanding-the-javascript-call-stack-861e41ae61d4)

**JavaScript Call Stack**
* JavaScript engine - is a single-threaded interpreter comprising of a heap and a single call stack, and can be found in a hosting environment like the browser. The browser provides web APIs like the DOM, AJAX, and Timers.
* Call stack is primarily used for function invocation. The call stack is single function(s) execution that is done one at a time from top to bottom, which makes it synchronous. Vital to Asynchronous programming.
* Asynchronous JavaScript - there is a callback function, an event loop, and a task queue in this JavaScript. The callback function is acted upon by the call stack during execution after the call back function has been pushed to the stack by the event loop. 
* Call stack - a data structure that uses the Last In, First Out (LIFO) principle to temporarily store and manage function invocation.
* LIFO - means that the last function that gets pushed into the stack is the first to be pop out, when the function returns.
* Temporarily store - occurs when the function is invoked, the function, its parameters, and variables are pushed into the call stack to form a stack frame. This stack frame is a memory location in the stack. The memory is cleared when the function returns as it is pop out of the stack.
* Manage function invocation - call stack maintains a record of the position of each stack frame, and it knows the next function to be executed. This is what makes code execution in JavaScript synchronous.
* Stack overflow - occurs when there is a recursive function, which is a function that calls itself, without an exit point. 
* Call stack are - are single-threaded, which means it can only do one thing at a time. Code execution is synchronous. A function invocation creates a stack frame that occupies a temporary memory. It works as a LIFO — Last In, First Out data structure.

## [JavaScript error messages](https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c)

**JavaScript error messages & Debugging**

* Types of error messages:
  - Reference errors: typos, undeclared variables, etc...
  - Syntax errors: occurs when you have something that cannot be parsed in terms of syntax
  - Range errors: when you give an invalid length
  - Type errors: show up when the types you are trying to use or access are incompatible
* Debugging - to debug your JS code use console.log(), and put in the variables you want to check. Or use chrome developer tools by opening your page with your JS code, choose your file to debug, click the line you wanna debug, and refresh your page again. Can also put a debugger statement in your code in the line you want to break. Another method is add conditional breakpoints by right-clicking a previous set breakpoint, which will make your program stop at that point only if a condition is met.
* Call stack - the path that your program has taken to reach the point were you set a breaking point or were you have an error.
* Handling errors - to avoid the code not being executed properly we usually try to catch the errors so we can gracefully fallback to a default state of our application in case of an error. Try using try…catch, which would make an error be thrown but not “uncaught”, so we can send it to a error logging to be checked later and send a fallback to the function. It will also keep your application running despite being with some side effects. Use this when the type checks are becoming “longer than your function logic”, when a request is made and you aren’t sure if the response might change, or temporarily when a code is continuously giving you problems and you still haven’t got around to refactor it.
* Tools to avoid runtime errors: 
  - quokka
  - eslint 
  - TypeScript

## [JavaScript errors reference on MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Errors)

**List of errors**
* Helpful debugging aid that can be used to find out why an error message is being thrown.
* Some of the errors that can occur:
  - Error: Permission denied to access property "x"
  - InternalError: too much recursion
  - RangeError: argument is not a valid code point
  - RangeError: invalid array length
  - RangeError: invalid date
  - RangeError: precision is out of range
  - RangeError: radix must be an integer
  - RangeError: repeat count must be less than infinity
  - RangeError: repeat count must be non-negative
  - ReferenceError: "x" is not defined
  - ReferenceError: assignment to undeclared variable "x"
  - ReferenceError: can't access lexical declaration`X' before initialization
  - ReferenceError: deprecated caller or arguments usage
  - ReferenceError: invalid assignment left-hand side
  - ReferenceError: reference to undefined property "x"
  - SyntaxError: "0"-prefixed octal literals and octal escape seq. are deprecated
  - SyntaxError: "use strict" not allowed in function with non-simple parameters
  - SyntaxError: "x" is a reserved identifier
  - SyntaxError: JSON.parse: bad parsing
  - SyntaxError: Malformed formal parameter
  - SyntaxError: Unexpected token
  - SyntaxError: Using //@ to indicate sourceURL pragmas is deprecated. Use //# instead
  - SyntaxError: a declaration in the head of a for-of loop can't have an initializer
  - SyntaxError: applying the 'delete' operator to an unqualified name is deprecated
