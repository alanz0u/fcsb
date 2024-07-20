# spchatoverlay
Secure Programming Project 2024

passwords for c1 - c5:
1. potato
2. watermelon
3. banana
4. coconut
5. apple



A good templete to write README

# Project Title

## Description
<!-- A brief description of what the project is, what it does, and why it is useful. -->
A light weight Command Line Interface chat system based on Python and websocket.
Features include:
1. Private text messaging
2. Group messaging
3. File transfer
4. End-to-end encryption

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)
- [Features](#features)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)
- [Acknowledgments](#acknowledgments)

## Installation
Step-by-step instructions on how to install and set up the project.

### Prerequisites
List any software or tools needed before installing.

### Installing
1. Step 1
2. Step 2
3. Step 3

## Usage
Enter the following command at command line terminal to (You might need to go first to the base directory that contains the Python scripts):
1. Set server and client configuration  
Edit the following options in server_config.yaml:
```
server_name: s1
chat_server:
  host: localhost
  port: 12345
exchange_server:
  host: localhost
  port: 5555
remote_servers:
  - name: s4
    host: 127.0.0.1
    port: 5556
```
Edit the following options in client_config.yaml:
```
chat_server
host: localhost
port: 12345
```
2. Start the server
Command to start the chat server:
```
python secure_chatapp.py
```
![Alt Text](snapshot/server_start.png)

Command to start the client:
```
python chat_client.py
```
![Alt Text](snapshot/client_start.png)

3. At the client-side terminal, follow the instructions and log in:
```
Enter your username:
(Example) c1
Enter your password:
(Example) potato
```
If login successfully, the following message will display:
```
Authentication successful!
active users: ['c1(c1@s2)]
```
![Alt Text](snapshot/client_auth.png)

4. Private Message
- Private text message to individual participant C2 on Server S2
```
@C2@S2 hello
```
![Alt Text](snapshot/client_msg_rcv.png)

- Group message to everyone in the chatroom
```
Hi everyone
```
![Alt Text](snapshot/client_msg_broadcast.png)

5. File transfer
```
FILE @C2@S2 readme.md
```


6. Exit the chatroom
EXIT

```python
# Example code snippet
print("Hello, World!")
