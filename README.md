# Social Network Application

The Social Network is a client-server-based system that enables users to communicate with each other in real-time. It provides a user-friendly interface where users can connect to a server, exchange messages, manage user relationships, and perform various chat-related actions.
Key Features of the Social Network Application:
* Client-Server Architecture: The application follows a client-server model, where the server acts as a centralized hub for message exchange and client management.
* User Authentication: Users are required to authenticate themselves with a username to access the chat system, ensuring secure and personalized communication.
* Real-time Messaging: Users can send and receive messages in real-time, allowing for instantaneous communication and conversation flow.
* User Relationship Management: The application allows users to manage their relationships by adding followers, viewing followers and followings, and blocking/unblocking other users.
* User Presence Tracking: Users can see the online status of other connected users, enabling them to know who is currently active.
* Message History: The application may store message history, providing users with the ability to view past conversations and recall important information.
* Error Handling and Notifications: The application handles errors gracefully, providing appropriate notifications to users in case of connection issues or other errors.
* Scalability and Extensibility: The application is designed to be scalable, allowing for the addition of more clients and features without compromising performance or stability.
* User-Friendly Interface: The application provides a user-friendly interface with intuitive controls, making it easy for users to navigate and interact with the chat system.
The Social Network Application enhances communication and collaboration, enabling users to connect with others and engage in meaningful conversations in a convenient and efficient manner.


## Server Side
This is a server-side application for a chat system. It provides the backend functionality to handle client connections, user authentication, message handling, and user management.

### Features

- User Authentication: Clients can connect to the server and authenticate using their username.
- Message Broadcasting: Authenticated users can send messages that are broadcasted to all connected clients.
- Active User List: The server keeps track of active users and updates the client UI accordingly.
- User Registration: New users can register and their information is stored in a user database file.
- Private Messaging: Users can send private messages to specific recipients.
- User Disconnection: The server handles client disconnections gracefully.

### Technologies Used

- Programming Language: C#
- Network Communication: TCP/IP sockets
- User Interface: Windows Forms

### Getting Started

To run the server-side application:

1. Clone the repository.
2. Open the solution in an IDE (e.g., Visual Studio).
3. Build the solution to ensure all dependencies are resolved.
4. Run the server-side application.

### Usage

1. Start the server-side application.
2. Clients can connect to the server using a chat client application.
3. Clients can register new accounts or authenticate with existing usernames.
4. Once authenticated, clients can send messages, view the active user list, send private messages, and perform other supported actions.

### Server-Side Code

The server-side code provides the main logic for handling client connections, user authentication, message broadcasting, and user management. It is written in C# and utilizes TCP/IP sockets for network communication. The code is organized into classes and methods to handle different aspects of the server functionality.

- Server Initialization: The server is initialized and starts listening for incoming client connections.
- Client Connections: Each client connection is accepted, and a new thread is spawned to handle communication with that client.
- User Authentication: The server validates client authentication requests by checking the provided username against the user database file.
- Message Broadcasting: Messages received from authenticated clients are broadcasted to all connected clients.
- User Management: The server keeps track of active users, handles user disconnections, and provides functionality for retrieving user lists, followers, and other user-related data.


## Social Network Application Client

This is the client-side application for the chat system. It provides a user interface for users to connect to the server, send and receive messages, manage user relationships (followers/following), and perform other supported actions.

### Features

- User Authentication: Users can enter their username and connect to the server.
- Sending Messages: Authenticated users can send messages to be broadcasted to all connected clients.
- Receiving Messages: Users can receive messages from other connected clients.
- User Management: Users can add and view followers, view users they are following, delete their own messages, and view their own messages.
- Blocking Users: Users can block other users to prevent receiving messages from them.
- Private Messaging: Users can send private messages to specific recipients.
- Disconnecting from the Server: Users can disconnect from the server gracefully.

### Technologies Used

- Programming Language: C#
- Network Communication: TCP/IP sockets
- User Interface: Windows Forms

### Getting Started

To run the client-side application:

1. Clone the repository.
2. Open the solution in an IDE (e.g., Visual Studio).
3. Build the solution to ensure all dependencies are resolved.
4. Run the client-side application.

### Usage

1. Enter the server IP address and port number in the corresponding text fields.
2. Enter your username in the "Username" field.
3. Click the "Connect" button to connect to the server.
4. Once connected, you can send messages by typing in the "Sweet" field and clicking the "Send" button.
5. You can view received messages in the log area.
6. Use the provided buttons to perform actions such as adding followers, viewing followers/following users, deleting messages, blocking users, and more.
7. To disconnect from the server, click the "Disconnect" button.

### Client-Side Code

The client-side code provides the user interface and handles user actions and interactions with the server. It is written in C# and utilizes TCP/IP sockets for network communication. The code is organized into classes and methods to handle different aspects of the client functionality.

- Connection: The client connects to the server using the provided IP address and port number.
- User Authentication: The client sends the entered username to the server for authentication.
- Message Sending: Authenticated clients can send messages to the server to be broadcasted.
- Message Receiving: Clients receive messages from the server and display them in the user interface.
- User Management: The client can perform various user management actions, such as adding followers, viewing followers/following users, deleting messages, blocking users, and more.
- User Interface: The Windows Forms UI allows users to interact with the Social Network Application easily.
