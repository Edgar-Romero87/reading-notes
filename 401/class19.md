# Message Queues
1. **What does it mean that web sockets are bidirectional? Why is this useful?**

The server can push messages to clients. Whenever you write a chat message, the idea is that the server will get it and push it to all other connected clients.

2. **Does socket.io use HTTP? Why?**

A socket.io server will attach to an HTTP server so it can serve its own client code through /socket.io/socket.io.js.

3. **What happens when a client emits an event?**

- Creates and fires customs events.
- Transmits data to the server.

4. **What happens when a server emits an event?**
- Send a message over to the client.
- A message event is sent to the WebSocket object. To handle it, add an event listener for the message event, or use the on message event handler. To begin listening for incoming data.

5. **What happens if a client “misses” an event?**

Unhandled messages are just ignored. Nothing happens with it.

6. **How can we mitigate this?**
Unhandled messages are just ignored. Nothing happens with it.


## Vocabulary Terms

### Web Socket
The WebSocket object provides the API for creating and managing a WebSocket connection to a server, as well as for sending and receiving data on the connection.

### Socket.io
Socket.IO is a library that enables real-time, bidirectional and event-based communication between the browser and the server.

### Client
The client has to start the WebSocket handshake process by contacting the server and requesting a WebSocket connection.

### Server
The server must listen for incoming socket connections using a standard TCP socket.