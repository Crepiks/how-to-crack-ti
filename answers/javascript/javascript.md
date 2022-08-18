# JavaScript Interview Answers

## What are primitive data types?

Primitive data types are the data types which are copied by values not by reference. Primive data types in JavaScript: Number, String, null, undefined, Boolean.

## What is undefined property?

Is a property which has no values different from `undefined` or even never was set value.

## What is null value?

Null value is a value which was explicitly assigned null.

## What is the difference between null and undefined?

`undefined` is a default value for all uninitialized values. Null ia a sign that variable was marked as having to value explicitly.

## What is the difference between window and document?

Windows is located higher in a hierarchy and refers to the whole browser windows with different APIs. Document is only a reference to DOM tree.

## What is isNaN?

`isNaN` is a function which check that provided value if NOT a number.

## What is the difference between let, const and var?

`let` and `const` are scoped by block scope when `var` is scoped only by function scope. `const` preserves the link to value when `let` can be reassigned its link.

## What are the differences between undeclared and undefined variables?

Undefined variable means a variable has been declared but it does not have a value. Undeclared variable means that the variable does not exist in the script at all.

## What are global variables?

Global variables are variables accessible in window's scope.

## What is NaN property?

NaN is a special value which appears after unsuccessful convertation into Number data type.

## What are classes in ES6?

They are syntactic sugar over prototypes.

## How do you copy properties from one object to other?

By using spread operator or by recursively creating deep copy.

## What is Hoisting?

Is a feature of JavaScript interpreter which allows function declarations and variables declared with `var` to be available before they are declared in the script.

## How do you assign default values to variables?

By using `||` (or) operator.

## What is the difference between Call, Apply and Bind?

Bind returns new function with new content while Call and Apply calls the function immediately. Call accepts list of arguments when Apply accepts the array of arguments.

## What is scope in javascript?

Scope is a part of the script where several variables are available.

## What is prototype chain?

Is is a sequence of prototypes which is scanned when interpreter tries to find specific property in the object.

## What is JSON and its common operations?

JSON is a universal data transaction format. It supports basic primitive types, objects and arrays and used to be an intermediate interface between different languages.

## How do you parse JSON string?

By using `JSON.parse()` method.

## What is the purpose JSON stringify?

Transforming value into JSON string for further exchange of store.

## What array methods do you know?

`.map`, `.concat`, `filter`, `.forEach`, `.reduce`, `.some`, `.every`

## What is the difference between Array.forEach() and Array.map()?

`.map` returns new array when `.forEach` does not.

## What are lambda or arrow functions?

Arrow functions is a function which inherits parent context and allows shorhand syntax for return statements.

## What is a pure function?

Pure functions is a function which does not affect outside environment and return predictable value according to the arguments input.

## What are closures?

Closure is a mechanism of catching values by the function where it was defined.

## What is IIFE(Immediately Invoked Function Expression)?

IIFE is function which executes immediately after it was defined.

## What is a callback function?

Callback functions is a function which is supplied as an argument and is supposed to be executed by parent function.

## What is a promise?

Promise is a representation of value which will appear later in time.

## Why do you need a promise?

Promises are needed to allows JavaScript process asynchronously using a single thread.

## What are the three states of promise?

Pending, fulfilled and rejected.

## Why do we need callbacks?

Callbacks are the initial implementation of asynchronous mechanism which allows to executed code after something happens.

## What is a callback hell?

Callback is a deeply nested chain of callbacks which makes code unreadable.

## What is promise chaining?

Promise chaining is a syntax of adding ordered code to promise which fill be executed after promise changes its state.

## What is the use of setTimeout?

`setTimeout` allows callback function to be executed after specified amount of time.

## What is the use of setInterval?

`setInterval` allows callback function to executed every specified amount time.

## What is an event loop?

Event loop is a architecture of JavaScript interpreter allowing it to process code asynchronously.

## What is call stack?

Call stack is a representation of functions called inside each other.

## How do you validate an email in javascript?

By using regular expressions.

## What are modules?

Module is a JavaScript file which contains `import` or `export` statements.

## Why do you need modules?

Modules are needed to decompose code into logical parts.

## What is a rest parameter?

Rest parameter is a parameter of a functions which collects all not defined arguments into array.

## What is a spread operator?

Spread operator is an operator which allows unwraping array of object.

## What is nodejs?

NodeJS is a platform which allows execution of JavaScript on platforms other than browser.
