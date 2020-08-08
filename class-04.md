# Online Readings

## [CSS Grid Garden](https://cssgridgarden.com/)

**Grid Garden Tutorial Answers**
* Level 1: grid-column-start: 3;
* Level 2: grid-column-start: 5;
* Level 3: grid-column-end: 4;
* Level 4: grid-column-end: 2;
* Level 5: grid-column-end: -2;
* Level 6: grid-column-start: -3;
* Level 7: grid-column-end: span 2;
* Level 8: grid-column-end: span 5;
* Level 9: grid-column-start: span 3;
* Level 10: grid-column: 4 / 6; 
* Level 11: grid-column: span 3/5;
* Level 12: grid-row-start: 3;
* Level 13: grid-row: 3/6;
* Level 14: grid-column: 2;
            grid-row: 5;
* Level 15: grid-column: 2/6;
            grid-row: 1/6;
* Level 16: grid-area: 1 / 2 / 4 / 6;
* Level 17: grid-area: 2 / 3 / 5 / 6;
* Level 18: order: 5;
* Level 19: order: -1;
* Level 20: grid-template-columns: 50%;
* Level 21: grid-template-columns: repeat(8, 12.5%);
* Level 22: grid-template-columns: 100px 3em 40%;
* Level 23: grid-template-columns: 1fr 5fr;
* Level 24: grid-template-columns: 50px repeat(3, 1fr) 50px;
* Level 25: grid-template-columns: 75px 3fr 2fr ;
* Level 26: grid-template-rows: 50px 0 0 0 1fr;
* Level 27: grid-template: 60% 60% / 200px;
* Level 28: grid-template: 1fr 50px / 1fr 4fr; 

## [RegExr](https://regexr.com/)

**RegExr**
* RegExr is an online tool to learn, build, & test Regular Expressions (RegEx / RegExp).
  - Supports JavaScript & PHP/PCRE RegEx.
  - Results update in real-time as you type.
  - Roll over a match or expression for details.
  - Validate patterns with suites of Tests.
  - Save & share expressions with others.
  - Use Tools to explore your results.
  - Full RegEx Reference with help & examples.
  - Undo & Redo with cmd-Z / Y in editors.
  - Search for & rate Community Patterns.

## [Regex Tutorial](https://medium.com/factory-mind/regex-tutorial-a-simple-cheatsheet-by-examples-649dc1c3f285)

**Regex Tutorial**
* Regular expressions (regex or regexp) are extremely useful in extracting information from any text by searching for one or more matches of a specific search pattern.
* Fields of application range from validation to parsing/replacing strings, passing through translating data to other formats and web scraping.
* One of the most interesting features is that once you’ve learned the syntax, you can actually use this tool in almost all programming languages.
* Anchors: ^ and $
* Quantifiers: * + ? and {} ​​
* OR operator: | or []
* Character classes: \d \w \s and .
* Flags: g, m, and i
* Grouping and capturing: () 
* Bracket expressions: []
* Greedy and Lazy match
  - quantifiers ( * + {}) are greedy operators
  - use a ? to make it lazy
* Boundaries: \b and \B
* Back-references: \1
* Look-ahead and Look-behind: (?=) and (?<=)

## [Regex 101](https://regex101.com/)
* Website where you can test your code out.

## [CSS Grid Reference](https://css-tricks.com/snippets/css/complete-guide-grid/)

**A Complete Guide to CSS Grid**
* CSS Grid Layout is the most powerful layout system available in CSS.2-dimensional system, meaning it can handle both columns and rows, unlike flexbox which is largely a 1-dimensional system. Work with Grid Layout by applying CSS rules both to a parent element, which becomes the Grid Container and to that element’s children, which become Grid Items.
* When sizing rows and columns, you can use all the lengths you are used to, like px, rem, %, etc, but you also have keywords like min-content, max-content, auto, and perhaps the most useful, fractional units. Also have access to a function which can help set boundaries for otherwise flexible units.
* repeat() function can be used to save on typing.
* Properties for the Parent (Grid Container)
  - display - defines the element as a grid container and establishes a new grid formatting context for its contents.
  - grid-template-columns & grid-template-rows - defines the columns and rows of the grid with a space-separated list of values. The values represent the track size, and the space between them represents the grid line.
  - grid-template-areas - defines a grid template by referencing the names of the grid areas which are specified with the grid-area property. 
  - grid-template - shorthand for setting grid-template-rows, grid-template-columns, and grid-template-areas in a single declaration.
  - column-gap, row-gap, grid-column-gap, & grid-row-gap - specifies the size of the grid lines. You can think of it like setting the width of the gutters between the columns/rows.
  - gap & grid-gap - shorthand for row-gap and column-gap
  - justify-items - Aligns grid items along the inline (row) axis. This value applies to all grid items inside the container.
  - align-items - Aligns grid items along the block (column) axis. This value applies to all grid items inside the container.
  - place-items - place-items sets both the align-items and justify-items properties in a single declaration.
  - justify-content - This property aligns the grid along the inline (row) axis.
  - align-content - This property aligns the grid along the block (column) axis.
  - place-content - place-content sets both the align-content and justify-content properties in a single declaration.
  - grid-auto-columns & grid-auto-rows - Specifies the size of any auto-generated grid tracks.
  - grid-auto-flow - This property controls how the auto-placement algorithm works.
  - grid - shorthand for setting all of the following properties in a single declaration: grid-template-rows, grid-template-columns, grid-template-areas, grid-auto-rows, grid-auto-columns, and grid-auto-flow.
* Properties for the Children (Grid Items)
  - grid-column-start, grid-column-end, grid-row-start, & grid-row-end - Determines a grid item’s location within the grid by referring to specific grid lines. grid-column-start/grid-row-start is the line where the item begins, and grid-column-end/grid-row-end is the line where the item ends.
  - grid-column & grid-row - Shorthand for grid-column-start + grid-column-end, and grid-row-start + grid-row-end
  - grid-area - Gives an item a name so that it can be referenced by a template created with the grid-template-areas property. Alternatively, this property can be used as an even shorter shorthand for grid-row-start + grid-column-start + grid-row-end + grid-column-end.
  - justify-self - Aligns a grid item inside a cell along the inline (row) axis. This value applies to a grid item inside a single cell.
  - align-self - Aligns a grid item inside a cell along the block (column) axis. This value applies to the content inside a single grid item.
  - place-self - sets both the align-self and justify-self properties in a single declaration.

## [Responsive design with CSS Grid](https://medium.com/samsung-internet-dev/common-responsive-layouts-with-css-grid-and-some-without-245a862f48df)

**Common Responsive Layouts with CSS Grid (and some without!)**
* CSS grid lets us not only arrange elements in a row or a column, but in multiple rows and columns. 
*  Grid gives us control over how wide or narrow each of the ‘grid cells’ get. 
* object-fit: cover; - will stop the image from stretching, but it will cause cropping to happen
* grid-gap - This defines the size of the space between the columns and the rows. 
* Using the span value with a number will make a grid cell span that many rows, or columns. 
* Using break-inside: avoid; will stop your cards from being split across multiple columns.
* The ‘Holy Grail’ layout describes a page with a header and footer that stick at the top and bottom of the window respectively, and a content section that is split into two sidebars and the main content sits between them. 
  - body {
    display: grid;
    grid-template-columns: 200px 1fr 200px;
    grid-template-rows: auto 1fr auto;
    height: 100vh;
}