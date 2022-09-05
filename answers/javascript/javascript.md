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

## What are the possible ways to create objects in JavaScript?

The most common way to create object is to declare it directly using curly braces.

```js
{
  foo: "bar";
}
```

Another way to create object is using contructor function with `new` keyword.

```js
const newObject = new ContructorFunction();
```

Also object can be created using `Object.create` function which accepts prototype and params.

```js
const newObject = Object.create();
```

## What are the problems with global variables?

Global variables sometimes rewrite values of each other. This can lead to uninstantional change of the value when connecting several scripts to the same page.

## How do you check whether a string contains a substring?

You can use several handy methods of the string object. `.contains()`, `.indexOf()` and `.lastIndexOf()`.

## How do you check if a key exists in an object?

You can use `.hasProperty()` or `.hasOwnProperty()` methods of the object.

## What is the main difference between Object.values and Object.entries method?

`Object.values()` return the array of values of the object when `Object.entries()` return the array consisting of array with key and value.

## How can you get the list of keys of any object?

Use can use method `Object.keys()`.

## What is a WeakSet?

Is a data structure which allows to store unique links to objects. Adding link which already exists in `WeakSet` will have no effect.

## What are the differences between WeakSet and Set?

The main differences between `Set` and `WeakSet` are that `WeakSet` can only store objects not primitive values and eliminates object if there are no other links to it.

## What is a WeakMap?

`WeakMap` operates the same way as `WeakSet` but stores data in key-value format.

## What is the difference between proto and prototype?

`__proto__` is a link to prototype of current object while `prototype` allows configuring objects created by constructur function.

## Why do you need JSON?

JSON is a unified format to send data accross different systems written in different languages.

## How do you define JSON arrays?

They are defined using brackets - the same way we define them in JavaScript. Example `[1, 2, 3]`

## What is the purpose of the array slice method?

`.slice` method allows to copy specified part of an array and return it as a new array.

## What is the purpose of the array splice method?

`.splice` modified initial array and can remove and add elements in the middle of it.

## What is a first class function?

First class functions are functions which can be manipulated as a usual object. For example, first class functions can be passed as a value to another function.

## What is a higher order function?

Higher order function is a function which accepts a functions and returns a function be modifing or extending it.

## What is a unary function?

Unary function is a function which accept only one argument.

## What is an anonymous function?

Anonymous function is a function which does not have a name and is usually used in the same place it is declared.

## What is promise.all?

`Promise.all()` is a function which accepts array of promises and return new promise which resolves when all promises are resolved. If one or the passed promises will be rejected the whole expression will be rejected too.

## What is the purpose of race method in promise?

`Promise.race()` allows to get the result of the fastest promise passed into it.

## What is a strict mode in javascript?

Strict mode is a mode which makes several JavaScript cases throw explicit error. For instance, in strict mode developer will see error when trying to access not declared variable. Strict mode is enabled by `use strict` string at the beginning of the file.

## What are PWAs?

PWA is a Progressive Web Application. PWA consits of several cutting edge technologies of web platform and usually is installable on home screen.

## How do you get the current url with javascript?

Use can use expressiong `window.location.href`.

## What is memoization?

Memoization is a caching on code level. Memoization prevents execution of complex pure function by taking result from stored data structure.

## How do you detect javascript disabled in the page?

You can place content which will be shown to the user when JS is disabled in `<noscript>` tag.

## How do you encode an URL?

By using `encodeURI()` method.

## How do you decode an URL?

By using `decodeURI()` method.
