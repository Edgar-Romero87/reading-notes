# HTML Links, CSS Layout, JS Functions

## Links
Links are the defining fetuare of the web because they allow you to move from one web page to another.
We commonly see this type of links:
- Links from one website to another.
- Links from one page to another on the same website.
- Links from one part of a web page to another part of the same page.
- Links that open in a new browser window.
- Links that start up you email program and address a new email to someone.

< a href="http://www. .com ">

Links are created using the < a >. you specify wich page you want to link to using *href* attribute. 

If you are linking to a page within your own site, it is best to use relative links rather than qualified URLs.
You can create links to open email programs with an email address in the "to" field.
You can use the id attribute to target elements within a page tha can be linked to.

## Layouts
- < div > elements are often used as containig elements to group together sections of a page.
- Browser display pages in normal flow unless you specify relative, absolute, or fixed positioning.
- The float property moves content to the left or right of the page and can be used to create multi-column layouts. (floated items requiere a defined width.) 
- Pages can be fixed width or liquid (strechy) layouts.
- Designers keep pages within 960-1000 pixels wide, and indicate what the site is about within the 600 pixels (to demostrate its relevance without scrolling).
- Grids help create professional and flexible designs.
- CSS frameworks provide rules for common task.
- You can include multiple CSS files in one page.


## Functions, Methods and Objects

### Functions & Methods
Functions consist of a series of statements that have been grouped together because they perform a specific task. A method is the same as an function, except methods are created inside (and are part of) an object.
If different parts of a script repeat the same task, you can reuse the function (rather than repeating the same set of statements).
Grouping together the statements, helps you organize your code.
To create a function, you give it a name and then write the statements needed to achieve its task inside the curly braces. This is know as a **function declaration**.
- You declare a function using the **function** keyword.
- You give the function a name (sometimes called an identifier) followed by parentheses.

Having declared the function, you can then execute all of the statements between the curly braces with just one line of code. This is know as **calling the function**.

#### Declaring Functions That Need Information
Sometimes a function needs specific information to perform its task. In such cases, when you declare the function you give it parameters. Inside the function, the parameters act like variables.

#### Calling Functions That Need Informtation.
When you call a function that has parameters, you specify the values it should use in the parentheses that follow its name. The values are called **arguments**, and they can be provided as values or as variables.

#### Getting a Single Value Out of A Function
Some function return information to the code that call them. For example, when they perform a calculation, they return the result.

#### Getting Multiple Values Out of A Function
Function can return more than value using an array. For example, this functons calculate the area and volume of a box.

## 6 Reason for Pair Programing
Pair programming is the practice of two developers sharing a single workstation to interactively tackle a coding task together. While there are many different styles, pair programming commonly involves two roles: the **Driver** and the **Navigator**. The Driver is the programmer who is typing and the only one whose hands are on the keyboard. The Navigator thinks about the big picture, what comes next, how an algorithm might be converted in to code, while scanning for typos or bugs. The Navigator might also utilize their computer as a second screen to look up solutions and documentation, but should not be writing any code.
1. Greater efficiency
2. Engaged collaboration
3. Learning from fellow students
4. Social skills
5. Job interview readiness
6. Work environment readiness

 At Code Fellows, pair programing is one way we foster a collaborative environment while developing key industry skills.

