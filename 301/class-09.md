# Refactoring
## Concepts of Functional Programming
[Article](https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa) 

“Complexity is anything that makes software hard to understand or to modify." — John Outerhout

## What is functional programming?
Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data 
## Pure functions:
It returns the same result if given the same arguments
If our function reads external files, it’s not a pure function — the file’s contents can change.
Any function that relies on a random number generator cannot be pure
Pure functions are stable, consistent, and predictable.
- It returns the same result if given the same arguments (it is also referred as deterministic)
- It does not cause any observable side effects
### Random number generation
Any function that relies on a random number generator cannot be pure.
### Observation
mutability is discouraged in functional programming.

## Immutability:

When data is immutable, its state cannot change after it’s created.
Referential transparency:

pure functions + immutable data = referential transparency
Functions as first-class entities:

refer to it from constants and variables
pass it as a parameter to other functions
return it as result from other functions
The idea is to treat functions as values and pass functions like data.

## Higher-order functions:
Takes one or more functions as arguments, or
returns a function as its result
Filter:

Given a collection, we want to filter by an attribute. The filter function expects a true or false value to determine if the element should or should not be included in the result collection.

## Map:
The map method transforms a collection by applying a function to all of its elements and building a new collection from the returned values.
Transform a given array into a new array
## Reduce:
The idea of reduce is to receive a function and a collection, and return a value created by combining the items.Reduce
The idea of reduce is to receive a function and a collection, and return a value created by combining the items.
A common example people talk about is to get the total amount of an order. Imagine you were at a shopping website. You’ve added Product 1, Product 2, Product 3, and Product 4 to your shopping cart (order). Now we want to calculate the total amount of the shopping cart.

[Refactoring JavaScript](https://dev.to/healeycodes/refactoring-javascript-for-performance-and-readability-with-examples-1hec)

It's important to get your code right the first time because in many businesses there isn't much value in refactoring. Or at least, it's hard to convince stakeholders that eventually uncared for codebases will grind productivity to a halt.