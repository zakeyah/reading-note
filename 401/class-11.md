# Event Driven Applications

## 1- Why is access control important?

#### it's important because it is a valuable security technique that can be used to regulate who or what can view or use any given resource. Without proper access control, you could leave your staff and your company-wide open to problems such as data loss, theft, or breach of privacy and data protection laws

## 2- Describe an application that would need access control.

#### Almost any type of application, like university app and companies.

## 3- What is a role used for?

#### A role is used to determine what type of capabilities a user has. Admin for example have all capabilities (read, write, update, delete), while a regular user may only have read capabilities.

## 4- Why is role based access control more scalable than discretionary or mandatory access control?
#### it is  less secure, because associated programs inherit security settings and allow malware to exploit them without the knowledge of the end-user. 

# Term

|    |  |
| ----------- | ----------- |
| Authorization | Authorization is a security mechanism to determine access levels or user/client privileges related to system resources including files, services, computer programs, data and application features. This is the process of granting or denying access to a network resource which allows the user access to various resources based on the user's identity.        |
| Role Based Access Control      | restricts network access based on a person's role within an organization and has become one of the main methods for advanced access control. The roles in RBAC refer to the levels of access that employees have to the network.        |
| Capabilities      | the functions that a user has access to (read, create, update, or delete for example)        |


### Event-Driven Programming in Node.js 

##### Event driven programming is a logical pattern that we can choose to confine our programming within to avoid issues of complexity and collision


### EventEmitter
##### Node.js natively provides us with a useful module called EventEmitter that allows us to get started incorporating Event-Driven Programming 

#####  Access the EventEmitter class through the `events` module, one imported you need to create a new object from the class to start using it

```js
const EventEmitter = require('events').EventEmitter;
const myEventEmitter = new EventEmitter();
```
- Use EventEmitters on method to set the listener
- Use the emit method to trigger the event
- Removing listeners with removeListener or removeAllListeners