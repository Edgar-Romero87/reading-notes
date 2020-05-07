# Layout
- Block-level- box
    Starts on a new line
- Inline box
    Is in line with the other elements
- Box inside a box
    The outside box is called the parent
    The inside called the child.
- Positioning Schemes:
    Normal flow
    Relative Positioning
    Absolute Positioning
    Fixed Positioning
    Floating Positioning

## Normal flow
- Position Static:
 Each block-level element sits on top of the next.This is the default so it's not necessary to use this property.
- Relative Positioning 
position: relative -Moves an element in relation to where it would have been in normal flow.
- Absolute Positioning
position: absolute -This takes the element out of its normal flow and no longer affects the position of other elements on the page. (Acts like it's not there.)
- Fixed Positioning
position: fixed -A type of absolute positioning that requires the position property to have a value of fixed. It keeps its position relative to the browser window.
- Overlapping Elements
If boxes overlap, the elements that appear later in the HTML code sits on top of those that are earlier.z - indextells the browser what is in front of what.
- Floating Elements
Allows you to take an element in normal flow and place it as far to the left or right of the containing element as possible.Anything else that sits inside the containing element will flow around the element that is floated.

- **Using Float** to place elements side-by-side the float property is commonly used to achieve this.
- **Clearing floats**
The clear property prevents elements, within the same containing element, should touch the left or right sides of a boxleft: left-hand side of the box should not touch any other elements appearing in the same containing elementright: right-hand side of the box should not touch any other elements appearing in the same containing elementboth: Neither sidenone: Elements can touch each other.
- **Parents of floated elements**
If a containing element only contains floated elements, some browsers will treat it as ifs 0 pixels tall.Old Solution: added an extra element after the last floated box (leaving and empty element in the HTML)New Solution: overflow: auto and width:100%
- **Multi-column with floats**
Position the columns next to each other.Widthfloatmargin.column1 { float: left; width: 620px; margin: 10px; } .column2 { float: left; width: 300px; margin: 10px; }.column1, .column2, .column3 { width: 300px; float: left; margin: 10px;}
- **Screen Sizes**
What device is your user going to use?Phone: 960x640
Tablet:1024x768
13" Laptop: 1280x800
27" Monitor:2560x1440
Standard Desktop version page size: 960-1000 pixels wide.
- **Fixed width layouts**
Design does not change with the user changes browser window size. (fixed pixel numbers)AdvantagesPixel values are accurateDesigner has greater control over the appearanceCan control the lengths of lines of textsize of an image will always remain the sameDisadvantagesCan end up with big gaps around the edgeIf the screen is a much here resolution the page can look smaller and text can be harder to readIf a user increases font sizes, text might not fit into the allotted spacesCan take up more vertical space.
- **Liquid Layouts**
Stretch and contract as the user changes browser window size (use of percentages)AdvantagesPage expand to fill the browser windowa user with a small window wont have to scroll to the side to see all the contentits tolerant of users change of font sizeDisadvantagespage can look different from what you expectedif the window is wide the text can stretchIf narrow words can be squashedimages can overflow
- **Layout GridsMany**: designers use a grid structure to help them position items on a page.Grids set consistent proportions and spaces between items.Creates a continuityHelp users predict where to find info on subsequent pages.Makes it easier to add new content to the site in a consistent wayHelps people collaborate example (Links to an external site.)
- **CSS Frameworks**: Aims to make your life easier by providing the code for common tasksAdvantagesSave time from rewriting codeHave been tested across different browsersDisadvantagesOften require that you use class names that only control the presentation of the pageOften contain more code than you need for your page. 960.gs (Links to an external site.) bootstrap (Links to an external site.)
- **Multiple Style Sheets**: possible reasons to use multiple1 sheet to control fonts and colors1 sheet to control layoutsCan use 1 <link> tag in HTML and in the main CSS use @import url("");or you can use multiple <link> in the HTML