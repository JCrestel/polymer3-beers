# A Polymer 3.x. tutorial. With beers.

*A work-in-progress tutorial for creating a Progressive Web App (PWA) with Polymer 3.x*

I have built this [Polymer 3 tutorial](https://github.com/LostInBrittany/polymer3-beers) as a quick entry point to [Polymer](https://www.polymer-project.org/). 

For the last several years, I've taught a web-development module in an Engineering School with a rather restrictive network. As I plan to use this tutorial in next year module, in order to explain PWA and Polymer to our students, I needed a tutorial that could be played without network acces, i.e. without Bower or Gulp or even without [Polymer CLI](https://github.com/Polymer/polymer-cli). So *Progreessive Web Apps with Polymer* needed to be able to be done even behind a very restrictive proxy, and all the dependencies are included inside the git project.

![Logo](./img/logo-500px.png)


## What are the objectives of this tutorial ##


Follow the tutorial to see how Polymer makes browsers smarter — without the use of native extensions or plug-ins:

+ See examples of how to use client-side data binding to build dynamic views of data that change immediately in response to user actions.
+ See how Polymer keeps your views in sync with your data without the need for DOM manipulation.
+ Learn how to build technical elements to make common web tasks, such as getting data into your app, easier.

When you finish the tutorial you will be able to:

+ Create a dynamic application that works in all modern browsers.
+ Create custom elements, with its looks and its behaviour encapsulated inside, setting the bases of a true component architecture client-side
+ Use data binding to wire up your data model to your views.
+ Get data from a server using Polymer iron elements.
+ Use App Router to add multipage capabilities to your application

The tutorial guides you through the entire process of building a simple application. Experiments at the end of each step provide suggestions for you to learn more about Polymer and the application you are building.

You can go through the whole tutorial in a couple of hours or you may want to spend a pleasant day really digging into it. If you're looking for a shorter introduction to Polymer, check out the official website.

![Screenshot](./img/polymer3-beers-final.jpg)  

![Screenshot](./img/polymer3-beers-final-details.jpg)

## What do I need to use this tutorial?

The tools strictly needed for this tutorial are a modern web browser (ideally [Chrome](https://www.google.com/chrome/) or [Chromium](https://www.chromium.org/)), a text editor (we suggest the excellent [Visual Studio Code](https://code.visualstudio.com/) or [Atom](https://atom.io))), a web server, [Node JS](https://nodejs.org) and the [Polymer CLI](https://github.com/Polymer/polymer-cli). If you're unable to install the Polymer CLI (for example your're in  workshop with slow network connection), you will be able to do the tutorial, even if in a slightly degraded mode, as we have committed all the needed resources to this repository.


### Web server

Security policies in the browser make impossible to fully test your JavaScript applications when they have been loaded by opening a local file, they need to be served from a web server.

If you already have a web server (Apache, Nginx, ...) in your computer, you can use it. If not, there are several quick options available:

- Web Server for Chrome: a Chrome/Chromium application that gives you a web server embedded in your browser. You can install it [from the Chrome Web Store](https://chrome.google.com/webstore/detail/web-server-for-chrome/ofhbbkphhbklhfoeikjpcbhemlocgigb?hl=en) .

  After installing the Web Server for Chrome app, click on the Apps shortcut on the bookmarks bar:


  [![Web Server for Chrome](img/chromewebserver-00.t.png)](img/chromewebserver-00.png)


  And then on the *Web Server for Chrome* logo to configure the server:


  [![Web Server for Chrome](img/chromewebserver-01.t.png)](img/chromewebserver-01.png)


  Now you choose as folder to serve the root of this repository. We also suggest to run it on port 8080. You launch the server and open a browser window navigate to http://localhost:8080/test.html to verify that everything is good

- Using Python: if you have Python in your system, the easiest way would be to run the embedded SimpleHTTPServer. Go to the project directory and run

  ```
  # Python 2.x
  python -m SimpleHTTPServer 8080
  ```

  or

  ```
  # Python 3.x
  python -m http.server 8080
  ```

  to start the web server. Now, open a browser window for the app and navigate to http://localhost:8080/test.html to verify that everything is good.

- If you have [NodeJS](http://nodejs.org) in your system, we have put a minimalist JavaScript web-server on `./scripts/web-server.js`. To see the app running in a browser, open a separate terminal/command line tab or window, go to the project directory and then run `node ./scripts/web-server.js` to start the web server. Now, open a browser window navigate to http://localhost:8080/test.html to verify that everything is good.



### Polymer CLI

Ideally you should install Polymer CLI. Polymer CLI is a *NodeJS* based tool, so you need it too:

- To get NodeJS for your platform, go to [the NodeJS site](https://nodejs.org).

  If you haven't administrator rights in your workstation, please download the binary package for your platform, 
  uncompress it in a folder inside your home folder and add to the PATH the `bin` folder inside it. 

- To install the Polymer CLI:

  ```bash
  npm install -g polymer-cli
  ```

Then you'll be able to use `polymer` command to create, build and serve your application.

> Note: in order to use Polymer CLI with Polymer 3.x, you need a recent version of Polymer CLI. Please be sure your insatlled version is at least 1.8. If you have an older version, please install a more recent one.


## How is the tutorial organized ##

As the computer used for the course haven't Git, we have structured the project to allow a Git-less use. The `app` directory is the main directory of the project, the working version of the code. The tutorial is divided in steps, each one in its own directory:

1. [Static HTML](./step-01/)
1. [Using Polymer elements](./step-02/)
1. [Creating a new element](./step-03/)
1. [Filtering](./step-04/)
1. [Sorting](./step-05/)
1. [Calling the server](./step-06/)
1. [Routing URLs using App Router](./step-07/)

In each step directory you have a README file that explain the objective of the step, that you will do in the working directory `app`. If you have problems or if you get lost, you also have the solution of each step in the step directories. So if you want to see the intended result of  the 6th step, you can point your browser to http://localhost:8080/step-06/index.html


## What should I do now?  ##

OK, now you're ready to follow this tutorial. If you're familiar with git, begin by cloning this repository (`git clone https://github.com/LostInBrittany/polymer3-beers`), else you can simply download the zipped file from [GitHub](https://github.com/LostInBrittany/polymer-beers/archive/master.zip).

Now can go to [step-01](./step-01) and begin to follow the README of that step. Let's begin!
