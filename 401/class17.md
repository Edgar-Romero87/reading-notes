# TCP Servers

1. **Given the examples of front-end events such as button click, window resize, form submit, etc, what are some examples of back-end events?**

Bearer Authentication, event in response to a login request. 
Emit, which causes all callbacks registered to the event to 'fire', (get called)

2. **Why are events sometimes better than asynchronous actions with callbacks?**

A callback is a procedure you pass as an argument to another procedure. The procedure receiving the parameter can call it, or share it so some other procedures in the system can call it. An event handler is a procedure called when an event happens.

3. **What does an EventEmitter instance do?**

All objects that emit events are instances of the EventEmitter class. These objects expose an eventEmitter. on() function that allows one or more functions to be attached to named events emitted by the object.

4. **When is a program’s call stack, event queue, and event loop active?**

When it is activated by an asynchronous event.

## Vocabulary Terms

### Observer Pattern
The Observer Pattern is a popular pattern used across all sorts of JavaScript applications. The instance (subject) maintains a collection of objects (observers) and notifies them all when changes to the state occur.
### Listener
An event listener is a procedure in JavaScript that waits for an event to occur. A simple example of an event is a user clicking the mouse or pressing a key on the keyboard.
### Event Handler
A function or method containing program statements that are executed in response to an event. An event handler typically is a software routine that processes actions such as keystrokes and mouse movements. With Web sites, event handlers make Web content dynamic.
### Event Driven Programming
Simply put, event-driven programming is when a program is designed to respond to user engagement in various forms. It is known as a programming paradigm in which the flow of program execution is determined by “events.” Events are any user interaction, such as a click or keypress, in response to prompt from the system.
### Event Loop
When you create a button and attach an action(like async timeout or ajax) with it. When you clicked that button multiple times their actions are stored on the event loop and execute one by one.
### Event Queue
The event queue is responsible for sending new functions to the track for processing. It follows the queue data structure to maintain the correct sequence in which all operations should be sent for execution.
### Call Stack
Responsible for keeping track of all the operations in line to be executed. Whenever a function is finished, it is popped from the stack.
### Emit/Raise/Trigger
Emit() is used to fire events - Triggers signal that an action was completed.
### Subscribe
Subscribe itself to the observable of interest (which is getTasks() in your case) and wait until it is successful and then execute the first passed callback function
### Database
A database is a data structure that stores organized information. Most databases contain multiple tables, which may each include several different fields.