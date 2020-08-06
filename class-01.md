# Online Readings - SMACSS and Responsive Web Design

## [Shay Howe's intro to RWD](https://learn.shayhowe.com/advanced-html-css/responsive-web-design/)

**Responsive Web Design(RWD)**
* *RWD* is the practice of building a website suitable to work on every device and screen size.
* RWD term itself was coined and developed by Ethan Macotte.

**Responsive vs. Adaptive vs. Mobile**
* *Responsive* means to react quickly and positively to any change. Responsive design websites have continually and fluidly change based on factors, such as viewport width.

* *Adaptive* means to be easily modified for a new purpose or situation, such as change. Adaptive websites are built to group of preset factors.

* A combination of responsive and adaptive is ideal for a website.

* *Mobile* means to build a seperate website commonly on a new domain soley for moble users.

**Flexible Layouts**
* RWD has three main components: flexible layouts, media queries, and flexible media

* *Flexible layout* is the practice of building the layout of a website with a flexable grid, capable of dynamically resizing to any width. Do not advocate use of fixed measurement units, such as pixels or inches. 
  - Formula to help identify the proportions of a flexable layout using relative values. Formula based around taking the target width of an element and dividing it by the width of it's parent element: target/context = result.

* *Flexible grids* are built using relative length units: percentages or em units. These relative lengths are then used to declare common grid property values: width, margin, or padding.

* Relative viewport lengths introduced by CSS3: vw, vmin, vh, vmax.

* *Media Queries* built as an extension to media types commonly found when targeting and including styles. Provides the ability to specify different styles for individual browser and device circumstances, for example the width of the viewport or device orientation.
  - Ways to use media queries: use @media rule inside of existing style sheet, importing a new style sheet using @import, or by linking to a separate style sheet from within HTML document.
  - Media types: all, screen, print, tv, braille, 3d-glasses
  - Logical operators of media queries: and, not, only
  - and logical operator allows extra conditions to be added
  - not logical operator negates the query
  - only logical operator is a new operator and is not recognized by user agents using HTML4 algorithm
  - Media features identify what attributes or properties will be targeted within the media query expression. Most common media feature is determining height or width for a device or browser viewport. Other types of media features include orientation, aspect ratio, pixel ratio, resolution ratio, and other features include color and scanning.

* *Mobile first* approach includes using styles targeted at smaller viewports as the default styles for a website, then use media queries to add styles as the viewport grows.

* *Viewport* meta tag is used to assist in the displaying of a website. The values that are used with viewport are height and width, scale, and resolution values. These values can be combined.

* *Flexible Media*

## [All About Floats](https://css-tricks.com/all-about-floats/)

**All About Floats**

## [Don't Overthink It Grids](https://css-tricks.com/dont-overthink-it-grids/)

**Don't Overthink It Grids**

## [CSS Floats Explained By Riding An Escalator](https://www.freecodecamp.org/news/css-floats-explained-by-riding-an-escalator-57fa55232333/)

**CSS Floats Explained By Riding An Escalator**

## [SMACSS Offical Documentation](http://smacss.com/)

**SMACSS**