 # HTML Text, CSS Introduction, and Basic JavaScript Instructions

 When creating a web page, you add tags (known as markup) to the contents of the page. These tags provide extra meaning and allow browsers to show users the appropriate structure of a page. 
 
 HTML elements are used to describe the structure of the page (e.g. headings, subheadings, paragraphs).

Headings **< h1 > < h2 > < h3 > < h4 >**
Paragraphs **< p >**

They also provide semantic information (e.g. where emphasis should be placed, the definition of any acronyms used, when given text is a quotation).

Bold **< b >** & Italic **< i >** 

Superscript **< sup>** & Subscript **< sub>**
Line breaks **< br />** & Horizontal rules **< hr />**

Strong **< strong>** & Emphasis **< em>**
Quotations **< blockquote> < q>**
Abbreviations & Acronyms **< abbr>** 
Citations **< cite>** & Definitions **< dfn>**

Author Details **< address>**
Changes to Content **< ins> < del> < s>**

## CSS Introduction
- CSS treats each HTML element as if it appears inside its own box and uses rules to indicate how that element should look.
- Rules are made of *selectors* (that specify the elements the rules applies to) and *declarations* (that indicate what these elements should look like)
- Different types of selectors allow you to target your rules at different elements.
- Declarations are made up of two parts: the *properties* of the element of what you want to change, and the *values* of those properties. For example, the font-family property sets the choice of font, and the value arial specifies Arial as the preferred typeface.
- CSS rules usually appear in a separate document, although they may appear withn an HTML page.


## Basic JavaScript Instructions
- A script is made up of a series of statements. Each statementis like a step in a recipe. Statements should end with a semicolon(;).
- Scripts contain very precise intructions. For example, you might specify that a value must be rememebered before creating a calculation using that value.
- *Variables* are used to temporarily store pieces of imformation used in the scrip. A variable is a good name for this concept because the data stored in a variable can change (or vary) each time a script runs.
- *Arrays* are special types of variables that store more than one piece of related informaton. 
- JavaScript distinguishes between numbers (0-9), strings (text), and Boolean values (true or false).
- Expressions evaluate into a single value.
- Expressions rely on on operators to calculate a value.

## Decision Making
There are often several places in a script where decisions are made that determine wich lines of code should run next. In order to determine wich path to take, you set a **condition**.For example, you can check that one value is equal to another, greater than another, or less that another. If the condition returns **true**, you take one path; if it is **false**, you take another path.

## Comparison Operators:
You can evaluate a situation by comparing one value in the script to what you expect it may be. The result will be a Boolean: **true** or **false**. Comparison operators are used to compare to operands.

### == IS EQUAL TO


### != IS NOT EQUAL


### === STRICT EQUAL TO


### !== STRICT NOT EQUAL TO

### >  GREATER THAN 

### <   LESS THAN 

### >=  GREATER THAN OR EQUAL TO

### <=  LESS THAN OR EQUAL TO

## **LOGICAL OPERATORS**
Logical operatos allow you to compare the results of more than one comparison operator. Logical expresions are evaluated *left* to *right* if the first condition can provide enough information to get the answer, then there is no need to evaluate the second condition. 

### && LOGICAL AND

### || LOGICAL OR

### ! LOGICAL NOT 

# If Statement
The **If** statement evaluates (or checks) a condition. If the condition evaluates to **true**, any statement in the subsequent code block are executed.
