

# What’s the difference between PUT and PATCH?

### The main difference between the PUT and PATCH method is that the PUT method uses the request URI to supply a modified version of the requested resource which replaces the original version of the resource, whereas the PATCH method supplies a set of instructions to modify the resource. 



# Provide links to 3 services or tools that allow you to “mock” an API for development like json-server

[postman](https://www.postman.com/features/mock-api/)

[mockoon](https://mockoon.com/)

[nock](https://github.com/nock/nock)

# Compare and contrast Swagger and APIDoc.js 1 Which HTTP status codes should be sent with each type of (un)successful API call?

SWAGGER :


- '200': description: OK
- '400': description: Bad request. User ID must be an integer and larger than 0.
- '401': description: Authorization information is missing or invalid.
- '404': description: A user with the specified ID was not found.
- '5XX':description: Unexpected error.

APIDoc
- 200(ok)
- 400(Bad Request)
- 401(4Not Authenticated)
- 404(Not found)
- 4xx (errors)

# Compare and contrast SOAP and ReST

**Main differences between SOAP and REST**
![](https://i.stack.imgur.com/DFII3.png)



# Terms
- Web Server => The term web server can refer to hardware or software, or both of them working together
- Express => Express is a back end web application framework for Node.js It is designed for building web applications and APIs
- Routing => refers to determining how an application responds to a client request to a particular endpoint, which is a URI (or path) and a specific HTTP request method.
- WRRC => a cycle of requests and responses that flow between clients and servers.