# Python Socket Chat Application

This is a simple Python-based chat application that uses sockets and threading to enable communication between a server and a client. Below are the instructions to set up and run the application.

---

## Prerequisites

Before running the application, ensure you have the following Python packages installed:

1. **socket** (built-in, no need to install)
2. **threading** (built-in, no need to install)

No additional installations are required as `socket` and `threading` are part of Python's standard library.

---

## Setup Instructions

1. **Clone the Repository**  
   Clone or download this repository to your local machine.

2. **Update the Client IP Address**  
   Open the `client.py` file and locate the following line:
   ```python
   SERVER = "" #<-------your IP here
   ```
   Replace `'SERVER_IP'` with the actual IP address of the machine running the server.

3. **Run the Server**  
   Open the `the_socket.py` file in Visual Studio Code (or your preferred IDE) and run it. This will start the server, which will listen for incoming client connections.

4. **Run the Client**  
   Open a terminal and navigate to the directory containing `client.py`. Run the client script using the following command:
   ```bash
   python client.py
   ```
---

## How It Works

- The server listens for incoming connections from clients.
- Each client connects to the server using the specified IP address.
- Once connected, clients can send messages to the server, which will broadcast the messages to all connected clients.
- The server and clients use threading to handle multiple connections simultaneously.

---

## Notes

- Ensure the server is running before launching any clients.
- If running the server and clients on the same machine, you can use `'127.0.0.1'` as the IP address in `client.py`.
- For testing across different machines, ensure the server's IP address is accessible over the network.

---
This was inspired by tech with tim on youtube.
Enjoy building and experimenting with this simple chat application! If you have any questions or run into issues, feel free to reach out. Happy coding!
