# Online Readings

## [EJS Partials](https://medium.com/@henslejoseph/ejs-partials-f6f102cb7433)

**EJS Partials**
* Partials - can reuse the same HTML across multiple views. Think of them as functions, make large websites easier to maintain as you don’t have to go and change a piece of text in every page it appears in. Instead, you define that reusable bundle of code in a file and include it wherever you need it.
* When making a partial, create a ejs file that will contain only HTML for the partail you are defining, and now you can use the partails in your other ejs templates. 
  - In EJS, any JavaScript or non-HTML syntax you include in your templates is always surrounded by <% %> delimiters. Use this for a partial in EJS, which is where the partial file is relative to the template you use it in: <%- include( PARTIAL_FILE ) %>
  - The <%- %> tags allow us to output the unescaped content onto the page (notice the -). This is important when using the include() statement since you don’t want EJS to escape your HTML characters like ‘<’, ‘>’, etc…
* Next create the homepage template and include the partial you created in it.

## [Watch EJS tutorial from WalkThroughCode on YouTube, Video 7, Partials](https://www.youtube.com/watch?v=3_xEEH4fTEk&t=0s&index=7&list=PL7sCSgsRZ-slYARh3YJIqPGZqtGVqZRGt)

**Video Notes**
* Video Notes
  - 
  - 
  - 
  - 