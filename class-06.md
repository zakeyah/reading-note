# What is Problem Domain?
Understanding the problem domain is both the hardest and most important aspect to developing any piece of software.

The problem domain is an engineering term referring to all information that defines the problem and constrains the solution (the constraints being part of the problem).

It includes the goals that the problem owner wishes to achieve, the context within which the problem exists, and all rules that define essential functions or other aspects of any solution product. It represents the environment in which a solution will have to operate, as well as the problem itself.

## Why Understanding the Problem is the Hardest Part of Any Software Project?
## So how do we dive deep into understanding the problem domain?

The short answer is to ask questions. But it’s not just asking questions, it’s asking the right questions.

The end-user is your greatest asset. The key to understanding the problem is to understand how the end-user works and how the product fits into how they work. Get the end user talking and keep them talking by asking “What else?” and “Tell me more about ___”.

Never assume that I know enough about the business domain to make assumptions about it. It’s always a better use of time to get the answers to questions as they come up than making assumptions and continuing down the wrong path.

# Object
### JavaScript Object Literal

A JavaScript object literal is a comma-separated list of name-value pairs wrapped in curly braces.

JavaScript objects are containers for named values called properties or methods.

Object literals encapsulate data, enclosing it in a tidy package. This minimizes the use of global variables which can cause problems when combining code.

1- syntax:

let objectName = {property1:value, property2:value};
2- Object Properties:

The name:values pairs in JavaScript objects are called properties.

You can access object properties in two ways:

objectName.propertyName;
or

objectName["propertyName"];  
3- Object Methods

Methods are actions that can be performed on objects.

Methods are stored in properties as function definitions.

## Document Object Model
## What is the DOM?

The DOM is a W3C (World Wide Web Consortium) standard.

The DOM defines a standard for accessing documents.

The Document Object Model (DOM) specifies how browsers should create a model of an HTML page and how JavaScript can access and update the contents of a web page while it is in the browser window.

What is the HTML DOM?

The HTML DOM is a standard object model and programming interface for HTML. It defines:

The HTML elements as objects

The properties, methods, events of all HTML elements
The browser represents the page using a DOM tree.
# The DOM tree

![](https://www.w3schools.com/js/pic_htmltree.gif)

OM trees have four types of nodes:

1- document nodes.

2- element nodes.

3- attribute nodes.

4- text nodes.

To add a new element to the HTML DOM, you must create the element (element node) first, and then append it to an existing element.

Finding a Node the command to find the HTML element we wanted:

document.getElementById(“”)

document.getElementsByClassName()

document.getElementsByTagName()

Adding and Removing HTML By Using Javascript
1- Creating New HTML Elements

The appendChild() method in the previous example, appended the new element as the last child of the parent.

This code creates a new element.

Create a text node first.

append the text node to the element

append the new element to an existing element.

2- Creating new HTML Elements - insertBefore()

3- Removing Existing HTML Elements

To remove an HTML element, use the remove() method

4- Replacing HTML Elements

To replace an element to the HTML DOM, use the replaceChild() method.