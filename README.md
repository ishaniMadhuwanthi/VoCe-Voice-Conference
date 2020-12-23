# VoCe-Voice-Conference

- - - - - 

## Overview

Peer to peer communication is a strategy used in applications such as Bit-Torrent, and Skype. In this Voce assignment, we have to design and code a basic peer to peer voice conferencing application which is similar to Skype. It has two types, 

	1. Implement voice communication between two parties
	2. Extend the application to support multi-party call conferencing

This is a real time application that, when the sender is speaking, sound is captured and the message  will be broadcast to the connected wifi clients who are connected to the same wifi network.

## Instructions

1. Clone the repository
2. **Task1** -  Implement voice communication between two parties
3. **Task2** -  Extend the application to support multi-party call conferencing

------------------------------
### **To voice communication between two parties**

Use Task1 folder to get communication between two parties. Program can be run as following.

```Java
**javac CaptureSound.java**
java CaptureSound <receiver IP>
```
Eg:- If client1 : 192.168.1.101
        client2 : 192.168.1.102 
        
client1 should run 
     ```Java
     java CaptureSound 192.168.1.102
     ```

#### Procedure

1.When the program is started, sender sends message. It stores in data packets.
2.Then the packets are send to a specified receiver through wifi, who is connected to the same wifi network with sender.
3.The sender should press “ENTER” to send the audio message to the receiver client for capturing. At  the same time, receiver also should press “ENTER” for playing the received audio message.Then they can hear what sender is saying.


---------------------

### **Implement multicast communication**

To start the program, when running the program the command line argument should differ from peer-to-peer communication between two parties.

```Java
javac Capture 224.0.0.0        <224.0.0.0 is the multicast IP address for every device connected>
```

#### Procedure

1.When the program is started, sender sends message. It stores in data packets.
2.Then the packets are send to a specified receivers through wifi, who are connected to the same wifi network with sender.(There are multiple receivers )
3.The sender should press “ENTER” to send the audio message to the receiver client for capturing. At  the same time, receivers also should press “ENTER” for playing the received audio message.Then they can hear what sender is saying.










