# HTML Lists, CSS Boxes, JS Control Flow

## HTML Lists
There are 3 types of lists < li >: 
- Ordered < ol > Use numbers.

- Unordered < ul >Use bullets.

- Definition < dl >

Inside the < dl > element you will usually see pair of:
 
 < dt > Use to contain the term being defined.
 
 < dd > Used to contain the definition.

 Lists can be nested inside one another.

## CSS Boxes
- CSS treats each HTML element as if it has its own box.
- You can use CSS to control the dimension of a box.
- You can also control the boarders, margins and padding for each box with CSS.
- It is posible to hide elements using the display and visible properties.
- Block-level boxes can be made into inline boxes, and inline boxes made into block-level boxes.
- Legibility can be improved by controlling the width of boxes containing text and the leading.
- CSS3 has introduced the ability to create image boarders and rounded boarders.

## JS Control Flow
**if ... else** statements allow you to run one set of code if a condition its true, and another if a condition is false.

**Switch** statements allow you to compare a value againts possible outcomes (and also provides a default option if none match).

### **LOOPS**
loops check a condition. If it returns *true*, a code block will run. Then the condition will be check again and if still returns *true*, the code block will run again. It repeat until the condition returns *false*. there are three common types of loops: 

#### FOR 
If you need to run code a specific number of times, use a **for** loop.(Its the most common loop.) In a **for** loop the condition is usually a counter wich is used to tell how many times the loop should run.

#### WHILE
If you not know how many times the code should run, you can use a **while** loop. Here the conditions can be something other than a counter, and the code will continue to loop for as long as the condition is **true**.

#### DO WHILE
This loop is very similar as the while loop, but has one key difference: it will always run the statements inside the curly braces at least once, even if the condition evaluates as false.

**Keywords** -you commonly see these two keywords used with loops:
- **Break** -this keyword causes the termination of the loop and tells the interpreter to go on to the next statement of code outside thye loop.(You may also see it used in functions) 
- **Continue** -This keyword tells the interpreter to continue with the current iteration, and then check the condition again.(If it is true, the code runs again.)