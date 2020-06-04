# REGEX and GRID

## Regex 
Is a string method.
Syntax: /--regex goes between these slashes--/

Some useful notes:

*- any character
\s - any space
\S - any non-space character
\w - any word character
\W - any non-word character
\d - any digit 
a? - 0 or 1 of a
a* - 0 or more of a
a+ - 1 or more of a
^ - start of a string
$ - end of a string

/hi/ => will match the first ‘hi’ that it finds

/hi/g => will match ALL ‘hi’’s that it finds

/hi/gi => will match ALL ‘hi’s and ‘HI’s that it find (case insensitive)

**g** look in the whole string.

Three methods that we use with regex:
- .test()
  * regex.test(str)
  * Returns true or false

- .match()
  * str.match(regex)
  * Returns an array of all the matches

- .replace()
  * str.replace(regex, thing to replace it with)
  * Returns the new string

## Grid
- Flex box is for 1 dimensional work
- Grid is for 2D

Grid Container: the parent container of everything in the grid.

Grid Item: the child inside the container

Grid Area

#### Properties of Parent
- display
  - grid
  - grid-inline
- grid-template-columns/grid-template-rows
  - track-size
  - line-name
- grid-template-areas
  - grid-area-name
- grid-template
  - shorthand
- justify-items
  - start
  - end
  - center
  - stretch
- align-items(start, end, center ,stretch)
- place-items
- justify-content (start, end, center ,stretch, space-around, space-between, space-evenly)
- align-content (start, end, center ,stretch, space-around, space-between, space-evenly)
- place content
- grid-auto-columns / grid-auto-rows
- grid-auto-flow
- grid

### Properties for the Children
- grid-column-start
- grid-column-end
- grid-row-start
- grid-row-end
- grid-column
- grid-row
- grid-area
- justify-self (start, end, center ,stretch)
- align-self (start, end, center ,stretch)
- place-self