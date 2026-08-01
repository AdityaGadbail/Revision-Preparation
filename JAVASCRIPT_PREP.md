# JavaScript Interview Questions & Answers — Complete Revision Guide

This is a complete revision guide for JavaScript interviews, covering everything from core fundamentals to advanced architectural concepts.

## 🔥 Most Asked / Tricky Questions  
- [Q: Explain the difference between `==` and `===`.](#q-explain-the-difference-between--and-)

- [Q: What is hoisting in JavaScript?](#q-what-is-hoisting-in-javascript)

- [Q: What is a closure? Provide an example.](#q-what-is-a-closure-provide-an-example)

- [Q: How do `var`, `let`, and `const` differ?](#q-how-do-var-let-and-const-differ)

- [Q: What is the event loop in JavaScript?](#q-what-is-the-event-loop-in-javascript)

- [Q: Explain the `this` keyword in JavaScript. How does its value change?](#q-explain-the-this-keyword-in-javascript-how-does-its-value-change)
- 
- [Q: How do `call`, `apply`, and `bind` work?](#q-how-do-call-apply-and-bind-work)

- [Q: What are arrow functions? What are their limitations compared to regular functions?](#q-what-are-arrow-functions-what-are-their-limitations-compared-to-regular-functions)

- [Q: Explain the concept of a prototype in JavaScript.](#q-explain-the-concept-of-a-prototype-in-javascript)

- [Q: What is the prototype chain?](#q-what-is-the-prototype-chain)

- [Q: Explain the difference between `__proto__` and `prototype`.](#q-explain-the-difference-between-__proto__-and-prototype)

- [Q: Explain the Event Loop, Call Stack, and Message Queue.](#q-explain-the-event-loop-call-stack-and-message-queue)

- [Q: What are Promises? How do they solve Callback Hell?](#q-what-are-promises-how-do-they-solve-callback-hell)

- [Q: What is `async/await`? How does it relate to Promises?](#q-what-is-asyncawait-how-does-it-relate-to-promises)

- [Q: What are the spread (`...`) and rest (`...`) operators? Explain their differences.](#q-what-are-the-spread--and-rest--operators-explain-their-differences)

- [Q: Explain Event Bubbling and Event Capturing.](#q-explain-event-bubbling-and-event-capturing)

- [Q: Explain Debouncing and Throttling. When would you use each?](#q-explain-debouncing-and-throttling-when-would-you-use-each)

- [Q: Explain LocalStorage, SessionStorage, and Cookies. What are their differences?](#q-explain-localstorage-sessionstorage-and-cookies-what-are-their-differences)

- [Q: How do you handle errors in asynchronous JavaScript?](#q-how-do-you-handle-errors-in-asynchronous-javascript)

- [Q: Implement a deep clone function for an object.](#q-implement-a-deep-clone-function-for-an-object)

---

## Table of Contents

- [JavaScript Fundamentals](#javascript-fundamentals)
  - [Q: What are the primitive data types in JavaScript?](#q-what-are-the-primitive-data-types-in-javascript)
  - [Q: Explain the difference between `null` and `undefined`.](#q-explain-the-difference-between-null-and-undefined)
  - [Q: What is type coercion in JavaScript? Provide an example.](#q-what-is-type-coercion-in-javascript-provide-an-example)
  - [Q: Explain the difference between `==` and `===`.](#q-explain-the-difference-between--and-)
  - [Q: What is hoisting in JavaScript?](#q-what-is-hoisting-in-javascript)
  - [Q: Describe the concept of scope in JavaScript (Global, Function, Block).](#q-describe-the-concept-of-scope-in-javascript-global-function-block)
  - [Q: What is a closure? Provide an example.](#q-what-is-a-closure-provide-an-example)
  - [Q: How do `var`, `let`, and `const` differ?](#q-how-do-var-let-and-const-differ)
  - [Q: What is the event loop in JavaScript?](#q-what-is-the-event-loop-in-javascript)
  - [Q: Explain the difference between pass by value and pass by reference.](#q-explain-the-difference-between-pass-by-value-and-pass-by-reference)
  - [Q: What is strict mode in JavaScript?](#q-what-is-strict-mode-in-javascript)

- [Functions & Functional Programming](#functions--functional-programming)
  - [Q: What is a first-class function?](#q-what-is-a-first-class-function)
  - [Q: What is a higher-order function? Provide an example.](#q-what-is-a-higher-order-function-provide-an-example)
  - [Q: Explain the `this` keyword in JavaScript. How does its value change?](#q-explain-the-this-keyword-in-javascript-how-does-its-value-change)
  - [Q: How do `call`, `apply`, and `bind` work?](#q-how-do-call-apply-and-bind-work)
  - [Q: What are arrow functions? What are their limitations compared to regular functions?](#q-what-are-arrow-functions-what-are-their-limitations-compared-to-regular-functions)
  - [Q: What is currying? Provide an example.](#q-what-is-currying-provide-an-example)
  - [Q: What is a pure function?](#q-what-is-a-pure-function)
  - [Q: Explain function composition.](#q-explain-function-composition)
  - [Q: What is recursion? Provide a simple example.](#q-what-is-recursion-provide-a-simple-example)
  - [Q: What is immutability in JavaScript?](#q-what-is-immutability-in-javascript)
  - [Q: What is a callback function?](#q-what-is-a-callback-function)

- [Objects, Prototypes & Classes](#objects-prototypes--classes)
  - [Q: Explain the concept of a prototype in JavaScript.](#q-explain-the-concept-of-a-prototype-in-javascript)
  - [Q: What is the prototype chain?](#q-what-is-the-prototype-chain)
  - [Q: How do you create objects in JavaScript? List several ways.](#q-how-do-you-create-objects-in-javascript-list-several-ways)
  - [Q: Explain the difference between `__proto__` and `prototype`.](#q-explain-the-difference-between-__proto__-and-prototype)
  - [Q: What are ES6 Classes? Are they truly classes?](#q-what-are-es6-classes-are-they-truly-classes)
  - [Q: How does inheritance work with ES6 Classes?](#q-how-does-inheritance-work-with-es6-classes)
  - [Q: What are getters and setters in JavaScript objects?](#q-what-are-getters-and-setters-in-javascript-objects)
  - [Q: Explain `Object.freeze()` and `Object.seal()`.](#q-explain-objectfreeze-and-objectseal)
  - [Q: What is `hasOwnProperty()`? Why is it important?](#q-what-is-hasownproperty-why-is-it-important)
  - [Q: What is the difference between `Object.keys()`, `Object.values()`, and `Object.entries()`?](#q-what-is-the-difference-between-objectkeys-objectvalues-and-objectentries)

- [Asynchronous JavaScript](#asynchronous-javascript)
  - [Q: What is asynchronous programming in JavaScript?](#q-what-is-asynchronous-programming-in-javascript)
  - [Q: Explain the Event Loop, Call Stack, and Message Queue.](#q-explain-the-event-loop-call-stack-and-message-queue)
  - [Q: What are Promises? How do they solve Callback Hell?](#q-what-are-promises-how-do-they-solve-callback-hell)
  - [Q: Explain the states of a Promise.](#q-explain-the-states-of-a-promise)
  - [Q: What is `async/await`? How does it relate to Promises?](#q-what-is-asyncawait-how-does-it-relate-to-promises)
  - [Q: What is the difference between `setTimeout` and `setInterval`?](#q-what-is-the-difference-between-settimeout-and-setinterval)
  - [Q: Explain Microtasks and Macrotasks (Task Queue vs. Microtask Queue).](#q-explain-microtasks-and-macrotasks-task-queue-vs-microtask-queue)
  - [Q: What is `Promise.all()` and `Promise.race()`? When would you use them?](#q-what-is-promiseall-and-promiserace-when-would-you-use-them)
  - [Q: How do you handle errors in asynchronous JavaScript?](#q-how-do-you-handle-errors-in-asynchronous-javascript)
  - [Q: What is `Promise.allSettled()`?](#q-what-is-promiseallsettled)
  - [Q: What is `Promise.any()`?](#q-what-is-promiseany)

- [ES6+ & Modern Features](#es6--modern-features)
  - [Q: What are `let` and `const`? How do they improve upon `var`?](#q-what-are-let-and-const-how-do-they-improve-upon-var)
  - [Q: Explain destructuring assignment in ES6. Provide examples.](#q-explain-destructuring-assignment-in-es6-provide-examples)
  - [Q: What are the spread (`...`) and rest (`...`) operators? Explain their differences.](#q-what-are-the-spread--and-rest--operators-explain-their-differences)
  - [Q: Explain ES6 Modules (`import`/`export`). Why are they important?](#q-explain-es6-modules-importexport-why-are-they-important)
  - [Q: What are Template Literals (Template Strings)?](#q-what-are-template-literals-template-strings)
  - [Q: What are default parameters in functions?](#q-what-are-default-parameters-in-functions)
  - [Q: What are `Map` and `Set` in ES6? How do they differ from plain objects/arrays?](#q-what-are-map-and-set-in-es6-how-do-they-differ-from-plain-objectsarrays)
  - [Q: Explain `for...of` and `for...in` loops. When would you use each?](#q-explain-forof-and-forin-loops-when-would-you-use-each)
  - [Q: What are Generators in JavaScript?](#q-what-are-generators-in-javascript)
  - [Q: What are Symbols in ES6?](#q-what-are-symbols-in-es6)

- [DOM Manipulation & Browser Events](#dom-manipulation--browser-events)
  - [Q: What is the DOM? How does JavaScript interact with it?](#q-what-is-the-dom-how-does-javascript-interact-with-it)
  - [Q: Explain Event Bubbling and Event Capturing.](#q-explain-event-bubbling-and-event-capturing)
  - [Q: What is Event Delegation? Why is it useful?](#q-what-is-event-delegation-why-is-it-useful)
  - [Q: How do you prevent default browser behavior and event propagation?](#q-how-do-you-prevent-default-browser-behavior-and-event-propagation)
  - [Q: What is the Shadow DOM?](#q-what-is-the-shadow-dom)
  - [Q: How do you select elements in the DOM?](#q-how-do-you-select-elements-in-the-dom)
  - [Q: What is the difference between `innerHTML`, `innerText`, and `textContent`?](#q-what-is-the-difference-between-innerhtml-innertext-and-textcontent)
  - [Q: How do you create and append a new element to the DOM?](#q-how-do-you-create-and-append-a-new-element-to-the-dom)
  - [Q: What are data attributes (`data-*`)? How do you access them in JavaScript?](#q-what-are-data-attributes-data--how-do-you-access-them-in-javascript)
  - [Q: Explain the `DOMContentLoaded` event vs. the `load` event.](#q-explain-the-domcontentloaded-event-vs-the-load-event)

- [Performance & Memory Management](#performance--memory-management)
  - [Q: What is a memory leak in JavaScript? How do they occur?](#q-what-is-a-memory-leak-in-javascript-how-do-they-occur)
  - [Q: How does Garbage Collection work in JavaScript?](#q-how-does-garbage-collection-work-in-javascript)
  - [Q: Explain Debouncing and Throttling. When would you use each?](#q-explain-debouncing-and-throttling-when-would-you-use-each)
  - [Q: What are Web Workers? Why are they useful?](#q-what-are-web-workers-why-are-they-useful)
  - [Q: How can you optimize a slow loop in JavaScript?](#q-how-can-you-optimize-a-slow-loop-in-javascript)
  - [Q: What is a DocumentFragment? How does it improve performance?](#q-what-is-a-documentfragment-how-does-it-improve-performance)
  - [Q: Explain the concept of "Reflow" and "Repaint" in the browser.](#q-explain-the-concept-of-reflow-and-repaint-in-the-browser)
  - [Q: What is the `requestAnimationFrame` API?](#q-what-is-the-requestanimationframe-api)
  - [Q: How do you identify memory leaks in a web application?](#q-how-do-you-identify-memory-leaks-in-a-web-application)

- [Web APIs & Browser Storage](#web-apis--browser-storage)
  - [Q: What is the Fetch API? How does it differ from XMLHttpRequest (XHR)?](#q-what-is-the-fetch-api-how-does-it-differ-from-xmlhttprequest-xhr)
  - [Q: Explain LocalStorage, SessionStorage, and Cookies. What are their differences?](#q-explain-localstorage-sessionstorage-and-cookies-what-are-their-differences)
  - [Q: What is the Intersection Observer API? What are its use cases?](#q-what-is-the-intersection-observer-api-what-are-its-use-cases)
  - [Q: What is the Web Storage API?](#q-what-is-the-web-storage-api)
  - [Q: Explain the concept of CORS (Cross-Origin Resource Sharing).](#q-explain-the-concept-of-cors-cross-origin-resource-sharing)
  - [Q: What are Service Workers?](#q-what-are-service-workers)
  - [Q: How do you handle JSON data in JavaScript?](#q-how-do-you-handle-json-data-in-javascript)
  - [Q: What is the Geolocation API?](#q-what-is-the-geolocation-api)

- [Testing & Error Handling](#testing--error-handling)
  - [Q: What are the different types of errors in JavaScript?](#q-what-are-the-different-types-of-errors-in-javascript)
  - [Q: How do you use `try...catch...finally` blocks?](#q-how-do-you-use-trycatchfinally-blocks)
  - [Q: How do you create custom errors in JavaScript?](#q-how-do-you-create-custom-errors-in-javascript)
  - [Q: What is the concept of Error Boundaries (in the context of UI frameworks like React, but conceptually in JS)?](#q-what-is-the-concept-of-error-boundaries-in-the-context-of-ui-frameworks-like-react-but-conceptually-in-js)
  - [Q: How do you handle global unhandled errors and promise rejections?](#q-how-do-you-handle-global-unhandled-errors-and-promise-rejections)
  - [Q: What is Jest? What are its key features?](#q-what-is-jest-what-are-its-key-features)
  - [Q: Explain the difference between Unit Testing, Integration Testing, and End-to-End (E2E) Testing.](#q-explain-the-difference-between-unit-testing-integration-testing-and-end-to-end-e2e-testing)
  - [Q: What is Test-Driven Development (TDD)?](#q-what-is-test-driven-development-tdd)

- [Coding Challenges & Polyfills](#coding-challenges--polyfills)
  - [Q: Write a polyfill for `Array.prototype.map()`.](#q-write-a-polyfill-for-arrayprototypemap)
  - [Q: Write a polyfill for `Array.prototype.filter()`.](#q-write-a-polyfill-for-arrayprototypefilter)
  - [Q: Write a polyfill for `Array.prototype.reduce()`.](#q-write-a-polyfill-for-arrayprototypereduce)
  - [Q: Implement a deep clone function for an object.](#q-implement-a-deep-clone-function-for-an-object)
  - [Q: Implement a debounce function.](#q-implement-a-debounce-function)
  - [Q: Implement a throttle function.](#q-implement-a-throttle-function)
  - [Q: Write a function to flatten a nested array.](#q-write-a-function-to-flatten-a-nested-array)
  - [Q: Write a polyfill for `Promise.all()`.](#q-write-a-polyfill-for-promiseall)

- [Design Patterns & Architecture](#design-patterns--architecture)
  - [Q: What are Design Patterns in JavaScript? Why use them?](#q-what-are-design-patterns-in-javascript-why-use-them)
  - [Q: Explain the Module Pattern.](#q-explain-the-module-pattern)
  - [Q: Explain the Singleton Pattern.](#q-explain-the-singleton-pattern)
  - [Q: Explain the Observer Pattern (Pub/Sub).](#q-explain-the-observer-pattern-pubsub)
  - [Q: Explain the Factory Pattern.](#q-explain-the-factory-pattern)
  - [Q: What is the difference between Object-Oriented Programming (OOP) and Functional Programming (FP) in JavaScript?](#q-what-is-the-difference-between-object-oriented-programming-oop-and-functional-programming-fp-in-javascript)
  - [Q: What is MVC (Model-View-Controller)?](#q-what-is-mvc-model-view-controller)

- [Behavioral & Scenario-based Questions](#behavioral--scenario-based-questions)
  - [Q: How would you debug a memory leak in a JavaScript application?](#q-how-would-you-debug-a-memory-leak-in-a-javascript-application)
  - [Q: You have a slow-rendering list of 10,000 items. How do you optimize it?](#q-you-have-a-slow-rendering-list-of-10000-items-how-do-you-optimize-it)
  - [Q: How do you handle a situation where an API request fails frequently due to network instability?](#q-how-do-you-handle-a-situation-where-an-api-request-fails-frequently-due-to-network-instability)
  - [Q: Explain how you would implement a search feature that fetches results from an API as the user types.](#q-explain-how-you-would-implement-a-search-feature-that-fetches-results-from-an-api-as-the-user-types)
  - [Q: How do you ensure your JavaScript code is secure?](#q-how-do-you-ensure-your-javascript-code-is-secure)
  - [Q: Describe a time you had to optimize the performance of a web application. What steps did you take?](#q-describe-a-time-you-had-to-optimize-the-performance-of-a-web-application-what-steps-did-you-take)

---

## JavaScript Fundamentals

### Q: What are the primitive data types in JavaScript?

**Answer:** JavaScript has seven primitive data types: `string`, `number`, `bigint`, `boolean`, `undefined`, `symbol`, and `null`. These types represent single, immutable values.

### Q: Explain the difference between `null` and `undefined`.

**Answer:** `undefined` means a variable has been declared but has not yet been assigned a value, or a property does not exist. `null` is an assignment value, meaning a variable has been explicitly assigned to have no value. `typeof undefined` is 'undefined', while `typeof null` is 'object' (a long-standing bug).

### Q: What is type coercion in JavaScript? Provide an example.

**Answer:** Type coercion is the automatic or implicit conversion of values from one data type to another. This often happens when operators are used with values of different types.**Example:**

```javascript
console.log(5 + '5'); // '55' (number 5 is coerced to string '5')
console.log(true == 1); // true (boolean true is coerced to number 1)
```

### Q: Explain the difference between `==` and `===`.

**Answer:** The `==` (loose equality) operator compares two values for equality after performing type coercion if their types are different. The `===` (strict equality) operator compares two values for equality without performing any type coercion; both the value and the type must be the same for it to return `true`.

### Q: What is hoisting in JavaScript?

**Answer:** Hoisting is a JavaScript mechanism where variable and function declarations are moved to the top of their containing scope during the compilation phase, before code execution. This means you can use variables and functions before they are declared in the code.

### Q: Describe the concept of scope in JavaScript (Global, Function, Block).

**Answer:** Scope determines the accessibility of variables, functions, and objects in some particular part of your code. **Global scope** variables are accessible from anywhere. **Function scope** variables are accessible only within the function they are declared in. **Block scope** (introduced with `let` and `const` in ES6) variables are accessible only within the block (e.g., `if` statement, `for` loop) they are declared in.

### Q: What is a closure? Provide an example.

**Answer:** A closure is the combination of a function bundled together (enclosed) with references to its surrounding state (the lexical environment). In simpler terms, a closure gives you access to an outer function's scope from an inner function, even after the outer function has finished executing.**Example:**

```javascript
function makeAdder(x) {
  return function(y) {
    return x + y;
  };
}

const addFive = makeAdder(5);
console.log(addFive(2)); // 7
```

### Q: How do `var`, `let`, and `const` differ?

**Answer:** `var` declarations are function-scoped and hoisted, allowing re-declaration and re-assignment. `let` declarations are block-scoped, hoisted (but not initialized), and allow re-assignment but not re-declaration. `const` declarations are block-scoped, hoisted (but not initialized), and do not allow re-assignment or re-declaration; they must be initialized at declaration.

### Q: What is the event loop in JavaScript?

**Answer:** The event loop is a fundamental concurrency model in JavaScript that handles asynchronous callbacks. It continuously checks if the call stack is empty. If it is, it looks into the message queue (or task queue) and pushes any pending callback functions onto the call stack for execution. This allows non-blocking I/O operations.

### Q: Explain the difference between pass by value and pass by reference.

**Answer:** In JavaScript, primitive types (string, number, boolean, null, undefined, symbol, bigint) are **passed by value**, meaning a copy of the value is passed to the function. Objects and arrays are **passed by reference** (more accurately, by sharing), meaning a copy of the reference (memory address) to the object is passed. Changes made to the object inside the function will affect the original object.

### Q: What is strict mode in JavaScript?

**Answer:** Strict mode (`'use strict';`) is a way to opt into a restricted variant of JavaScript. It eliminates some JavaScript silent errors by changing them to throw errors, fixes mistakes that make it difficult for JavaScript engines to perform optimizations, and prohibits some syntax likely to be defined in future versions of ECMAScript. It can be applied to entire scripts or individual functions.

---

## Functions & Functional Programming

### Q: What is a first-class function?

**Answer:** In JavaScript, functions are first-class citizens, meaning they can be treated like any other variable. They can be assigned to variables, passed as arguments to other functions, and returned as values from other functions.

### Q: What is a higher-order function? Provide an example.

**Answer:** A higher-order function (HOF) is a function that either takes one or more functions as arguments or returns a function as its result. HOFs are a cornerstone of functional programming.**Example:**

```javascript
function greet(name) {
  return function(message) {
    console.log(`${message}, ${name}!`);
  };
}

const greetJohn = greet("John");
greetJohn("Hello"); // Hello, John!

// Or using a function as an argument
const numbers = [1, 2, 3];
const doubled = numbers.map(num => num * 2); // map is a HOF
console.log(doubled); // [2, 4, 6]
```

### Q: Explain the `this` keyword in JavaScript. How does its value change?

**Answer:** The `this` keyword refers to the context in which a function is executed. Its value is determined by how the function is called. In a global context, `this` refers to the global object (e.g., `window` in browsers). In a method, `this` refers to the object that owns the method. In an event handler, `this` refers to the element that received the event. Arrow functions have lexical `this`, meaning they inherit `this` from their enclosing scope.

### Q: How do `call`, `apply`, and `bind` work?

**Answer:** `call`, `apply`, and `bind` are methods on `Function.prototype` used to explicitly set the `this` context of a function.

- `call()` invokes the function immediately with a specified `this` value and arguments passed individually.

- `apply()` invokes the function immediately with a specified `this` value and arguments passed as an array.

- `bind()` returns a *new* function with a `this` context permanently bound to a specified value, but does not invoke it immediately.**Example:**

```javascript
const person = { name: "Alice" };

function sayHello(greeting) {
  console.log(`${greeting}, ${this.name}!`);
}

sayHello.call(person, "Hi"); // Hi, Alice!
sayHello.apply(person, ["Hello"]); // Hello, Alice!

const boundSayHello = sayHello.bind(person, "Hey");
boundSayHello(); // Hey, Alice!
```

### Q: What are arrow functions? What are their limitations compared to regular functions?

**Answer:** Arrow functions (`=>`) provide a more concise syntax for writing function expressions. They do not have their own `this`, `arguments`, `super`, or `new.target` bindings, inheriting them from the enclosing lexical scope. This makes them unsuitable for methods that need their own `this` context (e.g., object methods, constructor functions) or for functions that need the `arguments` object.

### Q: What is currying? Provide an example.

**Answer:** Currying is a functional programming technique where a function that takes multiple arguments is transformed into a sequence of functions, each taking a single argument. It allows for partial application of arguments.**Example:**

```javascript
function multiply(a, b, c) {
  return a * b * c;
}

// Curried version
const curriedMultiply = (a) => (b) => (c) => a * b * c;

console.log(curriedMultiply(2)(3)(4)); // 24

const multiplyBySix = curriedMultiply(2)(3);
console.log(multiplyBySix(10)); // 60
```

### Q: What is a pure function?

**Answer:** A pure function is a function that, given the same input, will always return the same output and produces no side effects. Side effects include modifying external state, performing I/O operations, or mutating arguments. Pure functions are predictable, testable, and easier to reason about.

### Q: Explain function composition.

**Answer:** Function composition is the act of combining multiple functions to produce a new function. The result of one function is passed as the argument to the next function, creating a pipeline of operations. It promotes reusability and readability.**Example:**

```javascript
const addOne = (num) => num + 1;
const multiplyByTwo = (num) => num * 2;

const compose = (...fns) => (x) => fns.reduceRight((acc, fn) => fn(acc), x);

const addOneThenMultiplyByTwo = compose(multiplyByTwo, addOne);
console.log(addOneThenMultiplyByTwo(5)); // (5 + 1) * 2 = 12
```

### Q: What is recursion? Provide a simple example.

**Answer:** Recursion is a programming technique where a function calls itself to solve a problem. A recursive function must have a base case (a condition to stop the recursion) and a recursive step (where the function calls itself with a modified input).**Example:**

```javascript
function factorial(n) {
  if (n === 0) { // Base case
    return 1;
  }
  return n * factorial(n - 1); // Recursive step
}

console.log(factorial(5)); // 120
```

### Q: What is immutability in JavaScript?

**Answer:** Immutability means that once an object or primitive is created, it cannot be changed. Instead of modifying an existing value, a new value is created. This is particularly important for objects and arrays to prevent unexpected side effects and make state management more predictable, especially in complex applications. Methods like `map()`, `filter()`, `slice()`, and the spread operator (`...`) help achieve immutability with arrays and objects.

### Q: What is a callback function?

**Answer:** A callback function is a function passed into another function as an argument, which is then invoked inside the outer function to complete some kind of routine or action. Callbacks are commonly used to handle asynchronous operations, such as network requests or event handling.**Example:**

```javascript
function fetchData(callback) {
  setTimeout(() => {
    const data = "Data fetched!";
    callback(data);
  }, 1000);
}

function displayData(message) {
  console.log(message);
}

fetchData(displayData); // Data fetched! (after 1 second)
```

---

## Objects, Prototypes & Classes

### Q: Explain the concept of a prototype in JavaScript.

**Answer:** In JavaScript, every object has a prototype, which is another object that it inherits properties and methods from. This forms a prototype chain, allowing objects to inherit features from other objects. When you try to access a property or method on an object, JavaScript first looks on the object itself, then on its prototype, then on its prototype's prototype, and so on, until it finds the property or reaches the end of the chain (which is `null`).

### Q: What is the prototype chain?

**Answer:** The prototype chain is a mechanism in JavaScript that allows objects to inherit properties and methods from other objects. When an object is created, it gets a link to its prototype object. If a property or method is not found directly on the object, JavaScript traverses up this chain, checking each prototype in sequence until the property is found or the chain ends. This is how inheritance works in JavaScript.

### Q: How do you create objects in JavaScript? List several ways.

**Answer:** There are several ways to create objects:

1. **Object Literal:** `const obj = { key: 'value' };`

1. **`new Object()`****:** `const obj = new Object(); obj.key = 'value';`

1. **Constructor Function:**

   ```javascript
   function Person(name) {
     this.name = name;
   }
   const person1 = new Person('Alice');
   ```

1. **`Object.create()`****:** `const proto = { greet: function() { console.log('Hello'); } }; const obj = Object.create(proto);`

1. **ES6 Classes:**

   ```javascript
   class Car {
     constructor(make) {
       this.make = make;
     }
   }
   const myCar = new Car('Toyota');
   ```

### Q: Explain the difference between `__proto__` and `prototype`.

**Answer:**

- `__proto__` (dunder proto) is an internal property of an object that points to its prototype (the object from which it inherits properties). It's a non-standard but widely supported way to access an object's prototype.

- `prototype` is a property of *constructor functions* (and classes) that points to the object that will be set as the `__proto__` of instances created by that constructor/class. It's used to define properties and methods that will be inherited by all instances.

### Q: What are ES6 Classes? Are they truly classes?

**Answer:** ES6 Classes are a syntactic sugar over JavaScript's existing prototype-based inheritance. They provide a cleaner and more familiar syntax for creating objects and handling inheritance, similar to class-based languages like Java or C++. However, under the hood, they still use prototypes and the prototype chain. So, while they look like traditional classes, they are not truly class-based in the same way other languages are.

### Q: How does inheritance work with ES6 Classes?

**Answer:** ES6 Classes use the `extends` keyword to establish inheritance between classes. A `child` class can `extend` a `parent` class, inheriting its methods and properties. The `super()` keyword is used within the child class's constructor to call the parent class's constructor, ensuring that the parent's initialization logic is executed and `this` is correctly bound.**Example:**

```javascript
class Animal {
  constructor(name) {
    this.name = name;
  }
  speak() {
    console.log(`${this.name} makes a sound.`);
  }
}

class Dog extends Animal {
  constructor(name, breed) {
    super(name);
    this.breed = breed;
  }
  speak() {
    console.log(`${this.name} barks.`);
  }
}

const myDog = new Dog('Buddy', 'Golden Retriever');
myDog.speak(); // Buddy barks.
```

### Q: What are getters and setters in JavaScript objects?

**Answer:** Getters and setters are special methods that allow you to define object properties that are accessed like regular properties but execute a function when read (getter) or written to (setter). They provide a way to control access to an object's properties, allowing for validation, computation, or side effects when a property is accessed or modified.**Example:**

```javascript
const person = {
  firstName: 'John',
  lastName: 'Doe',
  get fullName() {
    return `${this.firstName} ${this.lastName}`;
  },
  set fullName(name) {
    const parts = name.split(' ');
    this.firstName = parts[0];
    this.lastName = parts[1];
  }
};

console.log(person.fullName); // John Doe
person.fullName = 'Jane Smith';
console.log(person.firstName); // Jane
```

### Q: Explain `Object.freeze()` and `Object.seal()`.

**Answer:**

- `Object.freeze()` prevents new properties from being added to an object, existing properties from being removed, and existing properties (including enumerable, configurable, and writable attributes) from being changed. It also prevents the prototype from being changed. The object becomes immutable.

- `Object.seal()` prevents new properties from being added to an object and marks all existing properties as non-configurable. However, existing properties can still be changed (their values can be updated) as long as they are writable. It's less strict than `freeze()`.

### Q: What is `hasOwnProperty()`? Why is it important?

**Answer:** The `hasOwnProperty()` method returns a boolean indicating whether the object has the specified property as its own property (not inherited). It's important because it allows you to distinguish between an object's own properties and those inherited from its prototype chain. This is crucial when iterating over object properties (e.g., with `for...in` loops) to avoid processing inherited properties.**Example:**

```javascript
const obj = { a: 1 };
const inheritedObj = Object.create(obj);
inheritedObj.b = 2;

console.log(inheritedObj.hasOwnProperty('b')); // true
console.log(inheritedObj.hasOwnProperty('a')); // false (inherited)
```

### Q: What is the difference between `Object.keys()`, `Object.values()`, and `Object.entries()`?

**Answer:** These are static methods on the `Object` constructor that return arrays of an object's *own enumerable string-keyed properties*:

- `Object.keys(obj)`: Returns an array of a given object's own enumerable property *names*.

- `Object.values(obj)`: Returns an array of a given object's own enumerable property *values*.

- `Object.entries(obj)`: Returns an array of a given object's own enumerable string-keyed property `[key, value]` pairs.**Example:**

```javascript
const myObject = { a: 1, b: 2, c: 3 };
console.log(Object.keys(myObject));   // ['a', 'b', 'c']
console.log(Object.values(myObject)); // [1, 2, 3]
console.log(Object.entries(myObject)); // [['a', 1], ['b', 2], ['c', 3]]
```

---

## Asynchronous JavaScript

### Q: What is asynchronous programming in JavaScript?

**Answer:** Asynchronous programming in JavaScript allows operations to run independently of the main program flow, without blocking the execution of other code. This is crucial for tasks like network requests, file I/O, or timers, which can take time to complete. Instead of waiting, JavaScript can continue executing other code and handle the result of the asynchronous operation once it's ready, typically using callbacks, Promises, or async/await.

### Q: Explain the Event Loop, Call Stack, and Message Queue.

**Answer:** These are core components of JavaScript's concurrency model:

- **Call Stack:** A LIFO (Last In, First Out) stack that stores function calls. When a function is called, it's pushed onto the stack; when it returns, it's popped off.

- **Message Queue (or Task Queue):** A FIFO (First In, First Out) queue that stores messages (callbacks) associated with asynchronous operations (e.g., `setTimeout`, DOM events, network responses) that are ready to be executed.

- **Event Loop:** Continuously monitors the Call Stack and the Message Queue. If the Call Stack is empty, it takes the first message (callback) from the Message Queue and pushes it onto the Call Stack for execution.

### Q: What are Promises? How do they solve Callback Hell?

**Answer:** Promises are objects that represent the eventual completion (or failure) of an asynchronous operation and its resulting value. They provide a cleaner, more structured way to handle asynchronous code compared to traditional callbacks, especially when dealing with multiple sequential asynchronous operations. Promises help avoid Callback Hell (or Pyramid of Doom) by allowing you to chain asynchronous operations using `.then()` and handle errors with `.catch()`.

### Q: Explain the states of a Promise.

**Answer:** A Promise can be in one of three states:

1. **Pending:** Initial state, neither fulfilled nor rejected.

1. **Fulfilled (Resolved):** Meaning that the operation completed successfully.

1. **Rejected:** Meaning that the operation failed.Once a Promise is fulfilled or rejected, it is said to be *settled* and its state cannot change again.

### Q: What is `async/await`? How does it relate to Promises?

**Answer:** `async/await` is a modern JavaScript syntax built on top of Promises that allows you to write asynchronous code that looks and behaves more like synchronous code. An `async` function always returns a Promise. The `await` keyword can only be used inside an `async` function and pauses the execution of the `async` function until the Promise it's waiting for settles (resolves or rejects).**Example:**

```javascript
async function fetchData() {
  try {
    const response = await fetch("https://api.example.com/data" );
    const data = await response.json();
    console.log(data);
  } catch (error) {
    console.error("Error fetching data:", error);
  }
}
fetchData();
```

### Q: What is the difference between `setTimeout` and `setInterval`?

**Answer:** Both `setTimeout` and `setInterval` are used to schedule code execution after a certain delay, but they differ in their behavior:

- `setTimeout(callback, delay)`: Executes the `callback` function *once* after the specified `delay` (in milliseconds).

- `setInterval(callback, delay)`: Executes the `callback` function *repeatedly* every `delay` milliseconds, until cleared with `clearInterval()`.

### Q: Explain Microtasks and Macrotasks (Task Queue vs. Microtask Queue).

**Answer:** JavaScript's event loop manages two types of queues for asynchronous operations:

- **Macrotasks (Task Queue):** Includes `setTimeout`, `setInterval`, I/O operations, UI rendering, etc. The event loop processes one macrotask at a time, then empties the microtask queue before picking the next macrotask.

- **Microtasks (Microtask Queue):** Includes Promise callbacks (`.then()`, `.catch()`, `.finally()`), `queueMicrotask`, and `MutationObserver`. The event loop empties the entire microtask queue *after* each macrotask and *before* rendering or processing the next macrotask. This means microtasks have higher priority than macrotasks.

### Q: What is `Promise.all()` and `Promise.race()`? When would you use them?

**Answer:** Both are static methods on the `Promise` object for handling multiple promises concurrently:

- `Promise.all(iterable)`: Takes an iterable of Promises as input and returns a single Promise. This returned Promise fulfills when *all* of the input Promises have fulfilled, or rejects as soon as *any* of the input Promises rejects. Use it when you need all results to proceed.

- `Promise.race(iterable)`: Takes an iterable of Promises as input and returns a single Promise. This returned Promise fulfills or rejects as soon as *any* of the input Promises fulfills or rejects, with the value or reason from that Promise. Use it when you only care about the first Promise to settle.

### Q: How do you handle errors in asynchronous JavaScript?

**Answer:** Error handling in asynchronous JavaScript depends on the mechanism used:

- **Callbacks:** Errors are typically passed as the first argument to the callback function (Node.js style `(err, data)`).

- **Promises:** Errors are handled using the `.catch()` method or by providing a second callback to `.then()`. Uncaught promise rejections can be handled globally with `window.addEventListener('unhandledrejection')`.

- **`async/await`****:** Errors are handled using standard `try...catch` blocks, similar to synchronous code, which makes error handling much cleaner.

### Q: What is `Promise.allSettled()`?

**Answer:** `Promise.allSettled(iterable)` takes an iterable of Promises and returns a single Promise that fulfills when *all* of the input Promises have settled (either fulfilled or rejected). The returned Promise resolves with an array of objects, each describing the outcome of a Promise (e.g., `{ status: 'fulfilled', value: result }` or `{ status: 'rejected', reason: error }`). This is useful when you want to know the outcome of every Promise, regardless of whether it succeeded or failed.

### Q: What is `Promise.any()`?

**Answer:** `Promise.any(iterable)` takes an iterable of Promises and returns a single Promise. This returned Promise fulfills as soon as *any* of the input Promises fulfills, with the value of that Promise. If all of the input Promises reject, then the returned Promise rejects with an `AggregateError` containing an array of all the rejection reasons. It's useful when you need the first successful result, and don't care about failures unless all fail.

---

## ES6+ & Modern Features

### Q: What are `let` and `const`? How do they improve upon `var`?

**Answer:** `let` and `const` are block-scoped variable declarations introduced in ES6, addressing issues with `var`'s function-scoping and hoisting behavior. `let` allows re-assignment but not re-declaration within the same scope, while `const` prevents both re-assignment and re-declaration, making it suitable for values that should not change. They improve code clarity, prevent accidental variable re-declarations, and reduce bugs related to variable scope and hoisting.

### Q: Explain destructuring assignment in ES6. Provide examples.

**Answer:** Destructuring assignment is a powerful ES6 feature that allows you to unpack values from arrays or properties from objects into distinct variables. It provides a concise way to extract data.**Example (Array Destructuring):**

```javascript
const numbers = [1, 2, 3];
const [a, b] = numbers;
console.log(a, b); // 1 2

// With rest pattern
const [first, ...rest] = numbers;
console.log(first, rest); // 1 [2, 3]
```

**Example (Object Destructuring):**

```javascript
const person = { name: 'Alice', age: 30 };
const { name, age } = person;
console.log(name, age); // Alice 30

// With alias and default value
const { name: fullName, city = 'New York' } = person;
console.log(fullName, city); // Alice New York
```

### Q: What are the spread (`...`) and rest (`...`) operators? Explain their differences.

**Answer:** Both use the `...` syntax but serve different purposes based on where they are used:

- **Spread Operator:** Used to expand an iterable (like an array or string) into individual elements, or to expand an object into key-value pairs. It's used when *calling* a function or creating new arrays/objects.**Example (Spread):**

   ```javascript
   const arr1 = [1, 2];
   const arr2 = [...arr1, 3, 4]; // [1, 2, 3, 4]
   const obj1 = { a: 1, b: 2 };
   const obj2 = { ...obj1, c: 3 }; // { a: 1, b: 2, c: 3 }
   ```

- **Rest Parameter:** Used to collect an indefinite number of arguments into an array. It's used in *function definitions* or array/object destructuring to gather remaining elements.**Example (Rest):**

   ```javascript
   function sum(...args) {
     return args.reduce((acc, val) => acc + val, 0);
   }
   console.log(sum(1, 2, 3, 4)); // 10
   
   const [first, ...remaining] = [1, 2, 3, 4];
   console.log(first, remaining); // 1 [2, 3, 4]
   ```

### Q: Explain ES6 Modules (`import`/`export`). Why are they important?

**Answer:** ES6 Modules provide a standardized way to organize JavaScript code into separate, reusable files. They allow you to `export` functions, classes, or variables from one file and `import` them into another. Key benefits include:

- **Modularity:** Better code organization and separation of concerns.

- **Encapsulation:** Variables and functions are private by default within a module unless explicitly exported.

- **Dependency Management:** Clear declaration of dependencies.

- **Performance:** Can be statically analyzed, enabling tree-shaking (removing unused code) and better optimization by bundlers.

### Q: What are Template Literals (Template Strings)?

**Answer:** Template literals are string literals allowing embedded expressions, multi-line strings, and string interpolation. They are enclosed by backticks (```) instead of single or double quotes.**Example:**

```javascript
const name = 'World';
const greeting = `Hello, ${name}!\nWelcome to multi-line strings.`;
console.log(greeting);
```

### Q: What are default parameters in functions?

**Answer:** Default parameters allow you to initialize a function parameter with a default value if an argument is not provided or is `undefined` when the function is called. This simplifies function signatures and reduces the need for manual checks inside the function body.**Example:**

```javascript
function greet(name = 'Guest') {
  console.log(`Hello, ${name}!`);
}
greet();        // Hello, Guest!
greet('Alice'); // Hello, Alice!
```

### Q: What are `Map` and `Set` in ES6? How do they differ from plain objects/arrays?

**Answer:**

- **`Map`****:** A collection of key-value pairs where keys can be of any data type (including objects or functions), unlike plain objects where keys must be strings or Symbols. `Map` maintains the insertion order of elements and provides methods like `set()`, `get()`, `has()`, `delete()`, and `size`.

- **`Set`****:** A collection of unique values. It allows you to store any type of value, whether primitive or object. `Set` provides methods like `add()`, `has()`, `delete()`, and `size`. It's useful for removing duplicates from an array or checking for the presence of an item.

### Q: Explain `for...of` and `for...in` loops. When would you use each?

**Answer:**

- **`for...in`**** loop:** Iterates over the *enumerable properties* of an object. It returns the *keys* (property names) as strings. It's generally not recommended for iterating over arrays because it can iterate over inherited properties and the order is not guaranteed.**Example (****`for...in`****):**

   ```javascript
   const obj = { a: 1, b: 2 };
   for (const key in obj) {
     console.log(key, obj[key]); // a 1, b 2
   }
   ```

- **`for...of`**** loop:** Iterates over the *values* of iterable objects (like Arrays, Strings, Maps, Sets, NodeLists, etc.). It returns the actual values, not the keys/indices. It's the preferred way to iterate over arrays and other iterable collections.**Example (`for...of`):}

   ```javascript
   const arr = [1, 2, 3];
   for (const value of arr) {
     console.log(value); // 1, 2, 3
   }
   ```

### Q: What are Generators in JavaScript?

**Answer:** Generators are special functions that can be paused and resumed, allowing them to produce a sequence of values over time rather than computing them all at once. They are defined using `function*` syntax and use the `yield` keyword to pause execution and return a value. When a generator function is called, it returns an iterator object, which can be used to control its execution (`.next()`). Generators are useful for implementing iterators, asynchronous programming, and infinite data streams.**Example:**

```javascript
function* idGenerator() {
  let id = 1;
  while (true) {
    yield id++;
  }
}

const gen = idGenerator();
console.log(gen.next().value); // 1
console.log(gen.next().value); // 2
```

### Q: What are Symbols in ES6?

**Answer:** Symbols are a new primitive data type introduced in ES6. They are unique and immutable values that can be used as object property keys. The primary purpose of Symbols is to create unique property keys that won't clash with other property keys, especially when adding properties to objects that you don't own or when implementing mixins. They are not enumerable by default.**Example:**

```javascript
const id = Symbol('id');
const user = {
  name: 'John',
  [id]: 123
};

console.log(user[id]); // 123
for (let key in user) {
  console.log(key); // Only 'name' is logged
}
```

---

## DOM Manipulation & Browser Events

### Q: What is the DOM? How does JavaScript interact with it?

**Answer:** The Document Object Model (DOM) is a programming interface for web documents. It represents the page structure as a tree of objects, where each node represents a part of the document (e.g., elements, attributes, text). JavaScript interacts with the DOM to dynamically change the content, structure, and style of a web page. It provides methods to select elements, modify their properties, add or remove elements, and handle events.

### Q: Explain Event Bubbling and Event Capturing.

**Answer:** These are two ways event propagation works in the DOM when an event occurs on an element that is nested inside other elements:

- **Event Capturing (Trickling Down):** The event starts from the `window` object, then goes down through the parent elements to the target element. This phase is rarely used in practice.

- **Event Bubbling (Bubbling Up):** The event starts at the target element and then propagates upwards through its parent elements to the `window` object. This is the default behavior for most events.

### Q: What is Event Delegation? Why is it useful?

**Answer:** Event delegation is a technique where you attach a single event listener to a parent element, instead of attaching individual listeners to multiple child elements. When an event bubbles up from a child element, the parent listener catches it. You can then determine which child element triggered the event using `event.target` and react accordingly. It's useful for:

- **Performance:** Reduces the number of event listeners, especially for large lists or dynamically added elements.

- **Dynamic Elements:** Automatically handles events for elements added to the DOM after the initial page load.

- **Memory Efficiency:** Less memory consumption as fewer listeners are created.

### Q: How do you prevent default browser behavior and event propagation?

**Answer:**

- **`event.preventDefault()`****:** Stops the default action of an event from happening. For example, preventing a form submission or a link from navigating.

- **`event.stopPropagation()`****:** Prevents the event from bubbling up (or capturing down) to parent (or child) elements. The event will only be handled by the current element and any listeners attached to it.

- **`event.stopImmediatePropagation()`****:** Prevents other listeners on the *same* element from being called, and also stops the event from bubbling up (or capturing down).

### Q: What is the Shadow DOM?

**Answer:** The Shadow DOM is a web standard that allows for component-based encapsulation in the DOM. It enables you to attach a hidden, separate DOM tree to an element, which is rendered along with the main document DOM. This encapsulation ensures that styles and scripts within the Shadow DOM do not leak out and affect the rest of the page, and vice versa. It's a key technology for building Web Components.

### Q: How do you select elements in the DOM?

**Answer:** JavaScript provides several methods to select DOM elements:

- `document.getElementById('id')`: Selects a single element by its ID.

- `document.getElementsByClassName('class')`: Returns an HTMLCollection of elements with the specified class.

- `document.getElementsByTagName('tag')`: Returns an HTMLCollection of elements with the specified tag name.

- `document.querySelector('selector')`: Returns the *first* element that matches a CSS selector.

- `document.querySelectorAll('selector')`: Returns a NodeList of *all* elements that match a CSS selector.

### Q: What is the difference between `innerHTML`, `innerText`, and `textContent`?

**Answer:**

- `innerHTML`: Gets or sets the HTML markup contained within an element. It parses the string as HTML, which can be a security risk (XSS) if used with unsanitized user input.

- `innerText`: Gets or sets the visible text content of an element and its descendants. It respects CSS styling (e.g., ignores hidden elements) and triggers a reflow when read.

- `textContent`: Gets or sets the text content of an element and all its descendants, regardless of CSS styling. It's generally faster than `innerText` because it doesn't trigger a reflow and is safer than `innerHTML` for plain text.

### Q: How do you create and append a new element to the DOM?

**Answer:** You can create and append elements using DOM manipulation methods:

1. Create the element: `const newDiv = document.createElement('div');`

1. Set its content or attributes: `newDiv.textContent = 'Hello World'; newDiv.className = 'my-class';`

1. Select the parent element: `const parent = document.getElementById('container');`

1. Append the new element: `parent.appendChild(newDiv);` (or `parent.append(newDiv)` for multiple nodes/strings).

### Q: What are data attributes (`data-*`)? How do you access them in JavaScript?

**Answer:** Data attributes allow you to store custom data directly on HTML elements. They are prefixed with `data-` (e.g., `data-user-id="123"`). In JavaScript, you can access them using the `dataset` property of the element. The `data-` prefix is removed, and the remaining part is converted to camelCase.**Example:**

```html
<div id="user" data-user-id="123" data-role="admin">User Info</div>
```

```javascript
const userDiv = document.getElementById('user');
console.log(userDiv.dataset.userId); // "123"
console.log(userDiv.dataset.role);   // "admin"
```

### Q: Explain the `DOMContentLoaded` event vs. the `load` event.

**Answer:**

- `DOMContentLoaded`: Fires when the initial HTML document has been completely loaded and parsed, without waiting for stylesheets, images, and subframes to finish loading. This is usually the best time to run DOM manipulation scripts.

- `load`: Fires when the whole page has loaded, including all dependent resources such as stylesheets and images. It's useful when you need to interact with elements that depend on external resources (e.g., getting the dimensions of an image).

---

## Performance & Memory Management

### Q: What is a memory leak in JavaScript? How do they occur?

**Answer:** A memory leak occurs when a piece of memory that is no longer needed by the application is not released back to the operating system. In JavaScript, this happens when objects are still referenced by the application, preventing the garbage collector from freeing them. Common causes include:

- Accidental global variables.

- Forgotten timers or callbacks (e.g., `setInterval` not cleared).

- Closures holding onto large objects unnecessarily.

- Detached DOM elements (elements removed from the DOM but still referenced in JavaScript).

### Q: How does Garbage Collection work in JavaScript?

**Answer:** JavaScript uses automatic garbage collection to manage memory. The most common algorithm is **Mark-and-Sweep**. It works by periodically starting from a set of "roots" (like global variables and the current call stack) and "marking" all objects that are reachable from these roots. Any object that is not marked is considered unreachable and its memory is "swept" (reclaimed).

### Q: Explain Debouncing and Throttling. When would you use each?

**Answer:** Both are techniques to control the rate at which a function is executed, often used for performance optimization with frequent events (like scrolling, resizing, or typing).

- **Debouncing:** Ensures a function is only executed *after* a certain amount of time has passed since it was last invoked. If the event occurs again before the time is up, the timer resets. Use it for tasks like search input suggestions (wait until the user stops typing).

- **Throttling:** Ensures a function is executed *at most once* in a specified time interval, regardless of how many times the event is triggered. Use it for tasks like tracking scroll position or handling window resize events.

### Q: What are Web Workers? Why are they useful?

**Answer:** Web Workers provide a way to run JavaScript code in background threads, separate from the main execution thread of a web application. This is crucial for performance because it allows you to perform computationally intensive tasks (like complex calculations or data processing) without blocking the main thread, keeping the UI responsive. Workers communicate with the main thread via a messaging system (`postMessage` and `onmessage`).

### Q: How can you optimize a slow loop in JavaScript?

**Answer:** Optimizing loops involves reducing the work done inside the loop and minimizing overhead:

- Cache array length: `for (let i = 0, len = arr.length; i < len; i++)` instead of checking `arr.length` every iteration.

- Use appropriate loop types: `for` loops are generally faster than `forEach` or `map` for simple iterations, though modern engines have optimized array methods significantly.

- Minimize DOM manipulation inside the loop: Build a string or DocumentFragment and append it to the DOM once after the loop finishes.

- Avoid creating functions inside the loop.

- Consider Web Workers for heavy computations.

### Q: What is a DocumentFragment? How does it improve performance?

**Answer:** A `DocumentFragment` is a lightweight, minimal document object that has no parent. It's used as a temporary container to hold DOM nodes. When you append a DocumentFragment to the DOM, only its children are inserted, not the fragment itself. It improves performance because changes made to a DocumentFragment do not trigger reflows or repaints in the main document. You can build a complex DOM structure in the fragment and then append it to the document in a single operation, minimizing performance overhead.

### Q: Explain the concept of "Reflow" and "Repaint" in the browser.

**Answer:**

- **Reflow (or Layout):** Occurs when the browser needs to recalculate the positions and geometries of elements in the document. This happens when you change properties that affect layout (e.g., width, height, margin, padding, font size, adding/removing elements). Reflows are computationally expensive.

- **Repaint:** Occurs when changes are made to an element's appearance that do not affect its layout (e.g., changing color, background-color, visibility). Repaints are less expensive than reflows but still consume resources.Optimizing performance often involves minimizing reflows and repaints, for example, by batching DOM changes or using CSS classes instead of inline styles.

### Q: What is the `requestAnimationFrame` API?

**Answer:** `requestAnimationFrame` is a browser API used for creating smooth animations. It tells the browser that you wish to perform an animation and requests that the browser call a specified function to update an animation before the next repaint. It's more efficient than using `setTimeout` or `setInterval` because it synchronizes with the browser's refresh rate (usually 60fps), preventing frame dropping and reducing CPU usage when the tab is inactive.

### Q: How do you identify memory leaks in a web application?

**Answer:** You can identify memory leaks using browser developer tools (like Chrome DevTools):

- **Performance Tab:** Record a timeline and look for a "sawtooth" pattern in memory usage that continuously grows over time without returning to a baseline.

- **Memory Tab (Heap Snapshots):** Take heap snapshots at different points in time and compare them to see which objects are accumulating and not being garbage collected. Look for detached DOM nodes or large arrays/objects that shouldn't exist.

- **Allocation Timelines:** Track memory allocations in real-time to pinpoint which functions are creating objects that aren't being cleaned up.

---

## Web APIs & Browser Storage

### Q: What is the Fetch API? How does it differ from XMLHttpRequest (XHR)?

**Answer:** The Fetch API provides a modern, Promise-based interface for making network requests (e.g., fetching resources across the network). It's a cleaner and more powerful alternative to the older `XMLHttpRequest` (XHR). Key differences:

- Fetch uses Promises, making asynchronous code easier to read and write (especially with `async/await`).

- Fetch does not send cross-origin cookies by default (unless configured).

- Fetch won't reject the Promise on HTTP error statuses (like 404 or 500); it only rejects on network failure. You must check the `response.ok` property.

### Q: Explain LocalStorage, SessionStorage, and Cookies. What are their differences?

**Answer:** These are mechanisms for storing data on the client-side:

- **LocalStorage:** Stores data with no expiration date. Data persists even when the browser is closed and reopened. Capacity is typically around 5-10MB per origin. Data is not sent to the server with every request.

- **SessionStorage:** Stores data for the duration of the page session. Data is cleared when the page or tab is closed. Capacity is similar to LocalStorage. Data is not sent to the server.

- **Cookies:** Small pieces of data (up to 4KB) sent to the server with every HTTP request. They can have expiration dates and are often used for authentication, session management, and tracking. They are less secure for sensitive data unless configured properly (e.g., HttpOnly, Secure flags).

### Q: What is the Intersection Observer API? What are its use cases?

**Answer:** The Intersection Observer API provides a way to asynchronously observe changes in the intersection of a target element with an ancestor element or with a top-level document's viewport. It's highly performant because it doesn't rely on scroll events or continuous polling.**Use cases:**

- Lazy loading images or other content as they scroll into view.

- Implementing "infinite scrolling" web pages.

- Reporting visibility of advertisements for calculating ad revenues.

- Triggering animations when elements become visible.

### Q: What is the Web Storage API?

**Answer:** The Web Storage API provides mechanisms by which browsers can store key/value pairs, in a much more intuitive fashion than using cookies. It encompasses both `localStorage` and `sessionStorage`. The keys and values are always strings (you must serialize objects using `JSON.stringify()` before storing and parse them with `JSON.parse()` when retrieving).

### Q: Explain the concept of CORS (Cross-Origin Resource Sharing).

**Answer:** CORS is a security mechanism implemented by browsers that restricts web pages from making requests to a different domain (origin) than the one that served the web page. This is known as the Same-Origin Policy. CORS allows servers to specify which origins are permitted to access their resources by sending specific HTTP headers (e.g., `Access-Control-Allow-Origin`). If the server doesn't provide the correct headers, the browser blocks the request.

### Q: What are Service Workers?

**Answer:** Service Workers are scripts that run in the background, separate from a web page, opening the door to features that don't need a web page or user interaction. They act as a proxy server that sits between web applications, the browser, and the network. They are primarily used for:

- Offline experiences (caching assets and API responses).

- Background sync.

- Push notifications.They require HTTPS for security reasons.

### Q: How do you handle JSON data in JavaScript?

**Answer:** JavaScript provides the built-in `JSON` object to handle JSON (JavaScript Object Notation) data:

- `JSON.parse(jsonString)`: Parses a JSON string and constructs the JavaScript value or object described by the string.

- `JSON.stringify(value)`: Converts a JavaScript object or value to a JSON string.**Example:**

```javascript
const obj = { name: "Alice", age: 30 };
const jsonString = JSON.stringify(obj); // '{"name":"Alice","age":30}'
const parsedObj = JSON.parse(jsonString); // { name: 'Alice', age: 30 }
```

### Q: What is the Geolocation API?

**Answer:** The Geolocation API allows the user to provide their location to web applications if they so desire. For privacy reasons, the user is asked for permission to report location information. It provides methods like `navigator.geolocation.getCurrentPosition()` to get the current location and `navigator.geolocation.watchPosition()` to track location changes.

---

## Testing & Error Handling

### Q: What are the different types of errors in JavaScript?

**Answer:** Common error types in JavaScript include:

- **SyntaxError:** Occurs when the code violates the syntax rules of the language (e.g., missing a parenthesis).

- **ReferenceError:** Occurs when trying to access a variable that has not been declared.

- **TypeError:** Occurs when a value is not of the expected type (e.g., calling a method on `undefined` or `null`).

- **RangeError:** Occurs when a numeric variable or parameter is outside of its valid range.

- **URIError:** Occurs when `encodeURI()` or `decodeURI()` are used incorrectly.

### Q: How do you use `try...catch...finally` blocks?

**Answer:** The `try...catch...finally` statement handles exceptions (errors) in JavaScript.

- **`try`****:** Contains the code that might throw an error.

- **`catch`****:** Contains the code that executes if an error is thrown in the `try` block. It receives the error object as an argument.

- **`finally`****:** Contains code that executes regardless of whether an error was thrown or caught. It's often used for cleanup tasks (e.g., closing a file or network connection).**Example:**

```javascript
try {
  // Code that might throw an error
  const result = riskyOperation();
} catch (error) {
  // Handle the error
  console.error("An error occurred:", error.message);
} finally {
  // Always executes
  console.log("Operation finished.");
}
```

### Q: How do you create custom errors in JavaScript?

**Answer:** You can create custom errors by extending the built-in `Error` class. This allows you to define specific error types for your application, making error handling more precise.**Example:**

```javascript
class ValidationError extends Error {
  constructor(message) {
    super(message);
    this.name = "ValidationError";
  }
}

function validateAge(age) {
  if (age < 0) {
    throw new ValidationError("Age cannot be negative.");
  }
  return true;
}
```

### Q: What is the concept of Error Boundaries (in the context of UI frameworks like React, but conceptually in JS)?

**Answer:** While Error Boundaries are a specific feature in React, the concept applies generally: it's a mechanism to catch JavaScript errors anywhere in a component tree (or application module), log those errors, and display a fallback UI instead of crashing the entire application. In plain JavaScript, this might involve wrapping main application entry points or specific modules in robust `try...catch` blocks or global error handlers to prevent a single failure from taking down the whole system.

### Q: How do you handle global unhandled errors and promise rejections?

**Answer:** You can catch errors that slip through `try...catch` blocks using global event listeners on the `window` object:

- **`window.onerror`**** or ****`window.addEventListener('error', ...)`****:** Catches unhandled synchronous errors and errors in event handlers.

- **`window.addEventListener('unhandledrejection', ...)`****:** Catches unhandled Promise rejections (when a Promise rejects but there is no `.catch()` handler).

### Q: What is Jest? What are its key features?

**Answer:** Jest is a popular JavaScript testing framework maintained by Meta (Facebook). It's widely used for testing React applications but works well with plain JavaScript, Node.js, Vue, and Angular. Key features include:

- **Zero configuration:** Works out of the box for most JavaScript projects.

- **Snapshots:** Allows you to capture the state of a UI component or object and compare it in future tests to detect unintended changes.

- **Mocking:** Built-in support for mocking functions, modules, and timers.

- **Code Coverage:** Built-in code coverage reports.

- **Parallel testing:** Runs tests in parallel for faster execution.

### Q: Explain the difference between Unit Testing, Integration Testing, and End-to-End (E2E) Testing.

**Answer:**

- **Unit Testing:** Tests individual, isolated units of code (e.g., a single function or class) to ensure they work correctly in isolation.

- **Integration Testing:** Tests how different units or modules work together. It verifies the interactions between components.

- **End-to-End (E2E) Testing:** Tests the entire application flow from start to finish, simulating real user scenarios in a browser environment (e.g., using tools like Cypress or Playwright).

### Q: What is Test-Driven Development (TDD)?

**Answer:** TDD is a software development process where you write tests *before* writing the actual code. The cycle is typically:

1. **Red:** Write a failing test for a new feature.

1. **Green:** Write the minimum amount of code necessary to make the test pass.

1. **Refactor:** Improve the code while ensuring the tests still pass.TDD helps ensure code quality, better design, and comprehensive test coverage.

---

## Coding Challenges & Polyfills

### Q: Write a polyfill for `Array.prototype.map()`.

**Answer:**

```javascript
if (!Array.prototype.myMap) {
  Array.prototype.myMap = function(callback, thisArg) {
    if (this == null) throw new TypeError('this is null or not defined');
    if (typeof callback !== 'function') throw new TypeError(callback + ' is not a function');
    
    const O = Object(this);
    const len = O.length >>> 0;
    const A = new Array(len);
    
    for (let k = 0; k < len; k++) {
      if (k in O) {
        A[k] = callback.call(thisArg, O[k], k, O);
      }
    }
    return A;
  };
}
```

### Q: Write a polyfill for `Array.prototype.filter()`.

**Answer:**

```javascript
if (!Array.prototype.myFilter) {
  Array.prototype.myFilter = function(callback, thisArg) {
    if (this == null) throw new TypeError('this is null or not defined');
    if (typeof callback !== 'function') throw new TypeError(callback + ' is not a function');
    
    const O = Object(this);
    const len = O.length >>> 0;
    const res = [];
    
    for (let i = 0; i < len; i++) {
      if (i in O) {
        const val = O[i];
        if (callback.call(thisArg, val, i, O)) {
          res.push(val);
        }
      }
    }
    return res;
  };
}
```

### Q: Write a polyfill for `Array.prototype.reduce()`.

**Answer:**

```javascript
if (!Array.prototype.myReduce) {
  Array.prototype.myReduce = function(callback, initialValue) {
    if (this == null) throw new TypeError('this is null or not defined');
    if (typeof callback !== 'function') throw new TypeError(callback + ' is not a function');
    
    const O = Object(this);
    const len = O.length >>> 0;
    let k = 0;
    let accumulator;
    
    if (arguments.length >= 2) {
      accumulator = initialValue;
    } else {
      while (k < len && !(k in O)) {
        k++;
      }
      if (k >= len) throw new TypeError('Reduce of empty array with no initial value');
      accumulator = O[k++];
    }
    
    while (k < len) {
      if (k in O) {
        accumulator = callback(accumulator, O[k], k, O);
      }
      k++;
    }
    return accumulator;
  };
}
```

### Q: Implement a deep clone function for an object.

**Answer:** A simple `JSON.parse(JSON.stringify(obj))` works for basic objects but fails with functions, Dates, undefined, or circular references. A robust recursive approach is needed.

```javascript
function deepClone(obj, hash = new WeakMap()) {
  if (obj === null || typeof obj !== 'object') return obj;
  if (obj instanceof Date) return new Date(obj);
  if (obj instanceof RegExp) return new RegExp(obj);
  
  if (hash.has(obj)) return hash.get(obj); // Handle circular references
  
  const clone = Array.isArray(obj) ? [] : {};
  hash.set(obj, clone);
  
  for (let key in obj) {
    if (Object.prototype.hasOwnProperty.call(obj, key)) {
      clone[key] = deepClone(obj[key], hash);
    }
  }
  return clone;
}
```

### Q: Implement a debounce function.

**Answer:**

```javascript
function debounce(func, delay) {
  let timeoutId;
  return function(...args) {
    const context = this;
    clearTimeout(timeoutId);
    timeoutId = setTimeout(() => {
      func.apply(context, args);
    }, delay);
  };
}
```

### Q: Implement a throttle function.

**Answer:**

```javascript
function throttle(func, limit) {
  let inThrottle;
  return function(...args) {
    const context = this;
    if (!inThrottle) {
      func.apply(context, args);
      inThrottle = true;
      setTimeout(() => inThrottle = false, limit);
    }
  };
}
```

### Q: Write a function to flatten a nested array.

**Answer:**

```javascript
// Using recursion
function flattenArray(arr) {
  return arr.reduce((acc, val) => 
    Array.isArray(val) ? acc.concat(flattenArray(val)) : acc.concat(val), []
  );
}

// Using ES6 flat() (if allowed)
// const flattened = arr.flat(Infinity);
```

### Q: Write a polyfill for `Promise.all()`.

**Answer:**

```javascript
function myPromiseAll(promises) {
  return new Promise((resolve, reject) => {
    if (!Array.isArray(promises)) {
      return reject(new TypeError('Argument must be an array'));
    }
    
    const results = [];
    let completedCount = 0;
    
    if (promises.length === 0) {
      return resolve(results);
    }
    
    promises.forEach((promise, index) => {
      Promise.resolve(promise)
        .then(value => {
          results[index] = value;
          completedCount++;
          if (completedCount === promises.length) {
            resolve(results);
          }
        })
        .catch(error => {
          reject(error);
        });
    });
  });
}
```

---

## Design Patterns & Architecture

### Q: What are Design Patterns in JavaScript? Why use them?

**Answer:** Design patterns are reusable, proven solutions to common problems in software design. They are not finished code, but templates or blueprints for solving a problem in a specific context. Using them helps write code that is more maintainable, scalable, and easier to understand, as they provide a shared vocabulary for developers.

### Q: Explain the Module Pattern.

**Answer:** The Module Pattern is used to encapsulate "private" variables and functions, exposing only a public API. Before ES6 modules, this was typically achieved using an IIFE (Immediately Invoked Function Expression) and closures. It helps prevent global namespace pollution.**Example:**

```javascript
const myModule = (function() {
  let privateVar = 'I am private';
  
  function privateMethod() {
    console.log(privateVar);
  }
  
  return {
    publicMethod: function() {
      privateMethod();
    }
  };
})();

myModule.publicMethod(); // Logs: I am private
// myModule.privateVar is undefined
```

### Q: Explain the Singleton Pattern.

**Answer:** The Singleton Pattern ensures that a class has only one instance and provides a global point of access to it. It's useful for managing shared resources, like a configuration object, a database connection, or a state store.**Example:**

```javascript
class Database {
  constructor() {
    if (Database.instance) {
      return Database.instance;
    }
    this.connection = 'Connected';
    Database.instance = this;
  }
}

const db1 = new Database();
const db2 = new Database();
console.log(db1 === db2); // true
```

### Q: Explain the Observer Pattern (Pub/Sub).

**Answer:** The Observer Pattern defines a one-to-many dependency between objects so that when one object (the subject/publisher) changes state, all its dependents (observers/subscribers) are notified and updated automatically. It's heavily used in event handling and state management (like Redux).**Example:**

```javascript
class Subject {
  constructor() {
    this.observers = [];
  }
  subscribe(observer) {
    this.observers.push(observer);
  }
  unsubscribe(observer) {
    this.observers = this.observers.filter(obs => obs !== observer);
  }
  notify(data) {
    this.observers.forEach(observer => observer(data));
  }
}
```

### Q: Explain the Factory Pattern.

**Answer:** The Factory Pattern is a creational pattern that provides an interface for creating objects in a superclass, but allows subclasses to alter the type of objects that will be created. It abstracts the object creation process, making it easier to manage complex object instantiation logic.**Example:**

```javascript
class Car { constructor() { this.type = 'Car'; } }
class Truck { constructor() { this.type = 'Truck'; } }

class VehicleFactory {
  createVehicle(type) {
    switch(type) {
      case 'car': return new Car();
      case 'truck': return new Truck();
      default: throw new Error('Unknown vehicle type');
    }
  }
}
```

### Q: What is the difference between Object-Oriented Programming (OOP) and Functional Programming (FP) in JavaScript?

**Answer:**

- **OOP:** Focuses on modeling the system as a collection of objects that contain both data (state) and behavior (methods). It relies on concepts like classes, inheritance, encapsulation, and polymorphism. State is often mutable.

- **FP:** Focuses on building software by composing pure functions, avoiding shared state, mutable data, and side effects. It relies on concepts like first-class functions, higher-order functions, immutability, and declarative code. JavaScript supports both paradigms.

### Q: What is MVC (Model-View-Controller)?

**Answer:** MVC is an architectural pattern that separates an application into three main logical components:

- **Model:** Manages the data, logic, and rules of the application.

- **View:** Handles the UI and presentation of the data.

- **Controller:** Accepts input, converts it to commands for the Model or View, and acts as an intermediary between them.

---

## Behavioral & Scenario-based Questions

### Q: How would you debug a memory leak in a JavaScript application?

**Answer:** I would start by using the browser's DevTools (e.g., Chrome DevTools). First, I'd use the Performance tab to record a timeline and look for a sawtooth pattern in memory usage that doesn't return to a baseline, indicating a leak. Then, I'd use the Memory tab to take Heap Snapshots at different points in time. By comparing these snapshots, I can identify objects that are accumulating and not being garbage collected. I'd look for detached DOM nodes, large arrays, or closures holding onto references unnecessarily. Once identified, I'd trace the allocation stack to find the code responsible and fix the reference issue.

### Q: You have a slow-rendering list of 10,000 items. How do you optimize it?

**Answer:** Rendering 10,000 DOM nodes at once will freeze the browser. I would optimize this using **Virtualization (or Windowing)**. Instead of rendering all items, I would only render the items currently visible in the viewport, plus a small buffer above and below. As the user scrolls, I would dynamically replace the DOM nodes with new data, reusing the existing elements. Libraries like `react-window` or `react-virtualized` do this. Alternatively, if virtualization isn't possible, I'd use pagination or an "infinite scroll" approach to load data in smaller chunks.

### Q: How do you handle a situation where an API request fails frequently due to network instability?

**Answer:** I would implement a **retry mechanism with exponential backoff**. If a request fails, the application shouldn't immediately retry, as it might overwhelm the server or fail again. Instead, it should wait a short time (e.g., 1 second), then retry. If it fails again, wait longer (e.g., 2 seconds, then 4 seconds), up to a maximum number of retries. I would also ensure the user is informed of the issue with a graceful error message and perhaps a manual "Retry" button if the automatic retries fail.

### Q: Explain how you would implement a search feature that fetches results from an API as the user types.

**Answer:** To prevent making an API call for every single keystroke (which would overload the server and cause race conditions), I would use **debouncing**. I'd wrap the API call function in a debounce function with a delay of, say, 300ms. This ensures the API is only called after the user has stopped typing for 300ms. Additionally, I would need to handle race conditions (where an older request resolves after a newer one) by either aborting previous requests using the `AbortController` API or by keeping track of the latest request ID and ignoring responses from older IDs.

### Q: How do you ensure your JavaScript code is secure?

**Answer:** Security involves several practices:

- **Preventing XSS (Cross-Site Scripting):** Never trust user input. Always sanitize and escape data before rendering it in the DOM (avoiding `innerHTML` when possible, using `textContent` instead).

- **Preventing CSRF (Cross-Site Request Forgery):** Use anti-CSRF tokens for state-changing requests.

- **Using HTTPS:** Ensure all data transmission is encrypted.

- **Dependency Management:** Regularly audit and update npm packages to patch known vulnerabilities (using `npm audit`).

- **Avoiding ****`eval()`****:** Never use `eval()` or `new Function()` with untrusted input, as it can execute malicious code.

### Q: Describe a time you had to optimize the performance of a web application. What steps did you take?

**Answer:** *(This requires a personal anecdote, but a good structure is:)* "In a previous project, the initial load time was very slow. I started by running Lighthouse audits to identify bottlenecks. I found that we were serving large, unoptimized images and a massive JavaScript bundle. I implemented image compression and lazy loading for images below the fold. For the JavaScript, I implemented code splitting using Webpack, so we only loaded the code necessary for the initial route. I also moved some heavy data processing to a Web Worker. These changes reduced the Time to Interactive (TTI) by 50%."

---

## How to Use This Guide

- **Daily Revision:** Try to cover one or two sections per day to avoid feeling overwhelmed.

- **Mock Interviews:** Have a friend ask you these questions, or practice answering them out loud to yourself.

- **Code Practice:** Don't just read the coding challenges; write them out in a code editor or on a whiteboard to build muscle memory.

- **Quick Lookup:** Use `Ctrl+F` (or `Cmd+F`) to quickly find specific topics or keywords you need to brush up on right before an interview.

---

## Table of Contents

- [JavaScript Fundamentals](#javascript-fundamentals)
  - [Q: What are the primitive data types in JavaScript?](#q-what-are-the-primitive-data-types-in-javascript)
  - [Q: Explain the difference between `null` and `undefined`.](#q-explain-the-difference-between-null-and-undefined)
  - [Q: What is type coercion in JavaScript? Provide an example.](#q-what-is-type-coercion-in-javascript-provide-an-example)
  - [Q: Explain the difference between `==` and `===`.](#q-explain-the-difference-between--and-)
  - [Q: What is hoisting in JavaScript?](#q-what-is-hoisting-in-javascript)
  - [Q: Describe the concept of scope in JavaScript (Global, Function, Block).](#q-describe-the-concept-of-scope-in-javascript-global-function-block)
  - [Q: What is a closure? Provide an example.](#q-what-is-a-closure-provide-an-example)
  - [Q: How do `var`, `let`, and `const` differ?](#q-how-do-var-let-and-const-differ)
  - [Q: What is the event loop in JavaScript?](#q-what-is-the-event-loop-in-javascript)
  - [Q: Explain the difference between pass by value and pass by reference.](#q-explain-the-difference-between-pass-by-value-and-pass-by-reference)
  - [Q: What is strict mode in JavaScript?](#q-what-is-strict-mode-in-javascript)

- [Functions & Functional Programming](#functions--functional-programming)
  - [Q: What is a first-class function?](#q-what-is-a-first-class-function)
  - [Q: What is a higher-order function? Provide an example.](#q-what-is-a-higher-order-function-provide-an-example)
  - [Q: Explain the `this` keyword in JavaScript. How does its value change?](#q-explain-the-this-keyword-in-javascript-how-does-its-value-change)
  - [Q: How do `call`, `apply`, and `bind` work?](#q-how-do-call-apply-and-bind-work)
  - [Q: What are arrow functions? What are their limitations compared to regular functions?](#q-what-are-arrow-functions-what-are-their-limitations-compared-to-regular-functions)
  - [Q: What is currying? Provide an example.](#q-what-is-currying-provide-an-example)
  - [Q: What is a pure function?](#q-what-is-a-pure-function)
  - [Q: Explain function composition.](#q-explain-function-composition)
  - [Q: What is recursion? Provide a simple example.](#q-what-is-recursion-provide-a-simple-example)
  - [Q: What is immutability in JavaScript?](#q-what-is-immutability-in-javascript)
  - [Q: What is a callback function?](#q-what-is-a-callback-function)

- [Objects, Prototypes & Classes](#objects-prototypes--classes)

- [Asynchronous JavaScript](#asynchronous-javascript)

- [ES6+ & Modern Features](#es6--modern-features)

- [DOM Manipulation & Browser Events](#dom-manipulation--browser-events)

- [Performance & Memory Management](#performance--memory-management)

- [Web APIs & Browser Storage](#web-apis--browser-storage)

- [Testing & Error Handling](#testing--error-handling)

- [Coding Challenges & Polyfills](#coding-challenges--polyfills)

- [Design Patterns & Architecture](#design-patterns--architecture)

- [Behavioral & Scenario-based Questions](#behavioral--scenario-based-questions)

---

## JavaScript Fundamentals

### Q: What are the primitive data types in JavaScript?

**Answer:** JavaScript has seven primitive data types: `string`, `number`, `bigint`, `boolean`, `undefined`, `symbol`, and `null`. These types represent single, immutable values.

### Q: Explain the difference between `null` and `undefined`.

**Answer:** `undefined` means a variable has been declared but has not yet been assigned a value, or a property does not exist. `null` is an assignment value, meaning a variable has been explicitly assigned to have no value. `typeof undefined` is 'undefined', while `typeof null` is 'object' (a long-standing bug).

### Q: What is type coercion in JavaScript? Provide an example.

**Answer:** Type coercion is the automatic or implicit conversion of values from one data type to another. This often happens when operators are used with values of different types.**Example:**

```javascript
console.log(5 + '5'); // '55' (number 5 is coerced to string '5')
console.log(true == 1); // true (boolean true is coerced to number 1)
```

### Q: Explain the difference between `==` and `===`.

**Answer:** The `==` (loose equality) operator compares two values for equality after performing type coercion if their types are different. The `===` (strict equality) operator compares two values for equality without performing any type coercion; both the value and the type must be the same for it to return `true`.

### Q: What is hoisting in JavaScript?

**Answer:** Hoisting is a JavaScript mechanism where variable and function declarations are moved to the top of their containing scope during the compilation phase, before code execution. This means you can use variables and functions before they are declared in the code.

### Q: Describe the concept of scope in JavaScript (Global, Function, Block).

**Answer:** Scope determines the accessibility of variables, functions, and objects in some particular part of your code. **Global scope** variables are accessible from anywhere. **Function scope** variables are accessible only within the function they are declared in. **Block scope** (introduced with `let` and `const` in ES6) variables are accessible only within the block (e.g., `if` statement, `for` loop) they are declared in.

### Q: What is a closure? Provide an example.

**Answer:** A closure is the combination of a function bundled together (enclosed) with references to its surrounding state (the lexical environment). In simpler terms, a closure gives you access to an outer function's scope from an inner function, even after the outer function has finished executing.**Example:**

```javascript
function makeAdder(x) {
  return function(y) {
    return x + y;
  };
}

const addFive = makeAdder(5);
console.log(addFive(2)); // 7
```

### Q: How do `var`, `let`, and `const` differ?

**Answer:** `var` declarations are function-scoped and hoisted, allowing re-declaration and re-assignment. `let` declarations are block-scoped, hoisted (but not initialized), and allow re-assignment but not re-declaration. `const` declarations are block-scoped, hoisted (but not initialized), and do not allow re-assignment or re-declaration; they must be initialized at declaration.

### Q: What is the event loop in JavaScript?

**Answer:** The event loop is a fundamental concurrency model in JavaScript that handles asynchronous callbacks. It continuously checks if the call stack is empty. If it is, it looks into the message queue (or task queue) and pushes any pending callback functions onto the call stack for execution. This allows non-blocking I/O operations.

### Q: Explain the difference between pass by value and pass by reference.

**Answer:** In JavaScript, primitive types (string, number, boolean, null, undefined, symbol, bigint) are **passed by value**, meaning a copy of the value is passed to the function. Objects and arrays are **passed by reference** (more accurately, by sharing), meaning a copy of the reference (memory address) to the object is passed. Changes made to the object inside the function will affect the original object.

### Q: What is strict mode in JavaScript?

**Answer:** Strict mode (`'use strict';`) is a way to opt into a restricted variant of JavaScript. It eliminates some JavaScript silent errors by changing them to throw errors, fixes mistakes that make it difficult for JavaScript engines to perform optimizations, and prohibits some syntax likely to be defined in future versions of ECMAScript. It can be applied to entire scripts or individual functions.

---

## Functions & Functional Programming

### Q: What is a first-class function?

**Answer:** In JavaScript, functions arefirst-class citizens, meaning they can be treated like any other variable. They can be assigned to variables, passed as arguments to other functions, and returned as values from other functions.

### Q: What is a higher-order function? Provide an example.

**Answer:** A higher-order function (HOF) is a function that either takes one or more functions as arguments or returns a function as its result. HOFs are a cornerstone of functional programming.**Example:**

```javascript
function greet(name) {
  return function(message) {
    console.log(`${message}, ${name}!`);
  };
}

const greetJohn = greet("John");
greetJohn("Hello"); // Hello, John!

// Or using a function as an argument
const numbers = [1, 2, 3];
const doubled = numbers.map(num => num * 2); // map is a HOF
console.log(doubled); // [2, 4, 6]
```

### Q: Explain the `this` keyword in JavaScript. How does its value change?

**Answer:** The `this` keyword refers to the context in which a function is executed. Its value is determined by how the function is called. In a global context, `this` refers to the global object (e.g., `window` in browsers). In a method, `this` refers to the object that owns the method. In an event handler, `this` refers to the element that received the event. Arrow functions have lexical `this`, meaning they inherit `this` from their enclosing scope.

### Q: How do `call`, `apply`, and `bind` work?

**Answer:** `call`, `apply`, and `bind` are methods on `Function.prototype` used to explicitly set the `this` context of a function.

- `call()` invokes the function immediately with a specified `this` value and arguments passed individually.

- `apply()` invokes the function immediately with a specified `this` value and arguments passed as an array.

- `bind()` returns a *new* function with a `this` context permanently bound to a specified value, but does not invoke it immediately.**Example:**

```javascript
const person = { name: "Alice" };

function sayHello(greeting) {
  console.log(`${greeting}, ${this.name}!`);
}

sayHello.call(person, "Hi"); // Hi, Alice!
sayHello.apply(person, ["Hello"]); // Hello, Alice!

const boundSayHello = sayHello.bind(person, "Hey");
boundSayHello(); // Hey, Alice!
```

### Q: What are arrow functions? What are their limitations compared to regular functions?

**Answer:** Arrow functions (`=>`) provide a more concise syntax for writing function expressions. They do not have their own `this`, `arguments`, `super`, or `new.target` bindings, inheriting them from the enclosing lexical scope. This makes them unsuitable for methods that need their own `this` context (e.g., object methods, constructor functions) or for functions that need the `arguments` object.

### Q: What is currying? Provide an example.

**Answer:** Currying is a functional programming technique where a function that takes multiple arguments is transformed into a sequence of functions, each taking a single argument. It allows for partial application of arguments.**Example:**

```javascript
function multiply(a, b, c) {
  return a * b * c;
}

// Curried version
const curriedMultiply = (a) => (b) => (c) => a * b * c;

console.log(curriedMultiply(2)(3)(4)); // 24

const multiplyBySix = curriedMultiply(2)(3);
console.log(multiplyBySix(10)); // 60
```

### Q: What is a pure function?

**Answer:** A pure function is a function that, given the same input, will always return the same output and produces no side effects. Side effects include modifying external state, performing I/O operations, or mutating arguments. Pure functions are predictable, testable, and easier to reason about.

### Q: Explain function composition.

**Answer:** Function composition is the act of combining multiple functions to produce a new function. The result of one function is passed as the argument to the next function, creating a pipeline of operations. It promotes reusability and readability.**Example:**

```javascript
const addOne = (num) => num + 1;
const multiplyByTwo = (num) => num * 2;

const compose = (...fns) => (x) => fns.reduceRight((acc, fn) => fn(acc), x);

const addOneThenMultiplyByTwo = compose(multiplyByTwo, addOne);
console.log(addOneThenMultiplyByTwo(5)); // (5 + 1) * 2 = 12
```

### Q: What is recursion? Provide a simple example.

**Answer:** Recursion is a programming technique where a function calls itself to solve a problem. A recursive function must have a base case (a condition to stop the recursion) and a recursive step (where the function calls itself with a modified input).**Example:**

```javascript
function factorial(n) {
  if (n === 0) { // Base case
    return 1;
  }
  return n * factorial(n - 1); // Recursive step
}

console.log(factorial(5)); // 120
```

### Q: What is immutability in JavaScript?

**Answer:** Immutability means that once an object or primitive is created, it cannot be changed. Instead of modifying an existing value, a new value is created. This is particularly important for objects and arrays to prevent unexpected side effects and make state management more predictable, especially in complex applications. Methods like `map()`, `filter()`, `slice()`, and the spread operator (`...`) help achieve immutability with arrays and objects.

### Q: What is a callback function?

**Answer:** A callback function is a function passed into another function as an argument, which is then invoked inside the outer function to complete some kind of routine or action. Callbacks are commonly used to handle asynchronous operations, such as network requests or event handling.**Example:**

```javascript
function fetchData(callback) {
  setTimeout(() => {
    const data = "Data fetched!";
    callback(data);
  }, 1000);
}

function displayData(message) {
  console.log(message);
}

fetchData(displayData); // Data fetched! (after 1 second)
```

---

## Objects, Prototypes & Classes

### Q: Explain the concept of a prototype in JavaScript.

**Answer:** In JavaScript, every object has a prototype, which is another object that it inherits properties and methods from. This forms a prototype chain, allowing objects to inherit features from other objects. When you try to access a property or method on an object, JavaScript first looks on the object itself, then on its prototype, then on its prototype's prototype, and so on, until it finds the property or reaches the end of the chain (which is `null`).

### Q: What is the prototype chain?

**Answer:** The prototype chain is a mechanism in JavaScript that allows objects to inherit properties and methods from other objects. When an object is created, it gets a link to its prototype object. If a property or method is not found directly on the object, JavaScript traverses up this chain, checking each prototype in sequence until the property is found or the chain ends. This is how inheritance works in JavaScript.

### Q: How do you create objects in JavaScript? List several ways.

**Answer:** There are several ways to create objects:

1. **Object Literal:** `const obj = { key: 'value' };`

1. **`new Object()`****:** `const obj = new Object(); obj.key = 'value';`

1. **Constructor Function:**

   ```javascript
   function Person(name) {
     this.name = name;
   }
   const person1 = new Person('Alice');
   ```

1. **`Object.create()`****:** `const proto = { greet: function() { console.log('Hello'); } }; const obj = Object.create(proto);`

1. **ES6 Classes:**

   ```javascript
   class Car {
     constructor(make) {
       this.make = make;
     }
   }
   const myCar = new Car('Toyota');
   ```

### Q: Explain the difference between `__proto__` and `prototype`.

**Answer:**

- `__proto__` (dunder proto) is an internal property of an object that points to its prototype (the object from which it inherits properties). It's a non-standard but widely supported way to access an object's prototype.

- `prototype` is a property of *constructor functions* (and classes) that points to the object that will be set as the `__proto__` of instances created by that constructor/class. It's used to define properties and methods that will be inherited by all instances.

### Q: What are ES6 Classes? Are they truly classes?

**Answer:** ES6 Classes are a syntactic sugar over JavaScript's existing prototype-based inheritance. They provide a cleaner and more familiar syntax for creating objects and handling inheritance, similar to class-based languages like Java or C++. However, under the hood, they still use prototypes and the prototype chain. So, while they look like traditional classes, they are not truly class-based in the same way other languages are.

### Q: How does inheritance work with ES6 Classes?

**Answer:** ES6 Classes use the `extends` keyword to establish inheritance between classes. A `child` class can `extend` a `parent` class, inheriting its methods and properties. The `super()` keyword is used within the child class's constructor to call the parent class's constructor, ensuring that the parent's initialization logic is executed and `this` is correctly bound.**Example:**

```javascript
class Animal {
  constructor(name) {
    this.name = name;
  }
  speak() {
    console.log(`${this.name} makes a sound.`);
  }
}

class Dog extends Animal {
  constructor(name, breed) {
    super(name);
    this.breed = breed;
  }
  speak() {
    console.log(`${this.name} barks.`);
  }
}

const myDog = new Dog('Buddy', 'Golden Retriever');
myDog.speak(); // Buddy barks.
```

### Q: What are getters and setters in JavaScript objects?

**Answer:** Getters and setters are special methods that allow you to define object properties that are accessed like regular properties but execute a function when read (getter) or written to (setter). They provide a way to control access to an object's properties, allowing for validation, computation, or side effects when a property is accessed or modified.**Example:**

```javascript
const person = {
  firstName: 'John',
  lastName: 'Doe',
  get fullName() {
    return `${this.firstName} ${this.lastName}`;
  },
  set fullName(name) {
    const parts = name.split(' ');
    this.firstName = parts[0];
    this.lastName = parts[1];
  }
};

console.log(person.fullName); // John Doe
person.fullName = 'Jane Smith';
console.log(person.firstName); // Jane
```

### Q: Explain `Object.freeze()` and `Object.seal()`.

**Answer:**

- `Object.freeze()` prevents new properties from being added to an object, existing properties from being removed, and existing properties (including enumerable, configurable, and writable attributes) from being changed. It also prevents the prototype from being changed. The object becomes immutable.

- `Object.seal()` prevents new properties from being added to an object and marks all existing properties as non-configurable. However, existing properties can still be changed (their values can be updated) as long as they are writable. It's less strict than `freeze()`.

### Q: What is `hasOwnProperty()`? Why is it important?

**Answer:** The `hasOwnProperty()` method returns a boolean indicating whether the object has the specified property as its own property (not inherited). It's important because it allows you to distinguish between an object's own properties and those inherited from its prototype chain. This is crucial when iterating over object properties (e.g., with `for...in` loops) to avoid processing inherited properties.**Example:**

```javascript
const obj = { a: 1 };
const inheritedObj = Object.create(obj);
inheritedObj.b = 2;

console.log(inheritedObj.hasOwnProperty('b')); // true
console.log(inheritedObj.hasOwnProperty('a')); // false (inherited)
```

### Q: What is the difference between `Object.keys()`, `Object.values()`, and `Object.entries()`?

**Answer:** These are static methods on the `Object` constructor that return arrays of an object's *own enumerable string-keyed properties*:

- `Object.keys(obj)`: Returns an array of a given object's own enumerable property *names*.

- `Object.values(obj)`: Returns an array of a given object's own enumerable property *values*.

- `Object.entries(obj)`: Returns an array of a given object's own enumerable string-keyed property `[key, value]` pairs.**Example:**

```javascript
const myObject = { a: 1, b: 2, c: 3 };
console.log(Object.keys(myObject));   // ['a', 'b', 'c']
console.log(Object.values(myObject)); // [1, 2, 3]
console.log(Object.entries(myObject)); // [['a', 1], ['b', 2], ['c', 3]]
```

---

## Asynchronous JavaScript

### Q: What is asynchronous programming in JavaScript?

**Answer:** Asynchronous programming in JavaScript allows operations to run independently of the main program flow, without blocking the execution of other code. This is crucial for tasks like network requests, file I/O, or timers, which can take time to complete. Instead of waiting, JavaScript can continue executing other code and handle the result of the asynchronous operation once it's ready, typically using callbacks, Promises, or async/await.

### Q: Explain the Event Loop, Call Stack, and Message Queue.

**Answer:** These are core components of JavaScript's concurrency model:

- **Call Stack:** A LIFO (Last In, First Out) stack that stores function calls. When a function is called, it's pushed onto the stack; when it returns, it's popped off.

- **Message Queue (or Task Queue):** A FIFO (First In, First Out) queue that stores messages (callbacks) associated with asynchronous operations (e.g., `setTimeout`, DOM events, network responses) that are ready to be executed.

- **Event Loop:** Continuously monitors the Call Stack and the Message Queue. If the Call Stack is empty, it takes the first message (callback) from the Message Queue and pushes it onto the Call Stack for execution.

### Q: What are Promises? How do they solve Callback Hell?

**Answer:** Promises are objects that represent the eventual completion (or failure) of an asynchronous operation and its resulting value. They provide a cleaner, more structured way to handle asynchronous code compared to traditional callbacks, especially when dealing with multiple sequential asynchronous operations. Promises help avoidCallback Hell (or Pyramid of Doom) by allowing you to chain asynchronous operations using `.then()` and handle errors with `.catch()`.

### Q: Explain the states of a Promise.

**Answer:** A Promise can be in one of three states:

1. **Pending:** Initial state, neither fulfilled nor rejected.

1. **Fulfilled (Resolved):** Meaning that the operation completed successfully.

1. **Rejected:** Meaning that the operation failed.Once a Promise is fulfilled or rejected, it is said to be *settled* and its state cannot change again.

### Q: What is `async/await`? How does it relate to Promises?

**Answer:** `async/await` is a modern JavaScript syntax built on top of Promises that allows you to write asynchronous code that looks and behaves more like synchronous code. An `async` function always returns a Promise. The `await` keyword can only be used inside an `async` function and pauses the execution of the `async` function until the Promise it's waiting for settles (resolves or rejects).**Example:**

```javascript
async function fetchData() {
  try {
    const response = await fetch("https://api.example.com/data" );
    const data = await response.json();
    console.log(data);
  } catch (error) {
    console.error("Error fetching data:", error);
  }
}
fetchData();
```

### Q: What is the difference between `setTimeout` and `setInterval`?

**Answer:** Both `setTimeout` and `setInterval` are used to schedule code execution after a certain delay, but they differ in their behavior:

- `setTimeout(callback, delay)`: Executes the `callback` function *once* after the specified `delay` (in milliseconds).

- `setInterval(callback, delay)`: Executes the `callback` function *repeatedly* every `delay` milliseconds, until cleared with `clearInterval()`.

### Q: Explain Microtasks and Macrotasks (Task Queue vs. Microtask Queue).

**Answer:** JavaScript's event loop manages two types of queues for asynchronous operations:

- **Macrotasks (Task Queue):** Includes `setTimeout`, `setInterval`, I/O operations, UI rendering, etc. The event loop processes one macrotask at a time, then empties the microtask queue before picking the next macrotask.

- **Microtasks (Microtask Queue):** Includes Promise callbacks (`.then()`, `.catch()`, `.finally()`), `queueMicrotask`, and `MutationObserver`. The event loop empties the entire microtask queue *after* each macrotask and *before* rendering or processing the next macrotask. This means microtasks have higher priority than macrotasks.

### Q: What is `Promise.all()` and `Promise.race()`? When would you use them?

**Answer:** Both are static methods on the `Promise` object for handling multiple promises concurrently:

- `Promise.all(iterable)`: Takes an iterable of Promises as input and returns a single Promise. This returned Promise fulfills when *all* of the input Promises have fulfilled, or rejects as soon as *any* of the input Promises rejects. Use it when you need all results to proceed.

- `Promise.race(iterable)`: Takes an iterable of Promises as input and returns a single Promise. This returned Promise fulfills or rejects as soon as *any* of the input Promises fulfills or rejects, with the value or reason from that Promise. Use it when you only care about the first Promise to settle.

### Q: How do you handle errors in asynchronous JavaScript?

**Answer:** Error handling in asynchronous JavaScript depends on the mechanism used:

- **Callbacks:** Errors are typically passed as the first argument to the callback function (Node.js style `(err, data)`).

- **Promises:** Errors are handled using the `.catch()` method or by providing a second callback to `.then()`. Uncaught promise rejections can be handled globally with `window.addEventListener('unhandledrejection')`.

- **`async/await`****:** Errors are handled using standard `try...catch` blocks, similar to synchronous code, which makes error handling much cleaner.

### Q: What is `Promise.allSettled()`?

**Answer:** `Promise.allSettled(iterable)` takes an iterable of Promises and returns a single Promise that fulfills when *all* of the input Promises have settled (either fulfilled or rejected). The returned Promise resolves with an array of objects, each describing the outcome of a Promise (e.g., `{ status: 'fulfilled', value: result }` or `{ status: 'rejected', reason: error }`). This is useful when you want to know the outcome of every Promise, regardless of whether it succeeded or failed.

### Q: What is `Promise.any()`?

**Answer:** `Promise.any(iterable)` takes an iterable of Promises and returns a single Promise. This returned Promise fulfills as soon as *any* of the input Promises fulfills, with the value of that Promise. If all of the input Promises reject, then the returned Promise rejects with an `AggregateError` containing an array of all the rejection reasons. It's useful when you need the first successful result, and don't care about failures unless all fail.

---

## ES6+ & Modern Features

### Q: What are `let` and `const`? How do they improve upon `var`?

**Answer:** `let` and `const` are block-scoped variable declarations introduced in ES6, addressing issues with `var`'s function-scoping and hoisting behavior. `let` allows re-assignment but not re-declaration within the same scope, while `const` prevents both re-assignment and re-declaration, making it suitable for values that should not change. They improve code clarity, prevent accidental variable re-declarations, and reduce bugs related to variable scope and hoisting.

### Q: Explain destructuring assignment in ES6. Provide examples.

**Answer:** Destructuring assignment is a powerful ES6 feature that allows you to unpack values from arrays or properties from objects into distinct variables. It provides a concise way to extract data.**Example (Array Destructuring):**

```javascript
const numbers = [1, 2, 3];
const [a, b] = numbers;
console.log(a, b); // 1 2

// With rest pattern
const [first, ...rest] = numbers;
console.log(first, rest); // 1 [2, 3]
```

**Example (Object Destructuring):**

```javascript
const person = { name: 'Alice', age: 30 };
const { name, age } = person;
console.log(name, age); // Alice 30

// With alias and default value
const { name: fullName, city = 'New York' } = person;
console.log(fullName, city); // Alice New York
```

### Q: What are the spread (`...`) and rest (`...`) operators? Explain their differences.

**Answer:** Both use the `...` syntax but serve different purposes based on where they are used:

- **Spread Operator:** Used to expand an iterable (like an array or string) into individual elements, or to expand an object into key-value pairs. It's used when *calling* a function or creating new arrays/objects.**Example (Spread):**

   ```javascript
   const arr1 = [1, 2];
   const arr2 = [...arr1, 3, 4]; // [1, 2, 3, 4]
   const obj1 = { a: 1, b: 2 };
   const obj2 = { ...obj1, c: 3 }; // { a: 1, b: 2, c: 3 }
   ```

- **Rest Parameter:** Used to collect an indefinite number of arguments into an array. It's used in *function definitions* or array/object destructuring to gather remaining elements.**Example (Rest):**

   ```javascript
   function sum(...args) {
     return args.reduce((acc, val) => acc + val, 0);
   }
   console.log(sum(1, 2, 3, 4)); // 10
   
   const [first, ...remaining] = [1, 2, 3, 4];
   console.log(first, remaining); // 1 [2, 3, 4]
   ```

### Q: Explain ES6 Modules (`import`/`export`). Why are they important?

**Answer:** ES6 Modules provide a standardized way to organize JavaScript code into separate, reusable files. They allow you to `export` functions, classes, or variables from one file and `import` them into another. Key benefits include:

- **Modularity:** Better code organization and separation of concerns.

- **Encapsulation:** Variables and functions are private by default within a module unless explicitly exported.

- **Dependency Management:** Clear declaration of dependencies.

- **Performance:** Can be statically analyzed, enabling tree-shaking (removing unused code) and better optimization by bundlers.

### Q: What are Template Literals (Template Strings)?

**Answer:** Template literals are string literals allowing embedded expressions, multi-line strings, and string interpolation. They are enclosed by backticks (```) instead of single or double quotes.**Example:**

```javascript
const name = 'World';
const greeting = `Hello, ${name}!\nWelcome to multi-line strings.`;
console.log(greeting);
```

### Q: What are default parameters in functions?

**Answer:** Default parameters allow you to initialize a function parameter with a default value if an argument is not provided or is `undefined` when the function is called. This simplifies function signatures and reduces the need for manual checks inside the function body.**Example:**

```javascript
function greet(name = 'Guest') {
  console.log(`Hello, ${name}!`);
}
greet();        // Hello, Guest!
greet('Alice'); // Hello, Alice!
```

### Q: What are `Map` and `Set` in ES6? How do they differ from plain objects/arrays?

**Answer:**

- **`Map`****:** A collection of key-value pairs where keys can be of any data type (including objects or functions), unlike plain objects where keys must be strings or Symbols. `Map` maintains the insertion order of elements and provides methods like `set()`, `get()`, `has()`, `delete()`, and `size`.

- **`Set`****:** A collection of unique values. It allows you to store any type of value, whether primitive or object. `Set` provides methods like `add()`, `has()`, `delete()`, and `size`. It's useful for removing duplicates from an array or checking for the presence of an item.

### Q: Explain `for...of` and `for...in` loops. When would you use each?

**Answer:**

- **`for...in`**** loop:** Iterates over the *enumerable properties* of an object. It returns the *keys* (property names) as strings. It's generally not recommended for iterating over arrays because it can iterate over inherited properties and the order is not guaranteed.**Example (****`for...in`****):**

   ```javascript
   const obj = { a: 1, b: 2 };
   for (const key in obj) {
     console.log(key, obj[key]); // a 1, b 2
   }
   ```

- **`for...of`**** loop:** Iterates over the *values* of iterable objects (like Arrays, Strings, Maps, Sets, NodeLists, etc.). It returns the actual values, not the keys/indices. It's the preferred way to iterate over arrays and other iterable collections.**Example (****`for...of`****):**

   ```javascript
   const arr = [1, 2, 3];
   for (const value of arr) {
     console.log(value); // 1, 2, 3
   }
   ```

### Q: What are Generators in JavaScript?

**Answer:** Generators are special functions that can be paused and resumed, allowing them to produce a sequence of values over time rather than computing them all at once. They are defined using `function*` syntax and use the `yield` keyword to pause execution and return a value. When a generator function is called, it returns an iterator object, which can be used to control its execution (`.next()`). Generators are useful for implementing iterators, asynchronous programming, and infinite data streams.**Example:**

```javascript
function* idGenerator() {
  let id = 1;
  while (true) {
    yield id++;
  }
}

const gen = idGenerator();
console.log(gen.next().value); // 1
console.log(gen.next().value); // 2
```

### Q: What are Symbols in ES6?

**Answer:** Symbols are a new primitive data type introduced in ES6. They are unique and immutable values that can be used as object property keys. The primary purpose of Symbols is to create unique property keys that won't clash with other property keys, especially when adding properties to objects that you don't own or when implementing mixins. They are not enumerable by default.**Example:**

```javascript
const id = Symbol('id');
const user = {
  name: 'John',
  [id]: 123
};

console.log(user[id]); // 123
for (let key in user) {
  console.log(key); // Only 'name' is logged
}
```

---

## DOM Manipulation & Browser Events

### Q: What is the DOM? How does JavaScript interact with it?

**Answer:** The Document Object Model (DOM) is a programming interface for web documents. It represents the page structure as a tree of objects, where each node represents a part of the document (e.g., elements, attributes, text). JavaScript interacts with the DOM to dynamically change the content, structure, and style of a web page. It provides methods to select elements, modify their properties, add or remove elements, and handle events.

### Q: Explain Event Bubbling and Event Capturing.

**Answer:** These are two ways event propagation works in the DOM when an event occurs on an element that is nested inside other elements:

- **Event Capturing (Trickling Down):** The event starts from the `window` object, then goes down through the parent elements to the target element. This phase is rarely used in practice.

- **Event Bubbling (Bubbling Up):** The event starts at the target element and then propagates upwards through its parent elements to the `window` object. This is the default behavior for most events.

### Q: What is Event Delegation? Why is it useful?

**Answer:** Event delegation is a technique where you attach a single event listener to a parent element, instead of attaching individual listeners to multiple child elements. When an event bubbles up from a child element, the parent listener catches it. You can then determine which child element triggered the event using `event.target` and react accordingly. It's useful for:

- **Performance:** Reduces the number of event listeners, especially for large lists or dynamically added elements.

- **Dynamic Elements:** Automatically handles events for elements added to the DOM after the initial page load.

- **Memory Efficiency:** Less memory consumption as fewer listeners are created.

### Q: How do you prevent default browser behavior and event propagation?

**Answer:**

- **`event.preventDefault()`****:** Stops the default action of an event from happening. For example, preventing a form submission or a link from navigating.

- **`event.stopPropagation()`****:** Prevents the event from bubbling up (or capturing down) to parent (or child) elements. The event will only be handled by the current element and any listeners attached to it.

- **`event.stopImmediatePropagation()`****:** Prevents other listeners on the *same* element from being called, and also stops the event from bubbling up (or capturing down).

### Q: What is the Shadow DOM?

**Answer:** The Shadow DOM is a web standard that allows for component-based encapsulation in the DOM. It enables you to attach a hidden, separate DOM tree to an element, which is rendered along with the main document DOM. Thisencapsulation ensures that styles and scripts within the Shadow DOM do not leak out and affect the rest of the page, and vice versa. It's a key technology for building Web Components.

### Q: How do you select elements in the DOM?

**Answer:** JavaScript provides several methods to select DOM elements:

- `document.getElementById('id')`: Selects a single element by its ID.

- `document.getElementsByClassName('class')`: Returns an HTMLCollection of elements with the specified class.

- `document.getElementsByTagName('tag')`: Returns an HTMLCollection of elements with the specified tag name.

- `document.querySelector('selector')`: Returns the *first* element that matches a CSS selector.

- `document.querySelectorAll('selector')`: Returns a NodeList of *all* elements that match a CSS selector.

### Q: What is the difference between `innerHTML`, `innerText`, and `textContent`?

**Answer:**

- `innerHTML`: Gets or sets the HTML markup contained within an element. It parses the string as HTML, which can be a security risk (XSS) if used with unsanitized user input.

- `innerText`: Gets or sets the visible text content of an element and its descendants. It respects CSS styling (e.g., ignores hidden elements) and triggers a reflow when read.

- `textContent`: Gets or sets the text content of an element and all its descendants, regardless of CSS styling. It's generally faster than `innerText` because it doesn't trigger a reflow and is safer than `innerHTML` for plain text.

### Q: How do you create and append a new element to the DOM?

**Answer:** You can create and append elements using DOM manipulation methods:

1. Create the element: `const newDiv = document.createElement('div');`

1. Set its content or attributes: `newDiv.textContent = 'Hello World'; newDiv.className = 'my-class';`

1. Select the parent element: `const parent = document.getElementById('container');`

1. Append the new element: `parent.appendChild(newDiv);` (or `parent.append(newDiv)` for multiple nodes/strings).

### Q: What are data attributes (`data-*`)? How do you access them in JavaScript?

**Answer:** Data attributes allow you to store custom data directly on HTML elements. They are prefixed with `data-` (e.g., `data-user-id="123"`). In JavaScript, you can access them using the `dataset` property of the element. The `data-` prefix is removed, and the remaining part is converted to camelCase.**Example:**

```html
<div id="user" data-user-id="123" data-role="admin">User Info</div>
```

```javascript
const userDiv = document.getElementById('user');
console.log(userDiv.dataset.userId); // "123"
console.log(userDiv.dataset.role);   // "admin"
```

### Q: Explain the `DOMContentLoaded` event vs. the `load` event.

**Answer:**

- `DOMContentLoaded`: Fires when the initial HTML document has been completely loaded and parsed, without waiting for stylesheets, images, and subframes to finish loading. This is usually the best time to run DOM manipulation scripts.

- `load`: Fires when the whole page has loaded, including all dependent resources such as stylesheets and images. It's useful when you need to interact with elements that depend on external resources (e.g., getting the dimensions of an image).

---

## Performance & Memory Management

### Q: What is a memory leak in JavaScript? How do they occur?

**Answer:** A memory leak occurs when a piece of memory that is no longer needed by the application is not released back to the operating system. In JavaScript, this happens when objects are still referenced by the application, preventing the garbage collector from freeing them. Common causes include:

- Accidental global variables.

- Forgotten timers or callbacks (e.g., `setInterval` not cleared).

- Closures holding onto large objects unnecessarily.

- Detached DOM elements (elements removed from the DOM but still referenced in JavaScript).

### Q: How does Garbage Collection work in JavaScript?

**Answer:** JavaScript uses automatic garbage collection to manage memory. The most common algorithm is **Mark-and-Sweep**. It works by periodically starting from a set of "roots" (like global variables and the current call stack) and "marking" all objects that are reachable from these roots. Any object that is not marked is considered unreachable and its memory is "swept" (reclaimed).

### Q: Explain Debouncing and Throttling. When would you use each?

**Answer:** Both are techniques to control the rate at which a function is executed, often used for performance optimization with frequent events (like scrolling, resizing, or typing).

- **Debouncing:** Ensures a function is only executed *after* a certain amount of time has passed since it was last invoked. If the event occurs again before the time is up, the timer resets. Use it for tasks like search input suggestions (wait until the user stops typing).

- **Throttling:** Ensures a function is executed *at most once* in a specified time interval, regardless of how many times the event is triggered. Use it for tasks like tracking scroll position or handling window resize events.

### Q: What are Web Workers? Why are they useful?

**Answer:** Web Workers provide a way to run JavaScript code in background threads, separate from the main execution thread of a web application. This is crucial for performance because it allows you to perform computationally intensive tasks (like complex calculations or data processing) without blocking the main thread, keeping the UI responsive. Workers communicate with the main thread via a messaging system (`postMessage` and `onmessage`).

### Q: How can you optimize a slow loop in JavaScript?

**Answer:** Optimizing loops involves reducing the work done inside the loop and minimizing overhead:

- Cache array length: `for (let i = 0, len = arr.length; i < len; i++)` instead of checking `arr.length` every iteration.

- Use appropriate loop types: `for` loops are generally faster than `forEach` or `map` for simple iterations, though modern engines have optimized array methods significantly.

- Minimize DOM manipulation inside the loop: Build a string or DocumentFragment and append it to the DOM once after the loop finishes.

- Avoid creating functions inside the loop.

- Consider Web Workers for heavy computations.

### Q: What is a DocumentFragment? How does it improve performance?

**Answer:** A `DocumentFragment` is a lightweight, minimal document object that has no parent. It's used as a temporary container to hold DOM nodes. When you append a DocumentFragment to the DOM, only its children are inserted, not the fragment itself. It improves performance because changes made to a DocumentFragment do not trigger reflows or repaints in the main document. You can build a complex DOM structure in the fragment and then append it to the document in a single operation, minimizing performance overhead.

### Q: Explain the concept of "Reflow" and "Repaint" in the browser.

**Answer:**

- **Reflow (or Layout):** Occurs when the browser needs to recalculate the positions and geometries of elements in the document. This happens when you change properties that affect layout (e.g., width, height, margin, padding, font size, adding/removing elements). Reflows are computationally expensive.

- **Repaint:** Occurs when changes are made to an element's appearance that do not affect its layout (e.g., changing color, background-color, visibility). Repaints are less expensive than reflows but still consume resources.Optimizing performance often involves minimizing reflows and repaints, for example, by batching DOM changes or using CSS classes instead of inline styles.

### Q: What is the `requestAnimationFrame` API?

**Answer:** `requestAnimationFrame` is a browser API used for creating smooth animations. It tells the browser that you wish to perform an animation and requests that the browser call a specified function to update an animation before the next repaint. It's more efficient than using `setTimeout` or `setInterval` because it synchronizes with the browser's refresh rate (usually 60fps), preventing frame dropping and reducing CPU usage when the tab is inactive.

### Q: How do you identify memory leaks in a web application?

**Answer:** You can identify memory leaks using browser developer tools (like Chrome DevTools):

- **Performance Tab:** Record a timeline and look for a "sawtooth" pattern in memory usage that continuously grows over time without returning to a baseline.

- **Memory Tab (Heap Snapshots):** Take heap snapshots at different points in time and compare them to see which objects are accumulating and not being garbage collected. Look for detached DOM nodes or large arrays/objects that shouldn't exist.

- **Allocation Timelines:** Track memory allocations in real-time to pinpoint which functions are creating objects that aren't being cleaned up.

---

## Web APIs & Browser Storage

### Q: What is the Fetch API? How does it differ from XMLHttpRequest (XHR)?

**Answer:** The Fetch API provides a modern, Promise-based interface for making network requests (e.g., fetching resources across the network). It's a cleaner and more powerful alternative to the older `XMLHttpRequest` (XHR). Key differences:

- Fetch uses Promises, making asynchronous code easier to read and write (especially with `async/await`).

- Fetch does not send cross-origin cookies by default (unless configured).

- Fetch won't reject the Promise on HTTP error statuses (like 404 or 500); it only rejects on network failure. You must check the `response.ok` property.

### Q: Explain LocalStorage, SessionStorage, and Cookies. What are their differences?

**Answer:** These are mechanisms for storing data on the client-side:

- **LocalStorage:** Stores data with no expiration date. Data persists even when the browser is closed and reopened. Capacity is typically around 5-10MB per origin. Data is not sent to the server with every request.

- **SessionStorage:** Stores data for the duration of the page session. Data is cleared when the page or tab is closed. Capacity is similar to LocalStorage. Data is not sent to the server.

- **Cookies:** Small pieces of data (up to 4KB) sent to the server with every HTTP request. They can have expiration dates and are often used for authentication, session management, and tracking. They are less secure for sensitive data unless configured properly (e.g., HttpOnly, Secure flags).

### Q: What is the Intersection Observer API? What are its use cases?

**Answer:** The Intersection Observer API provides a way to asynchronously observe changes in the intersection of a target element with an ancestor element or with a top-level document's viewport. It's highly performant because it doesn't rely on scroll events or continuous polling.**Use cases:**

- Lazy loading images or other content as they scroll into view.

- Implementing "infinite scrolling" web pages.

- Reporting visibility of advertisements for calculating ad revenues.

- Triggering animations when elements become visible.

### Q: What is the Web Storage API?

**Answer:** The Web Storage API provides mechanisms by which browsers can store key/value pairs, in a much more intuitive fashion than using cookies. It encompasses both `localStorage` and `sessionStorage`. The keys and values are always strings (you must serialize objects using `JSON.stringify()` before storing and parse them with `JSON.parse()` when retrieving).

### Q: Explain the concept of CORS (Cross-Origin Resource Sharing).

**Answer:** CORS is a security mechanism implemented by browsers that restricts web pages from making requests to a different domain (origin) than the one that served the web page. This is known as the Same-Origin Policy. CORS allows servers to specify which origins are permitted to access their resources by sending specific HTTP headers (e.g., `Access-Control-Allow-Origin`). If the server doesn't provide the correct headers, the browser blocks the request.

### Q: What are Service Workers?

**Answer:** Service Workers are scripts that run in the background, separate from a web page, opening the door to features that don't need a web page or user interaction. They act as a proxy server that sits between web applications, the browser, and the network. They are primarily used for:

- Offline experiences (caching assets and API responses).

- Background sync.

- Push notifications.They require HTTPS for security reasons.

### Q: How do you handle JSON data in JavaScript?

**Answer:** JavaScript provides the built-in `JSON` object to handle JSON (JavaScript Object Notation) data:

- `JSON.parse(jsonString)`: Parses a JSON string and constructs the JavaScript value or object described by the string.

- `JSON.stringify(value)`: Converts a JavaScript object or value to a JSON string.**Example:**

```javascript
const obj = { name: "Alice", age: 30 };
const jsonString = JSON.stringify(obj); // '{"name":"Alice","age":30}'
const parsedObj = JSON.parse(jsonString); // { name: 'Alice', age: 30 }
```

### Q: What is the Geolocation API?

**Answer:** The Geolocation API allows the user to provide their location to web applications if they so desire. For privacy reasons, the user is asked for permission to report location information. It provides methods like `navigator.geolocation.getCurrentPosition()` to get the current location and `navigator.geolocation.watchPosition()` to track location changes.

---

## Testing & Error Handling

### Q: What are the different types of errors in JavaScript?

**Answer:** Common error types in JavaScript include:

- **SyntaxError:** Occurs when the code violates the syntax rules of the language (e.g., missing a parenthesis).

- **ReferenceError:** Occurs when trying to access a variable that has not been declared.

- **TypeError:** Occurs when a value is not of the expected type (e.g., calling a method on `undefined` or `null`).

- **RangeError:** Occurs when a numeric variable or parameter is outside of its valid range.

- **URIError:** Occurs when `encodeURI()` or `decodeURI()` are used incorrectly.

### Q: How do you use `try...catch...finally` blocks?

**Answer:** The `try...catch...finally` statement handles exceptions (errors) in JavaScript.

- **`try`****:** Contains the code that might throw an error.

- **`catch`****:** Contains the code that executes if an error is thrown in the `try` block. It receives the error object as an argument.

- **`finally`****:** Contains code that executes regardless of whether an error was thrown or caught. It's often used for cleanup tasks (e.g., closing a file or network connection).**Example:**

```javascript
try {
  // Code that might throw an error
  const result = riskyOperation();
} catch (error) {
  // Handle the error
  console.error("An error occurred:", error.message);
} finally {
  // Always executes
  console.log("Operation finished.");
}
```

### Q: How do you create custom errors in JavaScript?

**Answer:** You can create custom errors by extending the built-in `Error` class. This allows you to define specific error types for your application, making error handling more precise.**Example:**

```javascript
class ValidationError extends Error {
  constructor(message) {
    super(message);
    this.name = "ValidationError";
  }
}

function validateAge(age) {
  if (age < 0) {
    throw new ValidationError("Age cannot be negative.");
  }
  return true;
}
```

### Q: What is the concept of Error Boundaries (in the context of UI frameworks like React, but conceptually in JS)?

**Answer:** While Error Boundaries are a specific feature in React, the concept applies generally: it's a mechanism to catch JavaScript errors anywhere in a component tree (or application module), log those errors, and display a fallback UI instead of crashing the entire application. In plain JavaScript, this might involve wrapping main application entry points or specific modules in robust `try...catch` blocks or global error handlers to prevent a single failure from taking down the whole system.

### Q: How do you handle global unhandled errors and promise rejections?

**Answer:** You can catch errors that slip through `try...catch` blocks using global event listeners on the `window` object:

- **`window.onerror`**** or ****`window.addEventListener('error', ...)`****:** Catches unhandled synchronous errors and errors in event handlers.

- **`window.addEventListener('unhandledrejection', ...)`****:** Catches unhandled Promise rejections (when a Promise rejects but there is no `.catch()` handler).

### Q: What is Jest? What are its key features?

**Answer:** Jest is a popular JavaScript testing framework maintained by Meta (Facebook). It's widely used for testing React applications but works well with plain JavaScript, Node.js, Vue, and Angular. Key features include:

- **Zero configuration:** Works out of the box for most JavaScript projects.

- **Snapshots:** Allows you to capture the state of a UI component or object and compare it in future tests to detect unintended changes.

- **Mocking:** Built-in support for mocking functions, modules, and timers.

- **Code Coverage:** Built-in code coverage reports.

- **Parallel testing:** Runs tests in parallel for faster execution.

### Q: Explain the difference between Unit Testing, Integration Testing, and End-to-End (E2E) Testing.

**Answer:**

- **Unit Testing:** Tests individual, isolated units of code (e.g., a single function or class) to ensure they work correctly in isolation.

- **Integration Testing:** Tests how different units or modules work together. It verifies the interactions between components.

- **End-to-End (E2E) Testing:** Tests the entire application flow from start to finish, simulating real user scenarios in a browser environment (e.g., using tools like Cypress or Playwright).

### Q: What is Test-Driven Development (TDD)?

**Answer:** TDD is a software development process where you write tests *before* writing the actual code. The cycle is typically:

1. **Red:** Write a failing test for a new feature.

1. **Green:** Write the minimum amount of code necessary to make the test pass.

1. **Refactor:** Improve the code while ensuring the tests still pass.TDD helps ensure code quality, better design, and comprehensive test coverage.

---

## Coding Challenges & Polyfills

### Q: Write a polyfill for `Array.prototype.map()`.

**Answer:**

```javascript
if (!Array.prototype.myMap) {
  Array.prototype.myMap = function(callback, thisArg) {
    if (this == null) throw new TypeError('this is null or not defined');
    if (typeof callback !== 'function') throw new TypeError(callback + ' is not a function');
    
    const O = Object(this);
    const len = O.length >>> 0;
    const A = new Array(len);
    
    for (let k = 0; k < len; k++) {
      if (k in O) {
        A[k] = callback.call(thisArg, O[k], k, O);
      }
    }
    return A;
  };
}
```

### Q: Write a polyfill for `Array.prototype.filter()`.

**Answer:**

```javascript
if (!Array.prototype.myFilter) {
  Array.prototype.myFilter = function(callback, thisArg) {
    if (this == null) throw new TypeError('this is null or not defined');
    if (typeof callback !== 'function') throw new TypeError(callback + ' is not a function');
    
    const O = Object(this);
    const len = O.length >>> 0;
    const res = [];
    
    for (let i = 0; i < len; i++) {
      if (i in O) {
        const val = O[i];
        if (callback.call(thisArg, val, i, O)) {
          res.push(val);
        }
      }
    }
    return res;
  };
}
```

### Q: Write a polyfill for `Array.prototype.reduce()`.

**Answer:**

```javascript
if (!Array.prototype.myReduce) {
  Array.prototype.myReduce = function(callback, initialValue) {
    if (this == null) throw new TypeError('this is null or not defined');
    if (typeof callback !== 'function') throw new TypeError(callback + ' is not a function');
    
    const O = Object(this);
    const len = O.length >>> 0;
    let k = 0;
    let accumulator;
    
    if (arguments.length >= 2) {
      accumulator = initialValue;
    } else {
      while (k < len && !(k in O)) {
        k++;
      }
      if (k >= len) throw new TypeError('Reduce of empty array with no initial value');
      accumulator = O[k++];
    }
    
    while (k < len) {
      if (k in O) {
        accumulator = callback(accumulator, O[k], k, O);
      }
      k++;
    }
    return accumulator;
  };
}
```

### Q: Implement a deep clone function for an object.

**Answer:** A simple `JSON.parse(JSON.stringify(obj))` works for basic objects but fails with functions, Dates, undefined, or circular references. A robust recursive approach is needed.

```javascript
function deepClone(obj, hash = new WeakMap()) {
  if (obj === null || typeof obj !== 'object') return obj;
  if (obj instanceof Date) return new Date(obj);
  if (obj instanceof RegExp) return new RegExp(obj);
  
  if (hash.has(obj)) return hash.get(obj); // Handle circular references
  
  const clone = Array.isArray(obj) ? [] : {};
  hash.set(obj, clone);
  
  for (let key in obj) {
    if (Object.prototype.hasOwnProperty.call(obj, key)) {
      clone[key] = deepClone(obj[key], hash);
    }
  }
  return clone;
}
```

### Q: Implement a debounce function.

**Answer:**

```javascript
function debounce(func, delay) {
  let timeoutId;
  return function(...args) {
    const context = this;
    clearTimeout(timeoutId);
    timeoutId = setTimeout(() => {
      func.apply(context, args);
    }, delay);
  };
}
```

### Q: Implement a throttle function.

**Answer:**

```javascript
function throttle(func, limit) {
  let inThrottle;
  return function(...args) {
    const context = this;
    if (!inThrottle) {
      func.apply(context, args);
      inThrottle = true;
      setTimeout(() => inThrottle = false, limit);
    }
  };
}
```

### Q: Write a function to flatten a nested array.

**Answer:**

```javascript
// Using recursion
function flattenArray(arr) {
  return arr.reduce((acc, val) => 
    Array.isArray(val) ? acc.concat(flattenArray(val)) : acc.concat(val), []
  );
}

// Using ES6 flat() (if allowed)
// const flattened = arr.flat(Infinity);
```

### Q: Write a polyfill for `Promise.all()`.

**Answer:**

```javascript
function myPromiseAll(promises) {
  return new Promise((resolve, reject) => {
    if (!Array.isArray(promises)) {
      return reject(new TypeError('Argument must be an array'));
    }
    
    const results = [];
    let completedCount = 0;
    
    if (promises.length === 0) {
      return resolve(results);
    }
    
    promises.forEach((promise, index) => {
      Promise.resolve(promise)
        .then(value => {
          results[index] = value;
          completedCount++;
          if (completedCount === promises.length) {
            resolve(results);
          }
        })
        .catch(error => {
          reject(error);
        });
    });
  });
}
```

---

## Design Patterns & Architecture

### Q: What are Design Patterns in JavaScript? Why use them?

**Answer:** Design patterns are reusable, proven solutions to common problems in software design. They are not finished code, but templates or blueprints for solving a problem in a specific context. Using them helps write code that is more maintainable, scalable, and easier to understand, as they provide a shared vocabulary for developers.

### Q: Explain the Module Pattern.

**Answer:** The Module Pattern is used to encapsulate "private" variables and functions, exposing only a public API. Before ES6 modules, this was typically achieved using an IIFE (Immediately Invoked Function Expression) and closures. It helps prevent global namespace pollution.**Example:**

```javascript
const myModule = (function() {
  let privateVar = 'I am private';
  
  function privateMethod() {
    console.log(privateVar);
  }
  
  return {
    publicMethod: function() {
      privateMethod();
    }
  };
})();

myModule.publicMethod(); // Logs: I am private
// myModule.privateVar is undefined
```

### Q: Explain the Singleton Pattern.

**Answer:** The Singleton Pattern ensures that a class has only one instance and provides a global point of access to it. It's useful for managing shared resources, like a configuration object, a database connection, or a state store.**Example:**

```javascript
class Database {
  constructor() {
    if (Database.instance) {
      return Database.instance;
    }
    this.connection = 'Connected';
    Database.instance = this;
  }
}

const db1 = new Database();
const db2 = new Database();
console.log(db1 === db2); // true
```

### Q: Explain the Observer Pattern (Pub/Sub).

**Answer:** The Observer Pattern defines a one-to-many dependency between objects so that when one object (the subject/publisher) changes state, all its dependents (observers/subscribers) are notified and updated automatically. It's heavily used in event handling and state management (like Redux).**Example:**

```javascript
class Subject {
  constructor() {
    this.observers = [];
  }
  subscribe(observer) {
    this.observers.push(observer);
  }
  unsubscribe(observer) {
    this.observers = this.observers.filter(obs => obs !== observer);
  }
  notify(data) {
    this.observers.forEach(observer => observer(data));
  }
}
```

### Q: Explain the Factory Pattern.

**Answer:** The Factory Pattern is a creational pattern that provides an interface for creating objects in a superclass, but allows subclasses to alter the type of objects that will be created. It abstracts the object creation process, making it easier to manage complex object instantiation logic.**Example:**

```javascript
class Car { constructor() { this.type = 'Car'; } }
class Truck { constructor() { this.type = 'Truck'; } }

class VehicleFactory {
  createVehicle(type) {
    switch(type) {
      case 'car': return new Car();
      case 'truck': return new Truck();
      default: throw new Error('Unknown vehicle type');
    }
  }
}
```

### Q: What is the difference between Object-Oriented Programming (OOP) and Functional Programming (FP) in JavaScript?

**Answer:**

- **OOP:** Focuses on modeling the system as a collection of objects that contain both data (state) and behavior (methods). It relies on concepts like classes, inheritance, encapsulation, and polymorphism. State is often mutable.

- **FP:** Focuses on building software by composing pure functions, avoiding shared state, mutable data, and side effects. It relies on concepts like first-class functions, higher-order functions, immutability, and declarative code. JavaScript supports both paradigms.

### Q: What is MVC (Model-View-Controller)?

**Answer:** MVC is an architectural pattern that separates an application into three main logical components:

- **Model:** Manages the data, logic, and rules of the application.

- **View:** Handles the UI and presentation of the data.

- **Controller:** Accepts input, converts it to commands for the Model or View, and acts as an intermediary between them.

---

## Behavioral & Scenario-based Questions

### Q: How would you debug a memory leak in a JavaScript application?

**Answer:** I would start by using the browser's DevTools (e.g., Chrome DevTools). First, I'd use the Performance tab to record a timeline and look for a sawtooth pattern in memory usage that doesn't return to a baseline, indicating a leak. Then, I'd use the Memory tab to take Heap Snapshots at different points in time. By comparing these snapshots, I can identify objects that are accumulating and not being garbage collected. I'd look for detached DOM nodes, large arrays, or closures holding onto references unnecessarily. Once identified, I'd trace the allocation stack to find the code responsible and fix the reference issue.

### Q: You have a slow-rendering list of 10,000 items. How do you optimize it?

**Answer:** Rendering 10,000 DOM nodes at once will freeze the browser. I would optimize this using **Virtualization (or Windowing)**. Instead of rendering all items, I would only render the items currently visible in the viewport, plus a small buffer above and below. As the user scrolls, I would dynamically replace the DOM nodes with new data, reusing the existing elements. Libraries like `react-window` or `react-virtualized` do this. Alternatively, if virtualization isn't possible, I'd use pagination or an "infinite scroll" approach to load data in smaller chunks.

### Q: How do you handle a situation where an API request fails frequently due to network instability?

**Answer:** I would implement a **retry mechanism with exponential backoff**. If a request fails, the application shouldn't immediately retry, as it might overwhelm the server or fail again. Instead, it should wait a short time (e.g., 1 second), then retry. If it fails again, wait longer (e.g., 2 seconds, then 4 seconds), up to a maximum number of retries. I would also ensure the user is informed of the issue with a graceful error message and perhaps a manual "Retry" button if the automatic retries fail.

### Q: Explain how you would implement a search feature that fetches results from an API as the user types.

**Answer:** To prevent making an API call for every single keystroke (which would overload the server and cause race conditions), I would use **debouncing**. I'd wrap the API call function in a debounce function with a delay of, say, 300ms. This ensures the API is only called after the user has stopped typing for 300ms. Additionally, I would need to handle race conditions (where an older request resolves after a newer one) by either aborting previous requests using the `AbortController` API or by keeping track of the latest request ID and ignoring responses from older IDs.

### Q: How do you ensure your JavaScript code is secure?

**Answer:** Security involves several practices:

- **Preventing XSS (Cross-Site Scripting):** Never trust user input. Always sanitize and escape data before rendering it in the DOM (avoiding `innerHTML` when possible, using `textContent` instead).

- **Preventing CSRF (Cross-Site Request Forgery):** Use anti-CSRF tokens for state-changing requests.

- **Using HTTPS:** Ensure all data transmission is encrypted.

- **Dependency Management:** Regularly audit and update npm packages to patch known vulnerabilities (using `npm audit`).

- **Avoiding ****`eval()`****:** Never use `eval()` or `new Function()` with untrusted input, as it can execute malicious code.

### Q: Describe a time you had to optimize the performance of a web application. What steps did you take?

**Answer:** *(This requires a personal anecdote, but a good structure is:)* "In a previous project, the initial load time was very slow. I started by running Lighthouse audits to identify bottlenecks. I found that we were serving large, unoptimized images and a massive JavaScript bundle. I implemented image compression and lazy loading for images below the fold. For the JavaScript, I implemented code splitting using Webpack, so we only loaded the code necessary for the initial route. I also moved some heavy data processing to a Web Worker. These changes reduced the Time to Interactive (TTI) by 50%."

---

## How to Use This Guide

- **Daily Revision:** Try to cover one or two sections per day to avoid feeling overwhelmed.

- **Mock Interviews:** Have a friend ask you these questions, or practice answering them out loud to yourself.

- **Code Practice:** Don't just read the coding challenges; write them out in a code editor or on a whiteboard to build muscle memory.

- **Quick Lookup:** Use `Ctrl+F` (or `Cmd+F`) to quickly find specific topics or keywords you need to brush up on right before an interview.
