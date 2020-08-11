# Online Readings

## [Sending Form Data](https://developer.mozilla.org/en-US/docs/Learn/HTML/Forms/Sending_and_retrieving_form_data)

**Sending Form Data**
* Client/server architecture
  - A client (usually a web browser) sends a request to a server (most of the time a web server, using the HTTP protocol. The server answers the request using the same protocol.
  - HTML form on a web page is a convenient user-friendly way to configure an HTTP request to send data to a server. This enables the user to provide information to be delivered in the HTTP request.
* Client side: defining how to send the data
  - form element defines how the data will be sent.
  - Its attributes are designed to let you configure the request to be sent when a user hits a submit button. Attributes: action and method.
  - Action attribute defines where the data gets sent. Its value must be a valid relative or absolute URL. The names and values of the non-file form controls are sent to the server as name=value pairs joined with ampersands.
      * Action value should be a file on the server that can handle the incoming data. The server then responds, generally handling the data and loading the URL defined by the action attribute, causing a new page load.
  - Method attribute defines how data is sent. HTML form data can be transmitted via a number of different methods, the most common being the GET method and the POST method.
  -  GET method - the method used by the browser to ask the server to send back a given resource.
  - POST method - the method the browser uses to talk to the server when asking for a response that takes into account the data provided in the body of the HTTP request.
* HTTP requests are never displayed to the user.
* Server side: retrieving the data
  - The server receives a string that will be parsed in order to get the data as a list of key/value pairs. The way you access this list depends on the development platform you use and on any specific frameworks you may be using with it.
  - PHP offers some global objects to access the data.
* Languages and frameworks
  - Django for Python
  - Express for Node.js
  - Laravel for PHP
  - Ruby On Rails for Ruby.
* Sending files with HTML forms: Files are binary data because HTTP is a text protocol.
  - Enctype attribute - lets you specify the value of the Content-Type HTTP header included in the request generated when the form is submitted. HTTP header tells the server what kind of data is being sent.
* Security issues
  - HTML forms are the most common server attack vectors, but its due to how the server handles data.
  - Never trust your users. All data that comes to your server must be checked. Escape potentially dangerous characters. Limit the incoming amount of data to allow only what's necessary. Sandbox uploaded files.

## [HTML5 Forms Reference](https://htmlreference.io/forms/)

**HTML5 Forms Reference**
* 

## [Video Series on Styling HTML5 Forms](https://www.youtube.com/playlist?list=PL4cUxeGkcC9g5_p_BVUGWykHfqx6bb7qK)

**Styling HTML5 Forms**
* Video Notes
  - 
  - 
  - 
  - 
  - 
  - 
  - 
  - 
  - 

