# Error Handling & Debugging
JavaScript can be hard to learn and everyone makes mistakes when writing it.
When you write JavaScript, do not expect to write it perfectly the firts time. Programming is like problem solving: you are given a puzzle and not only do you have to solve it, but you also need to create the instructions that allow the computer to solve it too.
When writing a long script, nobody gets everything right in their first attempt. The error messages that a browser gives look cryptic at first but they can help you determine what went wrong in your JavaScript and how to fix it.

## The Stack
The JavaScript interpreter processes one line of code at a time. When a statement needs data from another function, it **stacks** (or piles) the new function on top of the current task. Once the new task has been performed,  the interpreter can go back to the task in hand. 
Each time a new task is added to the stack, it creates a new execution context.
Variables defined in a function (or execution context) are only available in that function. 
If a function gets called a second time, the variables can have different values.

### Execution Context & Hoisting
Each time a script enters a new  execution context, there are two phases of activity:
1- **Prepare:**
The new scoped is created.
Variables, functions, and arguments are created.
The value of this keyword is determined.

2- **Execute:**
Now it can assign values to variables.
Reference functions and run their code.
Execute stamens.

### Understanding Scope

In the interpreter, each execution context has its own variables object. It holds the variables, functions and parameters available within it. Each execution context can also acmes its parent’s variables object. 
Functions in JavaScript are said to have **lexical scope**. They are linked to the object they were defined within. So, for each execution context, the scope is the current execution context’s variables object, plus the variables object for each parent execution context.
  
### Understanding Errors 
If JavaScript statements generates an error, then it throws an **execution**. At that point, the interpreter stops and looks for exception-
handling code.

Error Objects
Error objects can help you find where your mistakes are and browsers have tools to help you read them.


### How to Deal With Errors
Now that you know what an error is and how the browser treats them, there are two things you can do with errors:
1- Debug the script to fix the errors
If you come across an error while writing a script, you will need to debug the code, track down the source of the error and fix it. You will find that the developer tools available in every major modern browser will help you with this task.

2- Handled errors gracefully
 You can handle errors gracefully using **try, catch, throw and finally** statements. Sometimes, an error may occur in the script for a reason beyond your control. 

Debugging is the process of finding errors. It involves a process of deduction.
JavaScript has 7 different types of errors. Each creates its own error object, with can tell you its lie number and gives you a description of the error.   

### Writing a tubular data
In browsers that support it, the **console.table( )** method lets you output a table showing:
Objects
Arrays that contain other objects or arrays.

### Writing On A Condition
Using the **console.assert( )** method you can test if a condition is met, and write to the console only is the expression evaluates to false.

### Breakpoints
You can pause the execution of a script on any line using breakpoints. Then you can check the values stored in variables at that point in time.

### Stepping Through Code
If you set multiple breakpoints, you can step through them one-by-one to se where values change and a problem my occur.

### Conditional Brakpoints
You can indicate that. Breakpoint should be triggered only a condition that you specify is met. The condition can use existing variables.

### Debugger Keyword
 You can create a breakpoint in your code using just the **debugger** keyword. When the developer tools are open, this will automatically create a breakpoint. 

### Handling exemptions
If you know your code is might fail, use try, catch and finally. Each one is given its own code block.

### TRY
First, you specify the code that you think might thrown an exception within the try block. If an exception occurs in this section code, control is automatically  passed to the corresponding catch block.

### CATCH
If the try code throws an exception, catch steps in with an alternative set of code. It has one parameter: the error object. Although it is optional, you are not handling the error if you do not catch an error. 

### FINALLY
The content of the finally code block will run either way -whether the try block succeed or fail. It even runs if a return keyword is used in the try or catch block. It is sometimes used to clean up after the previous two clauses.

If you try to use a string in a mathematical operation (other than in addition), you do not get an error, you get a special value called **NaN** (not a number).