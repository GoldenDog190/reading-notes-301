# Online Reading

## [An Introduction to Node.js on sitepoint.com](https://www.sitepoint.com/an-introduction-to-node-js)

**What Is Node and When Should I Use It?**
* Node.js® is a JavaScript runtime built on Chrome’s V8 JavaScript engine.
* Node.js is an event-based, non-blocking, asynchronous I/O runtime that uses Google’s V8 JavaScript engine and libuv library.
  - The V8 engine is the open-source JavaScript engine that runs in Google Chrome and other Chromium-based web browsers, including Brave, Opera, and Vivaldi. Its responsible for compiling JavaScript directly to native machine code that your computer can execute.
  - Ryan Dahl, the creator of Node took the V8 engine and enhanced it with various features, such as a file system API, an HTTP library, and a number of operating system–related utility methods.
  - This means that Node.js is a program we can use to execute JavaScript on our computers.
* Installing Node.js:
  - Node Binaries - can be downloaded from official download page for your system.
  - Version Manager - is a program that allows you to install multiple versions of Node and switch between them at will. Advantages of it are it negates potential permission issues when using Node with npm and lets you set a Node version on a per-project basis.
  - Check that Node is installed with node -v
  - Create new .js file, and put a console.log(), which uses Node’s built-in console module to display a message in a terminal window. Then enter this command: node " your js file name". If running correctly the greeting or whatever you put in the console.log will be displayed.
* Node has excellent support for ECMAScript 2015 (ES6) 
  - Modern JavaScript featues:  template literals, object destructuring and Array.prototype.flatMap()
* Node comes bundled with a package manager called npm. To check which version you have installed on your system, type npm -v.
* Also, npm is the world’s largest software registry.
* Installing npm package globally:
  - Open terminal, and put: npm install -g jshint, which will install the jshint package globally on your system. 
* Installing npm package globally:
  - Create a test folder and open a terminal in that directory. Next type this: npm init -y, which will create and auto-populate a package.json file in the same folder. Next, use npm to install the lodash package and save it as a project dependency: npm install lodash --save. Create .js file, and put some code into it. Then run the script using node ".js file name".
* The folder entitled node_modules is where npm has saved lodash and any libraries that lodash depends on. The node_modules folder shouldn’t be checked in to version control, and can be re-created at any time by running npm install from within the project’s root. In the package.json file you will see odash listed under the dependencies field. By specifying your project’s dependencies in this way, you allow any developer anywhere to clone your project and use npm to install whatever packages it needs to run.
* Node.js and npm can be used for bundling your JavaScript files and dependencies into static assets, to running tests, or automatic code linting and style checking. To develop apps with modern JavaScript frame work you have to use Node and npm because these frameworks are all available via npm and rely on Node to create a sensible development environment in which they can run.
* Node.js plays a critical role in the technology stack of many high-profile companies.
* Node.js Execution Model:
  - Node.js is single-threaded, and event-driven, which means that everything that happens in Node is in reaction to an event. Node uses the libuv library to implement asynchronous/ non-blocking behavior. Capable of handling a large number of simultaneous connections, and has a built-in module to help a cloning strategy on a single server. The traditional approach to scaling a Node app is to clone it and have the cloned instances share the workload.
  - Node execution model in steps:
    1. Node apps pass async tasks to the event loop, along with a callback.
    2. The event loop efficiently manages a thread pool and executes tasks efficiently
    3. And executes each callback as tasks complete
* Downsides to Node.js: Limitated by running in a single thread, and the callback-based style of coding that JavaScript imposes.
* Node.js is suited to building applications that require some form of real-time interaction or collaboration, building APIs where you’re handling lots of requests that are I/O driven, or for sites involving data streaming.
* Advantages of Node.js: speed, scalability, no longer need to switch modes, can do everything in the same language, can easily share code between the server and the client, it speaks JSON, and JavaScript is ubiquitous.
* Other uses of Node.js: it can be used as a scripting language to automate repetitive or error prone tasks on your PC, can be used to write your own command line tool, and can be used to build cross-platform desktop apps and even to create robots.   