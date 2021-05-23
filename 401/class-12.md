# Socket.io

#### What is the benefit of transforming data into packets?
to transfer the file fast and efficient manner over the network and minimize the transmission latency, the data is broken into small pieces of variable length

#### UDP is often refereed to as a connectionless protocol. Why is this?
No connection needs to be established between the source and destination before you transmit data. UDP does not have a mechanism to make sure that the payload is not corrupted.

#### Can a socket server application have multiple socket connections?
A server socket listens on a single port. ... Multiple connections on the same server can share the same server-side IP/Port pair as long as they are associated with different client-side IP/Port pairs, and the server would be able to handle as many clients as available system resources allow it to.

#### Can a socket connection application be connected to multiple socket servers?
it is possible to run out of available ports if you make a lot of connections in a short amount of time.
since clients are different, multiple clients can connect to the same server socket

#### Can an application be both a socket server and a socket connection?
yes


# Term

|    |  |
| ----------- | ----------- |
| Observer Pattern | is a software design pattern in which an object, named the subject, maintains a list of its dependents, called observers, and notifies them automatically of any state changes, usually by calling one of their methods.        |
| Listener      | a function that listens for an event to occur.        |
| Event Handler      | a function that runs when a specific event fires        |
 Event-Driven Programming      | is when a program is designed to respond to user engagement in various forms.        |
| Event Loop      | is a programming construct or design pattern that waits for and dispatches events or messages in a program. The event loop works by making a request to some internal or external "event provider", then calls the relevant event handler.        |
| Event Queue      | s a repository where events from an application are held prior to being processed by a receiving program or system.        |
| Call Stack      |  mechanism for an interpreter to keep track of its place in a script that calls multiple functions - what function is currently being run and what functions are called from within that function        |
| Emit/Raise/Trigger      | in event-driven programming, emit sends a message to trigger a response and raise an event        |
| Database      | an organized collection of data, generally stored and accessed electronically from a computer system        |

### What Socket.IO :
Socket.IO is a library that enables real-time, bidirectional and event-based communication between the browser and the server.

### Socket.io Tutorial
- Socket.IO enables real-time bidirectional event-based communication
- Works on every platform, browser, or device
- Built on top of the WebSockets API (Client-side) and Node.js