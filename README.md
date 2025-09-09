## Question-1: What is the difference between var, let, and const?
## Ans: 
The main differences between var, let, and const in JavaScript are scope, reassignment, and redeclaration. var is function-scoped, allowing reassigning and redeclaring, and is generally avoided in modern JavaScript. let is block-scoped (limited to curly braces {}), can be reassigned but not redeclared within the same scope, and is preferred for variables whose values might change. const is also block-scoped, cannot be reassigned or redeclared after initialization, and is used for values that should remain constant.

## Question-2:  What is the difference between map(), forEach(), and filter()?
## Ans: 
The primary differences between map(), forEach(), and filter() in JavaScript array methods lie in their purpose and return values.
### forEach(): 
This method iterates over each element in an array and executes a provided callback function for each element. Its main purpose is to perform side effects, such as logging values or modifying external variables. forEach() does not return a new array; it always returns undefined.
### map(): 
This method creates a new array by calling a provided callback function on every element in the original array. The callback function is expected to return a value for each element, and these returned values form the elements of the new array. map() is used for transforming elements into a new set of data. 
### filter(): 
This method creates a new array containing only the elements from the original array that satisfy a specified condition. The provided callback function for filter() should return a boolean value (true or false) for each element. Only elements for which the callback returns true are included in the new array. filter() is used for selecting a subset of elements.
In summary, forEach() is for iteration and side effects (no return value). map() is for transformation and creating a new array of transformed elements. filter() is for selection and creating a new array of elements that meet a condition.

## Question-3: What are arrow functions in ES6?
## Ans: 
Arrow functions, introduced in ECMAScript 2015 (ES6), provide a concise syntax for writing function expressions in JavaScript. They offer a shorter and more elegant way to define functions compared to traditional function declarations or expressions.
##### Key characteristics of arrow functions:
Concise Syntax: They omit the function keyword and use an arrow (=>) to separate parameters from the function body.
Implicit Return: For single-expression arrow functions, the curly braces {} and the return keyword can be omitted, as the expression's result is automatically returned.
Lexical this Binding: This is a significant difference from traditional functions. Arrow functions do not create their own this context; instead, they inherit this from the surrounding (lexical) scope where they are defined. This simplifies handling this in callbacks and event handlers.
No arguments object: Arrow functions do not have their own arguments object. If access to arguments is needed, rest parameters (...args) can be used.
Cannot be used as constructors: Arrow functions cannot be used with the new keyword to create new objects.
No prototype property: They do not have a prototype property.
When to use arrow functions:
Arrow functions are particularly well-suited for:
Short, simple functions: Their concise syntax makes them ideal for one-liner functions.
Callbacks: They are frequently used as callbacks in array methods like map, filter, and reduce, and in asynchronous operations.
Maintaining this context: Their lexical this binding simplifies scenarios where this would otherwise be problematic in traditional functions.

## Question-4: How does destructuring assignment work in ES6?
## Ans: 
Destructuring assignment in ES6 is a powerful syntax that allows you to unpack values from arrays or properties from objects into distinct variables. It provides a more concise and readable way to extract data, avoiding the need to access each value by its index or key individually.
##### Array Destructuring
Array destructuring uses a syntax that mimics array literals on the left-hand side of an assignment. The variables are assigned to elements of the array based on their position.
##### Object Destructuring
Object destructuring uses a syntax that mimics object literals on the left-hand side of an assignment. The variables are assigned to properties of the object based on their key.

## Question-5: Explain template literals in ES6. How are they different from string concatenation?
## Ans: 
Template literals (or template strings) are a new way to work with strings in ES6. They provide a more flexible and powerful syntax for creating strings, especially when you need to embed variables or expressions. Template literals are enclosed by backticks (``), not single or double quotes.
Template literals are a superior alternative to string concatenation, which uses the + operator to join strings and variables.
Readability: Concatenation can quickly become messy and hard to read as you add more variables. Template literals provide a clean, readable syntax where the variables are right where they need to be.
Syntax: Concatenation requires you to manually add the + operator and quotes around each string part. With template literals, the entire string is written in a single block, with backticks at the start and end.
Functionality: Template literals offer built-in support for multi-line strings and expression evaluation, features that are cumbersome or not possible with simple string concatenation.

