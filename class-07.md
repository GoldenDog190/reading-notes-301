# Online Readings

## [What Google Learned From Its Quest to Build the Perfect Team](https://www.google.com/amp/mobile.nytimes.com/2016/02/28/magazine/what-google-learned-from-its-quest-to-build-the-perfect-team.amp.html)

* What Google Learned From Its Quest to Build the Perfect Team

  - Study groups are a big deal at M.B.A. programs, and the students to work together and come up with plans for businesses based on real data.
  - Team work and team composition is highly valued in todays companies, but so is improving the indivual worker in a pratice known as employee performance organization.
  - Groups that tend to work together innovate faster, see mistakes more quickly, and find better solutions to problems.
  - Google has been researching how to make the perfect team by examing how and why do some teams do better than others.
  - It was found that the norms within a group was a deciding factor in how well the group got along. Having the right norms and everyone treating each other well in a group allowed them to work together and get along.
  - Two main behaviors that a good team had were everyone talked about the same amount, which is refered to as conversational turn-taking, and had high average social sensitivity. Having both of these behaviors together creates the concept of psychological safety within the group.
  - Google decided to make an enviroment where people felt psychologically safe to make better teams, and to make teams that have members that listen to one another and show sensitivity to feelings and needs.

## [How I explained REST to my brother](https://gist.github.com/brookr/5977550)

**Conversation on REST**

* Ryan Tomayko - wrote first web servers that send documents across the internet, and researched about why the web works the way it does.
* http - tells the browser what protocol to use. and it is capable of describing the location of something anywhere in the world from anywhere in the world. It's the foundation of the web.
* REST - the whole world wide web is built on this architectural style, and provides a definition of a “resource”, which is what those things point to. 
* A web page is a “representation” of a resource, which are just concepts. 
* URLs tell the browser that there's a concept somewhere. A browser can then go ask for a specific representation of the concept. 
* A resource has only a single representation.
* Web Services or APIs - computers can use these same protocols to send messages back and forth to each other. 
* Redirect - one machine tell another machine about a resource that might be on yet another machine.
* Machines don't have a universal noun. Every programming language, database, or other kind of system has a different way of talking about nouns.  URLs let all of these systems tell each other about each other's nouns. 
* Polymorphism - Different nouns can have the same verb applied to them. Its a concept in programming and CS theory.
* HTTP - is about applying verbs to nouns. Example: when you go to a web page, the browser does an HTTP GET on the URL you type in and back comes a web page. 
* Machines just need data, and doesn't care about the layout or styling.

## [Documentation for SuperAgent](https://visionmedia.github.io/superagent/)

**SuperAgent**

* SuperAgent is light-weight progressive ajax API crafted for flexibility, readability, and a low learning curve after being frustrated with many of the existing request APIs. It also works with Node.js.
* Request basics - request can be initiated by invoking the appropriate method on the request object, then calling .then() (or .end() or await() to send the request. DELETE can be also called as .del()
* Setting header fields - Setting header fields is simple, invoke .set() with a field name and value.
* GET requests - The .query() method accepts objects, which when used with the GET method will form a query-string. Also accepts strings.
* HEAD requests - can use the .query() method for HEAD requests.
* POST / PUT requests - JSON POST request, where we set the Content-Type header field appropriately, and "write" some data.
* Setting the Content-Type - use the .set() method or .type() method.
* Serializing request body - SuperAgent will automatically serialize JSON and forms.
* Retrying requests - use the .retry() method, and SuperAgent will automatically retry requests. 
* Setting Accept - method .accept()
* Query strings - req.query(obj) is a method which may be used to build up a query-string.
* TLS options - Node.js SuperAgent supports methods to configure HTTPS requests: .ca(), .cert(), .key(), and .pfx().
* Parsing response bodies - SuperAgent will parse known response-body data for you
* Response properties: text, body, header fields, Content-Type, and status
* Timeouts - Set timeouts to avoid requests getting stuck.
* Authentication - .auth() method
* Following redirects - res.redirects(n) method
* Agents for global state: Saving cookies, and default options for multiple requests.
* Piping data - .pipe() 
* Multipart requests - methods .attach() and .field()
* Compression - node client supports compressed responses
* Buffering responses - req.buffer()
* CORS - .withCredentials() method enables the ability to send cookies from the origin.
* Error handling - callback function will always be passed two arguments: error and response
* Progress tracking - SuperAgent fires progress events on upload and download of large files.
* Testing on localhost: Forcing specific connection IP address using .connect() or ignoring broken/insecure HTTPS on localhost using .trustLocalhost().
* Promise and Generator support: SuperAgent's request is a "thenable" object that's compatible with JavaScript promises and the async/await syntax.
* Browser and node versions - SuperAgent has two implementations: one for web browsers and one for Node.JS. 

# API Keys Links - request personal keys and get them in your email, but do not post them on GitHub.

## [Geocoding API Docs](https://locationiq.com/)
## [Weather Bit API Docs](https://www.weatherbit.io/)
## [Yelp API Docs](https://www.yelp.com/developers/documentation/v3/business_search)
## [The Movie DB API Docs](https://developers.themoviedb.org/3/getting-started/introduction)
## [The Hiking Project API Docs](https://www.hikingproject.com/data)