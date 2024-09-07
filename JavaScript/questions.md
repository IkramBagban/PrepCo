# JavaScript Interview Questions

## Basic Questions

### What are the different data types in JavaScript?
**Answer**: JavaScript supports several data types including `Number`, `String`, `Boolean`, `Object`, `Array`, `Function`, and `Symbol`.

### Explain the difference between `null` and `undefined`.
**Answer**: `null` is an assignment value that represents the intentional absence of any object value. `undefined` indicates that a variable has been declared but has not yet been assigned a value.

### How do you handle errors in JavaScript?
**Answer**: Errors in JavaScript are handled using `try-catch` blocks. Code that may throw an error is placed inside the `try` block, and error handling code is placed inside the `catch` block.

## Advanced Questions

### What is a closure and how is it used?
**Answer**: A closure is a function that retains access to its lexical scope, even when the function is executed outside that scope. Closures are used to create private variables and functions.

### Describe the event loop and how it handles asynchronous operations.
**Answer**: The event loop is a mechanism that allows JavaScript to perform non-blocking operations. It processes tasks in the event queue and executes them after the current execution context is finished.

### How do `call`, `apply`, and `bind` methods differ?
**Answer**: `call` and `apply` invoke a function with a specified `this` value and arguments, but `call` takes arguments as a comma-separated list, while `apply` takes arguments as an array. `bind` creates a new function with a specified `this` value and optional initial arguments.

## ES6+ Features Questions

### What are the benefits of using `let` and `const` over `var`?
**Answer**: `let` and `const` provide block-scoping and prevent variable hoisting issues. `const` is used for constants whose values cannot be reassigned.

### Explain how arrow functions differ from traditional functions.
**Answer**: Arrow functions have a shorter syntax and do not have their own `this` context, which can be useful for maintaining lexical `this` in callbacks.

### What is destructuring and how is it used?
**Answer**: Destructuring is a syntax for extracting values from arrays or properties from objects into distinct variables. It simplifies extracting multiple properties from objects or elements from arrays.
