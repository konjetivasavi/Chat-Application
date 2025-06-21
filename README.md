Company : CODETECH IT SOLUTIONS

Name : Konjeti Vasavi

INTERN ID : CT04DF720

Duration : 4-WEEKS

Mentor : Neela Santhosh Kumar

Description :For DEVELOP A REAL-TIME CHAT APPLICATION USING SOCKET.IO
This code provides a simple yet complete real-time chat application using modern web technologies such as Node.js, Express, and Socket.IO. It is built with a minimal, user-friendly front end and a lightweight back end that collectively allow multiple clients to send and receive messages instantly in the browser. On the front end (index.html), the document is styled simply using CSS for a neat and responsive user interface. A message list (ul#messages) displays incoming messages and a small form at the bottom contains a text input (#input) and a send button for the user to enter messages. The design emphasizes straightforward usability, with scrollable chat content to accommodate any number of messages. The form is wired up with client-side JavaScript that listens for the submit event and prevents the default behavior, allowing JavaScript to handle message submission instead of a page reload. The user’s message is then emitted to the server via Socket.IO. The client also listens for incoming messages over a persistent socket connection and appends them as list items to the chat list.

On the server side (server.js), we leverage Express to serve the static front-end files and Socket.IO for the real-time, bidirectional communication between all connected clients. The app initializes an HTTP server and attaches the Socket.IO server to it so that the client and server can exchange events easily. When a client first connects, the connection event is triggered, allowing the server to register the user’s socket ID and log the connection. Whenever a user emits a chat message event with their message payload, the server listens for this event and broadcasts the message to all connected clients, including the sender. This is achieved by io.emit('chat message', msg), which simplifies creating a live, synchronized chat experience that updates instantly for everyone. Similarly, when a user disconnects—perhaps by closing the browser or navigating away—the disconnect event is handled so that the server can log that the client has left. Finally, the server is instructed to listen on port 3000, so visiting  in a browser loads the chat application interface. Once loaded, the browser automatically connects to the server through the Socket.IO client library included in the page.

Overall, this implementation is a classic real-time chat demo that illustrates the fundamentals of websockets using Socket.IO. It requires very little setup and is highly approachable even for beginners who want to understand the core concepts of persistent client–server communication, event-driven architecture, and handling dynamic user input. The front end and back end together highlight how small, modular pieces of code can quickly add up to a functioning app where all chat participants see each message as soon as it is sent. Being lightweight and dependency-friendly, this pattern can also scale into more sophisticated chat apps with features like user authentication, rooms, file sharing, or emojis. Because all messages flow through the central server, it’s also straightforward to add features such as moderation, logging, or message persistence. Thus, this simple yet full example lays the groundwork for a broad range of real-time collaborative and interactive web applications, demonstrating the flexibility of JavaScript on both the client and server sides.
 
Output:
![Image](https://github.com/user-attachments/assets/a8b415ad-f61e-4448-9c96-3457723d7efd)

![Image](https://github.com/user-attachments/assets/5b873644-7cf8-4854-954a-7500b672e8e6)
