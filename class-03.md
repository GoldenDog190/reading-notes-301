# Online Readings

## [Templating with Mustache](https://medium.com/@1sherlynn/javascript-templating-language-and-engine-mustache-js-with-node-and-express-f4c2530e73b2)

**JavaScript Templating**
* Fast and efficient technique to render client-side view templates with Javascript by using a JSON data source.
* Template is HTML markup, with added templating tags that will either insert variables or run programming logic.
* The template engine then replaces variables and instances declared in a template file with actual values at runtime, and convert the template into an HTML file sent to the client.

**Mustache**
* Mustache is a logic-less template syntax that can be used for HTML, config files, etc...
* Referred to as “logic-less” because there are no if statements, else clauses, or for loops. Instead, there are only tags. Some tags are replaced with a value, some nothing, and others a series of values.
* mustache.js is an implementation of the mustache template system in JavaScript.
* Mustache syntax: {{}}
* Mustache is not a templating engine, but a specification for a templating language. 

**Mustache-Express**
* Mustache Express lets you use Mustache and Express together easily. If you intend you use mustache with Node and Express, you can use mustache-express.
* To install use yearn or npm. Then configure mustache-express in your server.js/app.js/index.js file. Create a views folder and add some html view templates. Then in the router configuration, use res.render(TEMPLATE_NAME, JSON_DATA).


## [A Guide to Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)

**Properties for the Parent (flex container)** 
* Diplay - This defines a flex container; inline or block depending on the given value. It enables a flex context for all its direct children.
* Flex-direction - This establishes the main-axis, thus defining the direction flex items are placed in the flex container. Flexbox is a single-direction layout concept. Think of flex items as primarily laying out either in horizontal rows or vertical columns.
* Flex-wrap - Flex items will all try to fit onto one line by default. Can change that and allow the items to wrap as needed with this property.
* Flex-flow - Shorthand for the flex-direction and flex-wrap properties, which together define the flex container’s main and cross axes. The default value is row nowrap.
* Justify-content - Defines the alignment along the main axis. It helps distribute extra free space leftover when either all the flex items on a line are inflexible, or are flexible but have reached their maximum size. It also exerts some control over the alignment of items when they overflow the line.
* Align-items - Defines the default behavior for how flex items are laid out along the cross axis on the current line. Think of it as the justify-content version for the cross-axis.
* Align-content - Aligns a flex container’s lines within when there is extra space in the cross-axis, similar to how justify-content aligns individual items within the main-axis.

**Properties of the Child (flex items)**
* Order - Flex items are laid out in the source order. The order property controls the order in which they appear in the flex container.
* Flex-grow - Defines the ability for a flex item to grow if necessary. Accepts a unitless value that serves as a proportion. Dictates what amount of the available space inside the flex container the item should take up.
* Flex-shrink - Defines the ability for a flex item to shrink if necessary.
* Flex-basis - Defines the default size of an element before the remaining space is distributed. It can be a length or a keyword. 
* Flex - This is the shorthand for flex-grow, flex-shrink and flex-basis combined. 
* Align-self - This allows the default alignment to be overridden for individual flex items.

## [Flexbox Froggy](https://flexboxfroggy.com/)
**Tutorial Answers**
* Level 1: justify-content:flex-end;
* Level 2: justify-content: center;
* Level 3: justify-content: space-around;
* Level 4: justify-content: space-between;
* Level 5: align-items: flex-end;
* Level 6: justify-content: center;
           align-items: center;
* Level 7: justify-content: space-around;
           align-items: flex-end; 
* Level 8: flex-direction: row-reverse;
* Level 9: flex-direction: column;
* Level 10: flex-direction: row-reverse;
            justify-content: flex-end;
* Level 11: flex-direction: column;
            justify-content: flex-end;
* Level 12: flex-direction: column-reverse;
            justify-content: space-between;
* Level 13: flex-direction: row-reverse;
            justify-content: center;
            align-items:flex-end;
* Level 14: order: 1;
* Level 15: order: -1;
* Level 16: align-self: flex-end;
* Level 17: order: 1;
            align-self: flex-end;
* Level 18: flex-wrap: wrap;
* Level 19: flex-direction: column;
            flex-wrap: wrap;
* Level 20: flex-flow: column wrap;
* Level 21: align-content: flex-start;
* Level 22: align-content: flex-end;
* Level 23: flex-direction: column-reverse;
            align-content: center;
* Level 24: justify-content: center;
            align-content: space-between;
            flex-direction: column-reverse;
            flex-wrap: wrap-reverse;

## [Mustache.js Official Documentation](https://github.com/janl/mustache.js)

**mustache.js**
* mustache.js is a zero-dependency implementation of the mustache template system in JavaScript.
* Mustache is a logic-less template syntax. It can be used for HTML, config files, source code, etc... It works by expanding tags in a template using values provided in a hash or object.
* We call it "logic-less" because there are no if statements, else clauses, or for loops. Instead there are only tags. Some tags are replaced with a value, some nothing, and others a series of values.
* You can use mustache.js to render mustache templates anywhere you can use JavaScript. This includes web browsers, server-side environments such as Node.js, and CouchDB views.
* Install with npm
* A mustache template is a string that contains any number of mustache tags. Tags are indicated by the double mustaches that surround them. 

**Variables**
* The most basic tag type is a simple variable. 
* All variables are HTML-escaped by default.
* If you'd like to change HTML-escaping behavior globally, you can override Mustache's escape function.
* JavaScript's dot notation may be used to access keys that are properties of objects in a view.

**Sections**
* Sections render blocks of text zero or more times, depending on the value of the key in the current context.
* A section begins with a pound and ends with a slash. 

**Invereted Section**
* Inverted section opens with {{^section}} instead of {{#section}}. The block of an inverted section is rendered only if the value of that section's tag is null, undefined, false, falsy or an empty list.

**Pre-parsing & Caching Templates**
* By default, when mustache.js first parses a template it keeps the full parsed token tree in a cache. The next time it sees that same template it skips the parsing step and renders the template much more quickly. If you'd like, you can do this ahead of time using mustache.parse.

**Command line tool**
* mustache.js is shipped with a Node.js based command line tool. It might be installed as a global tool on your computer to render a mustache template of some kind.
* The command line tool is basically a wrapper around Mustache.render.

