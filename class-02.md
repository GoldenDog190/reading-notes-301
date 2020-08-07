# Ducket - HTML & CSS / JavaScript & JQuery Notes

## JavaScript and jQuery book by Jon Duckett pages 293-301, 306-331 and 354-357

**jQuery**
* *jQuery* is a JavaScript file that you include in your web pages. It lets you find elements using CSS-style selectors and then do something with the lelments using jQuery methods. 
  - $() is a shorthand for jQuery() function
* The jQuery object has many methods that you can use to work with the lelments you selected. The methods represent tasks that you commonly need to perform with elements.
  - The object and the elements it contains is refered to as a matched set or a jQuery selection.
  - Can use the methods of the jQuesry object to update the elements that it contains.
  - The member operator (.) indicates that the method on the right should be used to update the elements in the jQuery object on the left.
  - Each method has parameter that provide details about how to update elements
* In order to use jQuery, the 1st thing you need todo id include the jQuery script in your page. Next a second JavaScript file is included that uses jQuery selectors and methods to update the content of the HTML page. 
* jQuery is more simpler and shorter than JavaScript, and does the exact same thing as JavaScript.
  - Simple Selectors
  - Common tasks in less code
  - Cross-browser compatibility
* jQuery allows you to "write less, and do more," because it allows you to achieve the same goals but in few lines of code.
* A matched set/ jQuery selection
  - When you select one or more elements, a jQuery object is returned. Its also known as matched set/ jQuery selection
  - If selector returns single element, the jQuery object contains a refernce to one element node.
  - If selector returns seberal elements, the jQuery object contains reference to each element.
  * Some jQuery methods both retrieve info. from, and update the contents of elements, but they don't always apply to elements
  * jQuery objects store references to elements
    - When you create a selection with jQuery, it stores a reference to the corresponding nodes in the DOM tree, and doesn't create copies of them.
  * Caching jQuery selections in variables
    - A jQuery object stores references to elements. Caching a jQuesry object stores a reference to it in a variable.
  * Implicit iteration - the ability to update all of the elements in the jQuery slection.
  * Chaining - the process of placing several methods in the same selector.
  * jQuery .ready() method checks that the page is ready for your code to work with.
  * .html() and .text() methods both retrieve and update content of elements. 
  * Methods used to update elements
    - .html()
    - .text()
    - .replaceWith()
    - .remove()
  * Inserting elements 2 steps: create the new elements in jQuery object, and then use a method to insert the content into the page.
    - .before()
    - .after()
    - .prepend()
    - .append()
  * Can create attributes, or access and update their contents using:
    - .attr()
    - .removeAttr()
    - .addClass()
    - .removeClass()
  * .css() method lets you retrieve and set values of CSS properties.
  * jQuery allows you to recreate the functionality of a loop on a selection of elements, using the .each() method. As the .each90 method goes through elements in a selection, you can access the current element using this or $(this) keyword.
  * .on() method is used to handle all events.
  * Every event handling function recieves an event object. It has methods and properties related to the event that occured.
  * .on() method has 2 optional properties that let you filter the initial jQuery selection to respond to a subset of elements; pass information into the event handler using object literal notation.
  * Place the scripts for jQuery at the end of the page before the closing body tag. 

## [6 Reasons for Pair Programming](https://www.codefellows.org/blog/6-reasons-for-pair-programming/)

**6 Reasons for Pair Programming**
* Greater efficiency
* Engaged collaboration
* Learning from fellow students
* Social skills
* Job interview readiness
* Work enviroment readiness

## JavaScript and jQuery book by Jon Duckett pages 332-335

**Effects**
* When you start using jQuery, the effects methods can enhance your web page with transitions and movement. 
  - Basic effects
  - Fading effects
  - Sliding effects
  - customs effects
* .animate() method allows you to create some of your own effects and animations by changing CSS properties.

## JavaScript and jQuery book by Jon Duckett pages 302-305

**Finding Elements**
* Using jQuery, you usually select elements using CSS-style selectors. It also offers some extra selectors.
  - Basic Selectors
  - Hierarchy
  - Basic Filters
  - Content Filters
  - Visibility Filters
  - Child Filters
  - Atrribute Filters 
  - Form 