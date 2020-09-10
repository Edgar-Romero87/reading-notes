# Authentication

1. **Explain what a “Singleton” is (in Computer Science terms)**

A singleton class is a class that can have only one object (an instance of the class) at a time. After first time, if we try to instantiate the Singleton class, the new variable also points to the first instance created.

2. **Explain how the Singleton pattern can be used with Node modules, specifically with classes**

Singleton classes are used for logging, driver objects, caching and thread pool, database connections.

3. **If you were tasked with building a middleware system like Express uses, what approach might you take to construct/operate it?**

First identify my inputs given, and outputs expected, next I would create my folders and files to have all the modules organize, install my dependencies, and test my modules.

## Vocabulary Terms

## Router Middleware
Router-level middleware works in the same way as application-level middleware, except it is bound to an instance of `express.Router()`.
## Dynamic Module Loading
Loading modules asynchrously rather than statically.
## Singleton Pattern
The Singleton Pattern limits the number of instances of a particular object to just one. This single instance is called the singleton.
Singletons are useful in situations where system-wide actions need to be coordinated from a single central place.
## CRUD -> REST Method Matches
- Create -> PUT & POST
- Read -> GET
- Update -> PUT
- Delete -> DELETE
## Mock Testing
A method in jest used to test methods. Instead of using real life data like credit cards or make network requests. It fake data to be able to test certain methods.
