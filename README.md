# Simple Chat Application

This repository contains a basic chat application implemented in Python using sockets. It includes two scripts:
- **server.py**: Represents the server-side of the chat.
- **client.py**: Represents the client-side of the chat.

## Features
- Peer-to-peer communication between a client and a server.
- Exchange of messages in real-time.
- Support for terminating the chat session by typing `quit`.

## How It Works
### Server
1. The server listens for incoming client connections on localhost and port 9999.
2. Once a connection is established, the server continuously receives messages from the client.
3. The server displays received messages and responds with messages entered by the server user.
4. If the server or client sends the message `quit`, the connection is closed.

### Client
1. The client connects to the server on localhost and port 9999.
2. The client sends messages entered by the user to the server.
3. The client displays the server's responses.
4. If the client or server sends the message `quit`, the connection is terminated.

## Requirements
- Python 3.x

## How to Run
### Step 1: Start the Server
Run the `server.py` script:
```bash
python server.py
```

### Step 2: Start the Client
In a separate terminal, run the `client.py` script:
```bash
python client.py
```

### Step 3: Chat
- The client and server can now exchange messages.
- To end the chat, type `quit` from either the client or server.

## Example Interaction
**Server Terminal:**
```
Message: Hello Client
Client: Hello Server
Message: How are you?
Client: I am fine, thank you!
Message: quit
```

**Client Terminal:**
```
Message: Hello Server
Server: Hello Client
Message: I am fine, thank you!
Server: How are you?
Message: quit
```

## Notes
- This is a simple implementation for educational purposes and does not include advanced error handling or security mechanisms.
- Ensure that the server script is running before starting the client script.
