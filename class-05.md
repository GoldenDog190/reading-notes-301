# Online Readings

## [Heroku: Getting Started with Node](https://devcenter.heroku.com/articles/getting-started-with-nodejs#introduction)
**Introduction**
* This tutorial will have you deploying a Node.js app to Heroku.
**Set Up**
* In this step you’ll install the Heroku Command Line Interface (CLI). You use the CLI to manage and scale your applications, provision add-ons, view your application logs, and run your application locally.
**Prepare the app**
* In this step, you will prepare a sample application that’s ready to be deployed to Heroku.
**Deploy the app**
* In this step you will deploy the app to Heroku. Create an app on Heroku, which prepares Heroku to receive your source code. When you create an app, a git remote (called heroku) is also created and associated with your local git repository.
**View logs**
* To view info. about your running app using: heroku logs --tail 

## [Deploying a Simple Blog to Heroku](https://howtonode.org/deploy-blog-to-heroku)
**Node.js For Beginners. Deploy Your Blog to Heroku**
* Node.js is an open source, cross-platform runtime environment, which allows you to build server-side and networking applications. It's written in JavaScript and can be run within the Node.js runtime on any platform. 
* To create a server - First of all, we need to create a JavaScript file. Run at your terminal: node server.js. Then check it in your browser. Deploy server online. 
* Node allows you to use the so-called event loop, which works faster because of non-blocking behavior.
* WWW is for "World Wide Web" and we will turn your local server into a world wide server. 
* Make it world wide using the Heroku cloud application platform. Heroku is a cloud platform as a service, and allows you to deploy your web server, so everyone could see how awesome you are as a web developer. 
* Install Heroku, create project directory, and then create the server.js file inside it. Declare some variables: first one will give you the key to Node's HTTP functionality, second one is for possibility to interact with the file system, third one allows you to handle file paths, and last one allows you to determine a file's MIME-type. Create the package.json file and fill it with proper information. Use built-in Node Package Manager to download it, and it will create node_modules folder and place all the files inside of it. Create send404() function, and it will handle the sending of 404 error, which usually appears when requested file doesn't exist. Define sendPage() function, and it first writes the header and then sends the contents of the file. Next define how our server will handle responses. Create the HTTP server, and then CSS file. Check to see how server handles errors by starting your server locally run with node server.js, and then click the link, and then retuen to main page. Next deploy site using Heroku, and creating an Heroku application. Heroku will generate a random name for your application. Now we can deploy our project. Every Heroku app starts with no branches and no code. So, the first time we deploy our project, we need to specify a remote branch to push to. The application is now deployed. Choose a proper name for it. Now you can try it out by typing heroku open in terminal.
* DIRT (Data-Intensive Real-Time) - acronym created to describe such type of applications Node.js. Node allows a server to handle a lot of connections and work with a number of requests at the same time. And you don't need much memory for that. It's designed to be responsive and fast. Useful when you need to create an application that will be able to respond instantly to a large number of users.