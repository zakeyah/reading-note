# Message Queues

#### What does it mean that web sockets are bidirectional? Why is this useful?
Data flows both ways (full-duplex), a web socket can both send and receive which is useful because it allows data to be sent and received on the same channel.

#### Does socket.io use HTTP? Why?
a socket.io server will attach to an HTTP server so it can serve its own client code through /socket.io/socket.io.js

#### What happens when a client emits an event?
The event will be sent to the server, which will be listening for the event if already connected

#### What happens when a server emits an event?
all client already connected will be listening for the event

#### What happens if a client “misses” an event?
Unhandled messages are ignored .

#### How can we mitigate this?
Can avoid missing an event by always having handlers installed and then deciding in the handlers whether to do anything with the message or not


# Term

|    |  |
| ----------- | ----------- |
| Socket | one endpoint of a two-way communication link between two programs running on the network, a socket is bound to a port number so that the TCP layer can identify the application that data is destined to be sent to         |
| Web Socket      | is a computer communications protocol, providing full-duplex communication channels over a single TCP connection        |
| Socket.io      | library that enables real-time, bidirectional, and event-based communication between the browser and the server, consists of a Node.js server and a javascript client library for the browser        |
 Client      | program separate from the server that initiates requests for services or info from the server        |
| Server      | provides function, info, or service back to the client, acts as the main hub for communication        |
| OSI Mode      |  open systems interconnection model is a model that characterizes and standardizes the communication functions of a telecommunication or computing system without regard to its underlying internal structure and technology
7 layers: physical layer, data link layer, network layer, transport layer, session layer, presentation layer, application layer      |
| TCP Model      |  is the conceptual model and set of communications protocols used in the Internet and similar computer networks.       |
| TCP      | is a standard that defines how to establish and maintain a network conversation through which application programs can exchange data       |
| UDP      | user datagram protocol, connectionless protocol so there is no need to establish a connection prior to data transfer        |



### socket.io Cheat Sheet
- sending to sender-client only
- socket.emit('message', "this is a test");

- sending to all clients, include sender
- io.emit('message', "this is a test");

- sending to all clients except sender
- socket.broadcast.emit('message', "this is a test");

- sending to all clients in 'game' room(channel) except sender
- socket.broadcast.to('game').emit('message', 'nice game');

- sending to all clients in 'game' room(channel), include sender
- io.in('game').emit('message', 'cool game');

- sending to sender client, only if they are in 'game' room(channel)
- socket.to('game').emit('message', 'enjoy the game');

- sending to all clients in namespace 'myNamespace', include sender
- io.of('myNamespace').emit('message', 'gg');

- sending to individual socketid (server-side)
- socket.broadcast.to(socketid).emit('message', 'for your eyes only');

- join to subscribe the socket to a given channel (server-side):
- socket.join('some room');

- then simply use to or in (they are the same) when broadcasting or emitting (server-side)
- io.to('some room').emit('some event'):

- leave to unsubscribe the socket to a given channel (server-side)
- socket.leave('some room');


### Rooms and Namespaces

- Room is an arbitrary channel that sockets can join and leave, it can be used to broadcast events to a subset of clients
- Rooms are a server-only concept (client does not have access to the list of rooms it has joined)
- Can join to subscribe the socket to a given channel ```socket.join()```
- Each socket in Socket.io is identified by a random unique identifier (Socket#id), each socket automatically joins a room identified by its own id
- Upon disconnection, sockets leave all the channels they were part of automatically