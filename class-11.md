# Online Readings

## [Watch EJS tutorial from WalkThroughCode on YouTube, Videos 1-5](https://www.youtube.com/playlist?list=PL7sCSgsRZ-slYARh3YJIqPGZqtGVqZRGt)

**Video Notes**
* Video 1 Notes
  - 
  - 
  - 
  - 
  - 
* Video 2 Notes
  - 
  - 
  - 
  - 
  - 
* Video 3 Notes
  - 
  - 
  - 
  - 
  - 
* Video 4 Notes
  - 
  - 
  - 
  - 
  - 
* Video 5 Notes
  - 
  - 
  - 
  - 
  - 

## [Google Books API Docs](https://developers.google.com/books/docs/v1/using#WorkingVolumes)

**Working with volumes**
* Perform a volumes search by sending an HTTP GET request to the following URI: https://www.googleapis.com/books/v1/volumes?q=search+terms
* This request has a single required parameter:
  - q : search for volumes that contain this text string. Special keywords you can specify in the search terms to search in particular fields, such as: intitle, inauthor, inpublisher, subject,  isbn, lccn, and oclc.
* Can use standard query parameters or optional query parameters, such as download, filter, pagination, printType, projection, and sorting.
* Can retrieve information for a specific volume by sending an HTTP GET request to the Volume resource URI: https://www.googleapis.com/books/v1/volumes/volumeId
* accessInfo section - determines what features are available for an eBook. 
* For this you can use standard query parameters or optional query parameter, such as projection.

## [EJS Docs](http://ejs.co/)
**EJS (Embedded JavaScript Templating)**
* EJS - templating language that lets you generate HTML markup with plain JavaScript. 
  - Can use plain JavaScript
  - Fast development time
  - Simple syntax
  - Speedy execution
  - Easy debugging
  - Active development
* EJS features:
  - Fast compilation & rendering
  - Simple template tags
  - Custom delimiters
  - Sub-template included
  - Ships with CLI
  - Both serve JS & browser support
  - Static caching of intermediate JS and templates
  - Complies with the Express view system  

## [EJS Tutorial](https://scotch.io/tutorials/use-ejs-to-template-your-node-application)

**Use EJS to Template Your Node Application**
* Test Application
  - File Structure:
    - views
    ----- partials
    ---------- footer.ejs
    ---------- head.ejs
    ---------- header.ejs
    ----- pages
    ---------- index.ejs
    ---------- about.ejs
    - package.json
    - server.js
  - Node Setup in package.json
    {
    "name": "node-ejs",
    "main": "server.js",
    "dependencies": {
        "ejs": "^1.0.0",
        "express": "^4.6.1"
    }
}
  - Then install npm, and make a index page
  - Define application in server.js file, and set EJS as the view engine for our Express application.
  - Start up server using: $ node server.js
  - EJS Partials - code that is reused in an application. Example files: footer.ejs, head.ejs, header.ejs
  - Pass data to views
  - Echo a single variable
  - Loop over the data
* EJS doesn't support the ability to have layouts. 

## [Source Code for the EJS Tutorial](https://github.com/scotch-io/node-ejs)
* Use this to review code that goes along with the EJS tutorial above to get a better understanding of the code.