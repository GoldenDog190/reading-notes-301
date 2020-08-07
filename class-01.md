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

* *Flexible Media* is the final important aspect of RWD, and it used to to change the size of media, such as videos, along with the rest of the website. One quick way to make media scalable is using max-width property with the value of 100%, but it doesn't work well around iframes and embedded media. For the embedded media the embedded element needs to be absolutely positioned within a parent element. The parent element needs to have a width of 100%. The parent element also needs to have a height of 0. Padding is then given the value of the same aspect ratio of the video.

## [All About Floats](https://css-tricks.com/all-about-floats/)

**All About Floats**
* *Float*: CSS property that makes the text flow around the images, and can be used to create entire web layouts. 
* Floated elements remain part of the flow of the web page. 
* In comparision, an absolute position page elements are removed from the flow of the webpage, adn will not affect the position of other elements and other elements will not affect them.
* Four valid float properties: left, right, none, and inherit
* Floats sister property is clear. When using the clear property, the element will not move up adjacent to the float like the float desires, but will move itself down past the float.
* Clear values: both, left and right, none, and inherit
* If parent element contained nothing but float elemts, the height of it would collapse into nothing.
* Other float clearing tools: the empty div method, the overflow method, and the easy clearing method 
* Problems with floats: pushdown, double margin bug, 3px jog, and bottom margin bug 

## [Don't Overthink It Grids](https://css-tricks.com/dont-overthink-it-grids/)

**Don't Overthink It Grids**
* Majority of websites use a grid, which is useful when dealing with complex layouts. 
* Context - can use div as a generic wrapper around block level element
* Columns - Start with practical or common need, for example pick a main content area, and make two column divs with class names. Don't over think it!
* Next clearing context
* Gutters - hardest part of grids, make the math simple, first step use box-sizing: border-box, set width, and apply fixed padding to columns.
* Outside gutters - add left padding to grid parent, and then restore right padding to last column.
* Can add more column choices, and use scss/compass
* Modules - work within grids with modules to help break up content. Each Module can have padding of it's own.

## [CSS Floats Explained By Riding An Escalator](https://www.freecodecamp.org/news/css-floats-explained-by-riding-an-escalator-57fa55232333/)

**CSS Floats Explained By Riding An Escalator**
* *Floats* create alternate flows. Once introduced you need to write your code so that it accounts for up to three flows: normal, left, and right.
* Floats are similar to riding an escalator. 
 - Gotta respect the passing lane: when not using floats its like riding an escaltor with everyone blocking the way and not letting any one passby. With a float elements can get by each other without blocking each others way.
 - Left and Right: using left and right float can introduce two new flows, which allows the normal flow of elements, without a float value to fill in the spaces around these elements. 
 - Floats allow you to create these new relationships between flows. Float property also gives indication of an elements relationship to surrounding elements.
* *Clear Property* allows elements to specify where they should align in comparison to the floated elements.
 - clear: left tells each element floating left that they should align themselves behind the first element that is floated left.
 - clear: both allows you to reset the flow of elements, as opposed to continuiung to maintain a right, left, and normal flow.

## [SMACSS Offical Documentation](http://smacss.com/)

**SMACSS(Scalable and Modular Architechure for CSS)**
* At the core of SMACSS is categorization. The 5 Types of Categories are: base, layout, module, state, and theme
  - Base rules are defaults, single element selectors, but could include attribute selectors, pseudo-class selectors, child selectors or sibling selectors. Doesn't include any class or ID selectors. Base styles include heading sizes, default link styles, default font styles, and body background.
    * CSS reset is a set of Base styles designed to stripout/ reset the default margin, padding, and other properties. Defines a consistent foundation across browsers to build the site on. 
  - Layout rules divide the page into sections. Layouts hold one or more modules together. There is a distinction between layouts dictating the major and minor components of a page. 
    * Major components are refered to as layout styles, and include the header and footer traditionally styled using ID slelctors.
    * Minor components, such as a login form, sit within the scope of major componenets. Refered to as modules.
  - Moldules are reusable, modular parts of our design, and the desrete component of the page. The callouts, sidebars sections, product list, etc... Sits inside of the layout components. Aviod using IDs and element selectors, use class names only!
  - State rules describe how modules or layouts will look in a particular state. Describing how modules or layouts look on screens big or small. A state is something that augments and overrides all other styles. Generally applied to the same element as a layout rule or applied to the same element as a base module class. Difference from modules: can apply to layout/ or module styles, and indicate a JavaScript dependency.
  - Theme rules are similar to state rules in they describe how modules or layouts might look. Defines colors and images that give site its look and feel. Can affect any of the primary types, override base styles, change module elements, alter how states look, or affect layout with different arrangements. 
   * Font rules will normally affect base, module, and state styles.
 - Naming Rules - by seperating the rules, naming convention is benefical to understand which category a particular style belongs to and its role within the overall scope of the page.
* State changes represented in one of three ways: class name, pseudo-class, and media query.
  - Class name change happens with JavaScript, for example mouse clicks or moves changing the color.
  - Pseudo-class can only style changes to elements that are descendants or siblings of element.
  - Media queries describe how things should be styled under defined criteria, such as different viewport sizes.

* Depth of Applicability
 - If you just use CSS as you would use it for a small site on a larger site, issues will pop up due to relying too heavily on a defined HTML structure, and the depth of HTML to which the selectors apply is too deep. 
 - Minimize depth with the HTML structure, otherwise components on page can't be moved around easily. Using the shollow depth of applicability approach is also the ability to more readily convert modules into templates for dynamic contnent.

 * CSS gets evaluated from right to left.
 * Three simple guidelines to help limit the number of elements that need to be evaluated: use child selectors, avoid tag selectors for common elements, and use class names as the right-most selector.
 * SMACSS approach has two core goals: increase the semantic value of a section of HTML and content, and decrease the expectation of a specific HTML structure.
 * SMACSS is about identifying patterns and codifying them. 
 * Prototype should assist in viewing components in part or in whole and to allow the codification of the design language into building blocks. Prototype goals: show states, review localization, and isolate dependencies. 
 * Preprocessor allows you to use a special syntax in your CSS that is then compiled within your project. Preprocessor features: variables,operations, mixins, nesting, functions, interpolation, file importing, extending.
 * CSS sprites have become a mainstay of modern web development—and for good reason. They allow for multiple assets to be compiled into a single resource, minimizing the number of HTTP requests and ensuring that images for things like rollover states are already loaded when needed.
 * Formatting code
   - Single line vs. multiple lines
   - Grouping properties
   - Color declarations 