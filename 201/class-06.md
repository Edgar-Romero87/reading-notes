# Chapter 3: Object Literals

Objects group together a set of variables and functions to create a model of a something you would recognize from the real world. In an object:

If a variable is part of of an object, it is called a **Property**.

If a function is part of an object, it is called a **Method**.

Like variables and named fuctions, properties and methods have a name and value, in an object, that name is called **Key**.
Literal notations is the easiest and most popular way to create objects.

# Chapter 5: Document Object Model
The browser represents the page using a DOM tree.
DOM trees have four types of nodes: 
- Document Nodes
- Element Nodes
- Attribute Nodes
- Text Nodes 

You can select element nodes by their id or class attributes, by tag, or using CSS selector syntax.  
Whenever a DOM query can return more than one node, it will always return a **NodeList**.
From an element node you can access and update its content using properties such as *textContent* and *innerHTML* or using DOM manipulation techniques.
An element node can contain multiple text nodes and child elements that are siblings of each other.
In older browsers, implementation of the DOM is inconsistent (and is popular reason for using jQuery).
Browsers offer tools for viewing the DOM tree.