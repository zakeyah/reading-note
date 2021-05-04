# Readings: Express REST API

## Name 3 real world use cases where you’d want to change the request with custom middleware

1. Error handling
2. Security
3. Data management

## True or false: The route handler is middleware?
False, a route handler is the piece of code that makes an HTTP request, such as GET, POST, PUT, and DELETE

## In what ways can a middleware function end the process and send data to the browser?
it must call next() to pass control to the next middleware function. Otherwise, the request will be left hanging.


## At what point in the request lifecycle can you “inject” middleware?

After the request is made and before the response is sent, or it could be listed after the route being requested, but before the callback. 

## What can cause express to error with “Request headers sent twice, cannot start a second response”
callbacks that are accidentally called twice


# Terms:
**Middleware=>functions that have access to the request object (req), the response object (res), and the next function in the application’s request-response cycle.**

**Request Object=> is the object that sent when the client is requesting.**

**Response Object=> is the object that response when the client is requesting.**

**Application Middleware=> it's an application that uses middleware.**

**Routing Middleware=> refers to how an application’s endpoints (URIs) respond to client requests. For an introduction to routing.**

**Test Driven Development=>refers to a style of programming in which three activities are tightly interwoven: coding, testing ( and design .**

**Behavioral Testing=>Testing of the external behavior of the program (also known as black box testing), usually a functional testing**
