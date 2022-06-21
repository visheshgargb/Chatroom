# Chatroom
Description - Chatroom is a mutlithread based chatting tool where different clients can join a single server to chat with each other .
code is in c++ and is based on Linux based OS . It uses socket programming , multithreading and mutex .

To Run the application -

After installing g++, Type the following commands in the terminal.
 1. g++ server.cpp -lpthread -o server
 2. g++ client.cpp -lpthread -o client To run the server
 3. type ./server To run the client
 4. type ./client

To operate for multiple clients –

Open new terminal and type ./client command.

Internal Working -

The application consists of server and clients which are connected to each other by sockets.

Server – The server  shows the activity of various clients in the chat room. On executing the server code, the socket is created. Then the bind socket and listen socket functions are executed. After this the server is open for various clients to join. After receiving the request to join from the client, a new thread is created. And the msg_broadcast function is used to send the messages of one client to all other clients.

Client - The client side first request to join the server by entering a unique username. After this, a socket is created, and the client is ready to interact with all the other clients. The client can exit the chat room by typing “#exit”.

Learnings-

During the course of this project, I became familiar with the concepts of socket programming and multi-threading and their use in the implementation of chat server. I also learnt about the concept and implementation of mutex in this project.

Additional Tasks-

1. Chat room server is implemented from the concepts of socket programming and multi-threading.
2. The concept of mutex has been used while adding and removing clients from the chat room for proper synchronization.
3. The client can exit the chat room by typing “#exit”. References-
4. https://www.geeksforgeeks.org/socket-programming-cc/ • https://www.geeksforgeeks.org/multithreading-c-2/
5. https://beej.us/guide/bgnet/pdf/bgnet_a4_c_1.pdf

Video Illustration of project- 

https://www.youtube.com/watch?v=-QVt5NJtSxI&ab_channel=VISHESHGARG
