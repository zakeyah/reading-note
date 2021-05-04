# Data Modeling

## Name 3 advantages to Test Driven Development
- ensures that the code meets the desired requirements.
- spend less time in the debugger.
- improved design qualities in code


## In what case would you need to use beforeEach() or afterEach() in a test suite?
- Use beforeEach() if a method needs to be called before a test is run
- Use afterEach() if you need to reset the environment after a test has run

## What is one downside of Test Driven Development
- Slow process.
- Running tests only some parts of the code might give an output different than what will the actual output going to be.

## What’s the primary difference between ES6 Classes and Constructor/Prototype Classes?
- ES6 Classes are syntactical sugar so it is easier to read and write.

## Why REST?
- Much easier to code/implement for web services than SOAP
- Don't need to maintain a state of information from one request to another

# Term

|    |  |
| ----------- | ----------- |
| functional programming | Software is composed using pure functions (avoid shared state, mutable data, side-effects) If functions are interrelated, changing one function could break everything else        |
| object-oriented programming (OOP)      | computer programming model that organizes software design around data, or objects, rather than functions and logic. An object can be defined as a data field that has unique attributes and behavior.        |
| class      | templates for creating objects. The constructor() method is used for creating and initializing an object created with a class.        |
| super      |  keyword is used to access and call functions on an object's parent.        |
| this      | refers to the current object being instantiated        |
| Test Driven Development (TDD)      | refers to a style of programming in which three activities are tightly interwoven: coding, testing ( and design .        |
| Jest      | is a JavaScript testing framework designed to ensure correctness of any JavaScript codebase.        |
| Continuous Integration (CI)      | Consistent merging from multiple places into one multiple time a day       |
| REST      | Representational State Transfer. Uses HTTP requests to retrieve/use data|
| Data Model     | Data model is a diagram that illustrates relationships and behaviors of different pieces of an application and how those pieces depend on one another        |



# NoSQL vs SQL
## NoSQL 
- primarily called non-relational database
- document based, key-value pairs, graph databases, or wide-column stores
- dynamic schema for unstructured data
- horizonally scalable
- queries are focused on collection of documents, sometimes called unstructured query language (UnQL)


## SQL
- primarly called relational databases
- table databases
- predefined schema
- vertically scalable
- use structured query language

## NoSQL Modeling Techniques
- Often compared by various non-functional criteria, such as scalability, performance, and consistency
- Often starts from the application-specific queries as opposed to relational modeling
- Often requires a deeper understanding of data structures and algorithms than relational database modeling does
- Data duplication and denormalization are first class citizens