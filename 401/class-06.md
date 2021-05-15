# Authentication

## Explain what a “Singleton” is (in Computer Science terms)

#### A singleton is a class that allows only a single instance of itself to be created and gives access to that created instance. It contains static variables that can accommodate unique and private instances of itself. It is used in scenarios when a user wants to restrict instantiation of a class to only one object. This is helpful usually when a single object is required to coordinate actions across a system.


## Explain how the Singleton pattern can be used with Node modules, specifically with classes

##### Sometimes you need to make sure that you have one and only one instance of an object. This is where the singleton pattern can be useful. A singleton represents a single instance of an object. Only one can be created, no matter how many times the object is instantiated. If there’s already an instance, the singleton will create a new one. Let’s take a look at where creating multiple instances of one object might create problems within our application.


## If you were tasked with building a middleware system like Express uses, what approach might you take to construct/operate it?

- create function in middleware ( request , response and next )

- Allow the middleware to have access globally .

- Allow the middleware to end the process or move to the next middleware .


# Term


|    |  |
| ----------- | ----------- |
| Router Middleware | Router-level middleware works in the same way as application-level middleware, except it is bound to an instance of express.Router(). Load router-level middleware by using the router.use() and router.METHOD() functions.        |
| Dynamic Module Loading      | This allows you to dynamically load modules only when they are needed, rather than having to load everything up front.        |
| Singleton Pattern      | is a software design pattern that restricts the instantiation of a class to one "single" instance. This is useful when exactly one object is needed to coordinate actions across the system.        |
| CRUD -> REST Method Matches      |  is an acronym for C - create, R - read , U -update, D - delete- the four basic functions that are implemented in any relational DB applications.        |
| Mock Testing     | is an approach to unit testing that lets you make assertions about how the code under test is interacting with other system modules       |

## Securing Passwords

Passwords are the first line of defense against cyber criminals. It is the most vital secret of every activity we do over the internet(bank account, email account, shopping cart account).
The benefit of hashing is that if someone steals the database with hashed passwords, they only make off with the hashes and not the actual plaintext passwords.

## Basic Auth
Basic access authentication is a method for an HTTp user agent (web browser) to provide a user name and password when making a request

## OWASP auth cheatsheet
Authentication: process of verifying than an individual, entity or website is whom it claims to be.Authentication in the context of web applications is commonly performed by submitting a username or ID and one or more items of private information that only a given user should know.

## bcrypt.js

A library to help you hash passwords.
