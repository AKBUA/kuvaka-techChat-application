https://github.com/AKBUA/kuvaka-techChat-application.git
# clone repository
git clone  https://github.com/AKBUA/kuvaka-techChat-application.git


# Server

# navigate to server directory
cd server
# Install dependencies
npm install
# run server 
npm start



# Client

# navigate to client directory
cd client
# Install dependencies
npm install
# run client 
npm start


# Architecture
The chat application consists of a server and a client. The server is built using Node.js and Express, providing a WebSocket connection with Socket.IO. The client is a React application that communicates with the server via WebSocket to enable real-time chat functionality.

# Concurrency Handling

The server handles concurrency through the use of the Socket.IO library. Each client connection is treated as a separate socket, allowing for bidirectional communication between the server and multiple clients simultaneously. Socket.IO manages the events and communication channels efficiently, ensuring that messages are broadcasted to all connected clients in real-time.

# Assumptions and Design Choices

#   Random Username Generation:

Assumption: Usernames are randomly generated on the server for simplicity.
Design Choice: To provide a quick and easy way to identify users without requiring manual input.

# Real-Time Communication:

Assumption: The application prioritizes real-time communication over message persistence.
Design Choice: WebSocket and Socket.IO are chosen for their real-time capabilities, making the application suitable for chat scenarios where instant communication is essential.

# Styling:

Assumption: The focus is on functionality rather than extensive styling.
Design Choice: Minimal styling is applied for a clean and straightforward user interface. This allows for easy extension and customization by developers.


# Separate Server and Client:

Assumption: The server and client are kept separate for modularity and scalability.
Design Choice: This separation allows for independent deployment and scaling of the server and client, facilitating future updates and improvements to each component individually.
