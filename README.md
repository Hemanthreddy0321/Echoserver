# Echoserver
Echo server and client using python socket

# AIM:

To develop a simple webserver to serve html programming pages.

## DESIGN STEPS:

### Step 1:

Design of echo server and client using python socket

### Step 2:

Implementation using Python code

### Step 3:

Testing the server and client 

## PROGRAM:
""
SERVER:

import socket
HOST,PORT = '127.0.0.1',65432
with socket.create_server((HOST,PORT)) as s:
    conn ,addr =s.accept()
    with conn:
        print(f'connected by{addr}')
        while data :=conn.recv(1024):
            conn.sendall(data)

 CLIENT :  
 import socket
HOST ,PORT ='127.0.0.1',65432
with socket.create_connection((HOST, PORT)) as s:
    s.sendall(b'Hemanth A, 212223220035')
    print(f'Received:{s.recv(1024)!r}')
    
""
## OUTPUT:
SERVER:
![image](https://github.com/user-attachments/assets/4a85a26a-b3c0-48e6-b69a-a922440865ef)
CLIENT:
![image](https://github.com/user-attachments/assets/82d133db-7ec0-40aa-aec8-72d7be562b6e)


## RESULT:
The program is executed successfully
