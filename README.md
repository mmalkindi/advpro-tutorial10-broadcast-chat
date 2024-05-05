# Tutorial 10 - Part 2: Broadcast Chat

## 2.1 Original code of broadcast chat

![1 Server 3 Client test run](img/server_3client.png)

This setup involves 4 terminal tabs, 1 running the server using `cargo run --bin server` first and the other 3 running the client using `cargo run --bin client` afterwards.
When a client connects, the server prints their IP address and sends the message `From server: Welcome to chat! Type a message`.
Connected clients can type messages in the terminal tab and hit Enter to send it to the server. Everytime a client receives a message from a server, it will print it.
For every message the server receives from a client, it will print the IP address alongside the message and then resends the message to all connected clients.
