# jQuery, Events, and The DOM

## JQuery
jQuery offers a simple way to achieve a variety of common  JavaScript was quickly and consistently, across all major browsers and without any fallback code needed.

### What is jQuery?
jQuery is a JavaScript file that you include I your web pages. It lets you find elements using CSS-style selectors and then do something with the element using jQuery methods.

1- Find elements using CSS-style selectors.
A function called jQuery( ) lets you find one or more elements in the page. It creates and inject called jQuery with holds references to those elements. $( ) is often used as a shorthand to save typing jQuery( ).

### Similarities to the DOM 
- jQuery selectors perform s similar task to traditional DOM queries, but the syntax is much simpler.
- You can store the jQuery object in a variable, just just as you can with DOM nodes.
- You can use jQuery methods and properties ( like DOM methods and properties) to manipulate the DOM nodes that you select.

The jQuery object has many methods that you can use to work with the elements you select.

2- Do something with the elements using jQuery methods.  

### Key differences from the DOM

- It’s cross browser, and there’s no need to write fallback code.
Selecting elements its simpler and its more accurate.
- Event handling its simpler as it uses one method that works in all major browsers.
- Methods affect all the select elements without the need to loop through each one.
- Additional methods are provided for popular required tasks such as animations.
- Once you have made a selection, you can apply multiple methods to it.

## Why use JQuery?
JQuery doesn’t do anything you cannot achieve with pure JavaScript. It is just a JavaScript file but estimates show it has been used on over a quarter of the sites on the web, because makes code simpler. 


## A matched Set/ jQuery selection
When you select on or more elements, a jquery object is returned. It is also known as a matched set or a jquery selection.

Single element:
 $(‘ul’) this selector picks the < ul > element from the page. So the jquery object contains a reference to just one node.

Multiple elements:
$(‘li’) this selector pics all the < li > elements.  Here, the jquery object has references for each of the nodes that was selected.

## JQuery methods that get and set data
Some jQuery methods both retrieve information from, and update the contents of, elements. But they do not always apply to all elements.

- Get information
If a jquery selection holds more than one element, and a method is use to get information from the selected elements, it will retrieve information from only the first element in the matched set.

- Set information 
If a jquery  selection holds more than one element, and a method is used to update information on the page, it will update all of the elements in the matched set, not just the first one.

## Jquery objects store references to elements
When you create a selection with jquery, it stores a reference to them corresponding nodes in the DOM tree. It does not create copies of them.

## Coaching jquery selections in variables
A jquery object stores references to elements. Coaching jquery object stores a reference to it in a variable.


# DOM: Document Object Model
The browser represents the page using a DOM tree. DOM trees have four types of nodes:
* Document Nodes
* Element Nodes
* Attribute Nodes
* Text Nodes

You can select element nodes by their id or class attributes, by tag, or using CSS selector syntax.
Whenever a DOM query can return more than one node, it will always return a NodeList. From an element node you can access and update its content using properties such as textContent and innerHTML or using DOM manipulation techniques. An element node can contain multiple text nodes and child elements that are siblings of each other. In older browsers, implementation of the DOM is inconsistent (and is popular reason for using jQuery). Browsers offer tools for viewing the DOM tree.

# 6 Reasons for Pair Programming
- Pair Programming involves one person speaking out loud and "navigating" while the other person is "driving" and inputting what's spoken into the computer.
- PP is more efficient because it's easier for both users to catch mistakes in the code. It takes a little longer, but it produces high quality code that won't require a ton of troubleshooting or debugging later.
- The whole purpose of PP is collaboration. Students who work together learn from each other, and collaboration helps improve social skills. People could have different coding styles and still work well together if they have good communication.
- Programmers already familiar with PP have an advantage both at the job interview and on the first day of the job after hire. Recruiters want to know that they're hiring someone with good communication skills who works well with others.
