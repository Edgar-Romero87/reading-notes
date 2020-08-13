# Classes, Inheritance, Func...

1. **Name 3 advantages to Test Driven Development**

* Better program design and higher code quality.
* Detailed project documentation. 
* Code flexibility and easier maintenance.

2. **In what case would you need to use `beforeEach()` or `afterEach()` in a test suite?**

The `beforeEach` and `afterEach` commands are used to set up and tear down tasks at the beginning and end of test blocks. They can both handle asynchronous code just as the tests themselves can. The reason we would want to use beforeEach and afterEach would be to help keep your code clean and prevent duplicate code. If the tests are required to interact with a specific piece of code in order to run, using these commands will save time and make things easier to read and require less resources for the test suite to run.

3. **What is one downside of Test Driven Development?**

What is one downside of Test Driven Development.

4. **What’s the primary difference between ES6 Classes and Constructor/Prototype Classes?**

While you can get virtually the same end result using either method, the newer ES6 Classes are much easier to read and understand with just a quick glance. In addition, they are easier to write as the syntax is much more straight forward.

5. **Name a use case for a static method**

A static method belongs to the class rather than the object of a class.

6. **Write an example of a Higher Order function and describe the use case it solves**

The `filter()` method creates a new array with all elements that pass the test provided by the callback function. The callback function passed to the `filter()` method accepts 3 arguments: element, index, and array.

```
const persons = [
  { name: 'Peter', age: 16 },
  { name: 'Mark', age: 18 },
  { name: 'John', age: 27 },
  { name: 'Jane', age: 14 },
  { name: 'Tony', age: 24},
];
const fullAge = persons.filter(person => person.age >= 18);
console.log(fullAge);
```
## Vocabulary Terms
### functional programming
Is the process of building software by composing pure functions, avoiding shared state, mutable data, and side-effects.
### pure function
A pure function is a function that has the following properties: Its return value is the same for the same arguments. Its evaluation has no side effects. Thus a pure function is a computational analogue of a mathematical function.
### higher-order function
A function that operates on another function.
### immutable state
A state that refers to objects, arrays, etc. that ca not be modified after it is created.
### object
An object is a collection of properties, and a property is an association between a name (or key) and a value.
### object-oriented programming (OOP)
Object-oriented programming (OOP) is a programming paradigm based on the concept of "objects", which can contain data, in the form of fields (often known as attributes or properties), and code, in the form of procedures (often known as methods).
### class
A class is a type of function, but instead of using the keyword function to initiate it, we use the keyword class, and the properties are assigned inside a `constructor()` method.
### prototype
When a function is created in JavaScript, the JavaScript engine adds a prototype property to the function. This prototype property is an object (called a prototype object) that has a constructor property by default. The constructor property points back to the function on which prototype object is a property
### super
The super keyword is used to access and call functions on an object's parent. The super. prop and super[expr] expressions are valid in any method definition in both classes and object literals.
### inheritance
Inheritance is an important concept in object oriented programming. In the classical inheritance, methods from base class get copied into derived class. In JavaScript, inheritance is supported by using prototype object.
### constructor
A constructor is a function that creates an instance of a class which is typically called an “object”. In JavaScript, a constructor gets called when you declare an object using the new keyword. The purpose of a constructor is to create an object and set values if there are any object properties present.
### instance
An “instance” means a reference to an “object” created by “new” or the equivalent. What's special about JavaScript, and other scripting languages, is that an “instance” is just a regular object; it's not what it is, but how it's made that is different.
### context
Context in JavaScript is related to objects. It refers to the object within the function being executed. this refers to the object that the function is executing in.
### this
The JavaScript this keyword refers to the object it belongs to. ... In a function, this refers to the global object. In a function, in strict mode, this is undefined . In an event, this refers to the element that received the event.
### Test Driven Development (TDD)
Test-driven development is a software development process that relies on the repetition of a very short development cycle: requirements are turned into very specific test cases, then the code is improved so that the tests pass.
### Jest
Jest is a JavaScript testing framework designed to ensure correctness of any Javascript codebase.
### Continuous Integration (CI)
In software engineering, continuous integration is the practice of merging all developers' working copies to a shared mainline several times a day.
### unit test
Unit tests only test a single part of your implementation. A unit. No dependencies or integrations, no framework specifics.