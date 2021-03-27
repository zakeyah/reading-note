# What Is Node.js?
###  This is what the project’s home page has to say:

**Node.js® is a JavaScript runtime built on Chrome’s V8 JavaScript engine.**

### And this is what Stack Overflow has to offer:

**Node.js is an event-based, non-blocking, asynchronous I/O runtime that uses Google’s V8 JavaScript engine and libuv library.**

# Node.js is a program we can use to execute JavaScript on our computers. In other words, it’s a JavaScript runtime.

How to check that Node is installed on my system by opening a terminal and typing node -v. If all has gone well, you should see something like v12.14.1 displayed. This is the current LTS version at the time of writing.

# What Is Node.js Used For?
### Node.js Lets Us Run JavaScript on the Server

# The Node.js Execution Model

Node.js is an event-driven example: when a new request comes in (one kind of event) the server will start processing it. If it then encounters a blocking I/O operation, instead of waiting for this to complete, it will register a callback before continuing to process the next event. When the I/O operation has finished (another kind of event), the server will execute the callback and continue working on the original request. Under the hood, Node uses the libuv library to implement this asynchronous (that is, non-blocking) behavior.
Node.js capable of handling a large number of simultaneous connections

### The traditional approach to scaling a Node app is to clone it and have the cloned instances share the workload.

### Node.js even has a built-in module to help you implement a cloning strategy on a single server. 

## Are There Any Downsides? 

The fact that Node runs in a single thread does impose some limitations: For example:

- blocking I/O calls should be avoided
- CPU-intensive operations should be handed off to a worker thread
- errors should always be handled correctly for fear of crashing the entire process.

# What Kind of Apps Is Node.js Suited To? 
Node is particularly suited to building applications that require some form of real-time interaction or collaboration

- chat sites 
- apps such as CodeShare, where you can watch a document being edited live by someone else. 💻
- building APIs where you’re handling lots of requests that are I/O driven (such as those needing to perform operations on a database).
- sites involving data streaming, as Node makes it possible to process files while they’re still being uploaded. 
# What Are the Advantages of Node.js? 
speed and scalability
it speaks JSON.
JSON is probably the most important data exchange format on the Web
the lingua franca for interacting with object databases (such as MongoDB).
JSON is ideally suited for consumption by a JavaScript program, meaning that when you’re working with Node, data can flow neatly between layers without the need for reformatting. You can have one syntax from browser to server to database. 
ubiquitous
##  Other Uses of Node  And it doesn’t stop at the server. There are many other exciting and varied uses of Node.js! For example:

it can be used as a scripting language to automate repetitive or error prone tasks on your PC.
It can also be used to write your own command line tool, such as this** Yeoman-Style generator** to scaffold out new projects.
Node.js can also can be used to build cross-platform desktop apps and even to create your own robots

# npm 
Introducing npm, the JavaScript Package Manager  check which version you have installed on your system, type npm -v.

- the package manager for JavaScript
- the world’s largest software registry
how we would use npm to install a package.

- Installing a Package Globally npm install -g jshint

This will install the jshint package globally on your system. We can use it to lint the index.js file
-Installing a Package Locally npm init -y

This will create and auto-populate a package.json file in the same folder.
install the lodash package and save it as a project dependency npm install lodash --save
- Working with the package.json File

node_modules folder => This is where npm has saved lodash and any libraries that lodash depends on.