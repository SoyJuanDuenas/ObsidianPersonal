#ComputerScience 

HTTP (Hypertext Transfer Protocol) is the foundation of data communication on the World Wide Web. It defines how messages are formatted and transmitted and how web servers and browsers should respond to various commands.

HTTP stands for Hypertext Transfer Protocol, is a set of rules between a user and a server to make a properly comunication, HTTP Protocol is especifically to transfer data from one point to another. And how the name stand, the data are hypertext which is text with links.

HTTP Protocol has 3 important properties:

- **Request - Response based:** The client send a request and the server return a response. HTTP treats each request as an independent transaction, wich does not retain user [[state]] beyond the request.
 ![[Pasted image 20241228160006.png]]
 - **Human readable:** HTTP is text-based then is easy to troubleshoot.
 - **Naturally extensible:** along there is a agreement between the client and the server, new definitions are avaliable.

In the context of a client - server comunication, the [[state]] is not necesarly in the HTTP protocol, can be also the information saved in the server about specific client, this are called [[browser cookies]]. 

The user-agent are from the request are made, when we make a request we should use one of the [[HTTP methods]] in order to request the server a specific type of intruction.
