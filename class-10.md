
# The Call Stack
A call stack is a mechanism for an interpreter (like the JavaScript interpreter in a web browser) to keep track of its place in a script that calls multiple functions — what function is currently being run and what functions are called from within that function.
- It's the instruction sheet for the interpreter.
- When a function is called it gets added to the top of the call stack
- When the current function is finished its taken off the stack and the next function gets run
- If the stack takes up more space that it has assigned to it will cause a 'stack overflow'.
- Runs on LIFO - last in first out.
- When a function it invoked, the function, its parameters and variable are pushed onto the stack.
- When the function finished it gets popped off the top of the stack.

## Error messages
### Types of error messages
- Reference Errors
  - When a variable is not yet declared.
  - Trying to access a poorly scoped variable
- Syntax errors
  - Trying to parse an invalid object
  - Forgetting , or } etc.
- Range Errors
  - Trying to manipulate something outside its range
  - Looking for and index of an array that is larger than the array
- Type errors
  - Trying to work with incompatible types
### Debugging
- Use console.log
- Use breakpoints in the browser
## Call Stack
### Handling Errors
- Try-catch blocks
- Try{ //do this } catch(err){ //show the err }
### Tools to avoid
- quokka - code evaluator
- eslint - helps with style and flag possible errors along the way.

## Conclusion
Being able to read error messages and practicing debugging is one of your biggest weapons has a developer, do it frequently and with enough time you will notice a great decrease in the time you spend on each error that you find along the way. And remember, before a commit/push, remove all the debugging stuff from your code, we don’t want the client or another developer to get stuck on a debugger now do we?

[The Call Stack defined on MDN](https://developer.mozilla.org/en-US/docs/Glossary/Call_stack)

[Understanding the JavaScript Call Stack](https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4/)

[JavaScript error messages](https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c)