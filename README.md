# 3a.CREATION FOR ECHO CLIENT AND ECHO SERVER USING TCP SOCKETS
# AIM
To write a python program for creating Echo Client and Echo Server using TCP
Sockets Links.
## ALGORITHM:
1. Import the necessary modules in python
2. Create a socket connection to using the socket module.
3. Send message to the client and receive the message from the client using the Socket module in
 server .
4. Send and receive the message using the send function in socket.
## PROGRAM
```
NAME : DHARSHINI S N 
REGISTER NUMBER : 212224230062
```

## CLIENT:
```
import socket
s=socket.socket()
s.bind(('localhost',8000))
s.listen(5)
c,addr=s.accept()
while True:
    clientMessage=c.recv(1024).decode()
    c.send((clientMessage.encode()))
```

## SERVER:
```
import socket
s=socket.socket()
s.connect(('localhost',8000))
while True:
    msg=input("client>")
    s.send(msg.encode())
    print("server>",s.recv(1024).decode())
```
## OUPUT
## CLIENT:
<img width="960" alt="echoc" src="https://github.com/user-attachments/assets/5511a0bf-d3e5-4a46-ab1a-9f6ad0c8f709">

## SERVER:
<img width="960" alt="echos" src="https://github.com/user-attachments/assets/6b0a8392-8896-4511-aeb0-3b2a2f0e9639">

## RESULT
Thus, the python program for creating Echo Client and Echo Server using TCP Sockets Links 
was successfully created and executed.
