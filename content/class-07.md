# HTML Tables; JS Constructor Functions

## Domain Modeling
Domain modeling is the process of creating a conceptual model in code for a specific problem. A model describes the various entities, their attributes and behaviors, as well as the constraints that govern the problem domain. An entity that stores data in properties and encapsulates behaviors in methods is commonly referred to as an object-oriented model.
A domain model that's articulated well can verify and validate the understanding of a specific problem among various stakeholders. As a communication tool, it defines a vocabulary that can be used within and between both technical and business teams.


## HTML Tables
The table < table > element is used to add tables to a web page. When representing information in a table, you need to think in therms of a grid made up of rod and columns (a bit like a spreadsheet).
A table is drawn out row by row. Each row is created with the < tr > element.
Inside each row there are a number of cells represented by the < td > element (or < th > if it is a header).
You can make cells of a table span more than one row or column using the rowspan  and colspan attributes.
For long tables you can split the table into a < thead >, < tbody >, and  < tfoot >.
JS Constructor Functions

### Creating an Object: Constructor notation 

The **new** keyword and the object constructor crate a blank object. You can then add properties and methods to the object.
First you create a new object using the combination of the **new** keyword and the **Object()** constructor function.

### Updating an Object

To update the value of properties, use dot notation or square brackets. They work on objects created using literal or constructor notation. To delete a property, use the **delete** keyword.

### Creating Many Objects: Constructor Notation

Sometimes you will want several objects to represent similar things. Object constructor can use a function as a **template** fr creating objects. First create the template with the object’s properties and methods.
-The function has three parameters. Each one sets the value of a property in the object. The methods will be the same for each object created using this function.
You create **instances** of the object using the constructor function. The new keyword followed by a call to the function creates a new object. The properties of each object are given as arguments to the function.

### Arrays are Objects

Arrays are actually a special type of object. They hold a related set of key/value pairs (like all objects), but the key for each value is its index number.

### Arrays of Objects & Objects in Arrays

You can combine arrays and objects to create complex data structures: Arrays can store a series of objects (and remember their order).
Objects can also hold arrays (as value of their properties).

### Creating an Instance of the Date Object

In order to work with dates, you creat an instance of the **Date** object. You can then specify the time and date that you want it to represent. To create a **Date** object, use the **Date ()** object constructor.  