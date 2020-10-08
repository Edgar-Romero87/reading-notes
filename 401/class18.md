# Socket.io

1. **What is the benefit of transforming data into packets?**
- Optimize the use of the channel capacity available.
- Minimize the transmission latency.
- Increase the robustness of communication.

2. **UDP is often referred to as a connectionless protocol. Why is this?**

DNS, TFTP, and many other protocols rely on UDP for their data transmission. UDP is a connectionless protocol. No connection needs to be established between the source and destination before you transmit data. UDP does not have a mechanism to make sure that the payload is not corrupted.

3. **Can a socket server application have multiple socket connections?**

Yes. A port of a server can be used by many clients (connections)

4. **Can a socket connection application be connected to multiple socket servers?**

A port of a client can be used by a single connection. The reason is a port can be used by a single process, which allocates the port (doing "bind" as a server that will listen to that port for incoming connections, or doing a sort of "open" as a client wanting to do outbound connections from that port out).

5. **Can an application be both a socket server and a socket connection?**

Yes, if you use two different ports or if the sockets won't be using the same port at the same time.

## Vocabulary Terms
### OSI Model
The OSI Model (Open Systems Interconnection Model) is a conceptual framework used to describe the functions of a networking system. The OSI model characterizes computing functions into a universal set of rules and requirements in order to support interoperability between different products and software.
### TCP Model
TCP allows for the transmission of information in both directions. This means that computer systems that communicate over TCP can send and receive data at the same time, similar to a telephone conversation. The protocol uses segments (packets) as the basic units of data transmission. The TCP/IP reference model has four layers: Network interface, Internet, Transport, and Application.
### TCP
TCP (Transmission Control Protocol) is a standard that defines how to establish and maintain a network conversation through which application programs can exchange data. TCP works with the Internet Protocol (IP), which defines how computers send packets of data to each other.
### UDP
UDP (User Datagram Protocol) is a communications protocol that is primarily used for establishing low-latency and loss-tolerating connections between applications on the internet. It speeds up transmissions by enabling the transfer of data before an agreement is provided by the receiving party.
### Packets
A packet is a small amount of data sent over a network, such as a LAN or the Internet. Similar to a real-life package, each packet includes a source and destination as well as the content (or data) being transferred.
### Socket
A socket is one endpoint of a two-way communication link between two programs running on the network. A socket is bound to a port number so that the TCP layer can identify the application that data is destined to be sent to. 