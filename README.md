# Peer to Peer File Sharing Application using Chord-DHT Algorithm

## Peer to Peer Model:

Peer-to-peer messaging is a form of communication where two or more users communicate directly with each other over a network, without the need for a centralized server or intermediary. In P2P messaging, each user can both send and receive messages, and the messages are transmitted directly between the users' devices. It’s a very simple and secure way to send messages, files, andany other private information. P2P messaging can be used for various purposes, such as instant messaging, file sharing, and video conferencing. P2P messaging is often used in decentralized communication systems, where the goal is to avoid relying on a centralized server or authority  for communication.

P2P networks are the foundation of the internet architecture and do not distinguish between client and server devices. Retrieval and routing algorithms based on DHT are popular in structured P2P networks because they offer determinability, simplicity, and distribution in searching. DHTs are robust against node failure, attacks, and sudden high loads, and are scalable, self-configuring, and provide simple interfaces for multiple P2P applications.

## Chord-DHT(Distributed Hash Table ALgorithm):

Chord Protocol is a type of P2P computing protocol that offers a new approach to effectively locate resources. The protocol uses a hash function to map a given keyword (such as a file name) to a specific node in the system, allowing data to be associated with keys. The IP address of a node is also hashed to obtain its identifier. By assigning a key to each data item in a peer-to-peer network application, the Chord protocol can easily solve data lookup problems. Unlike other protocols, Chord does not require every node to know all the other nodes, which allows for greater scalability. Each node only needs to store limited routing information about other nodes, and when nodes join or leave the system, Chord updates the routing information accordingly.
The Chord DHT algorithm provides a scalable and fault-tolerant way of storing and retrieving data in a P2P network, with low overhead and high availability. It has been used in a variety of P2P applications, including file-sharing, content delivery networks, and distributed databases.

## Objective of this project:

The scope of this study is to design and implement a decentralized peer-to-peer system using CHORD-DHT algorithm over TCP/IP protocol that defínes a file sharing mechanism which serves as a communication model for interconnected nodes.

## Significance:

P2P networks are a vital component in the design of file systems because they enable files to be shared across multiple nodes in a network. The Chord DHT model, a distributed system, is an essential aspect of modern operating systems as it relies heavily on concepts such as concurrency, synchronization, communication, and resource management. Chord DHT's decentralized peer-to-peer architecture resembles the distributed file systems . This decentralized approach provides several advantages over traditional centralized file systems, including increased scalability, fault tolerance, and improved performance.

## Why this algorithm is chosen?

In a peer-to-peer system, devices communicate with each other directly, without relying on a central server. This approach offers several advantages over traditional client-server models, including greater scalability, reduced latency, and increased fault tolerance. By utilizing the TCP/IP protocol, this peer-to-peer system can leverage the existing infrastructure of the internet to establish connections and transmit data between devices. One challenge that a peer to peer application usually faces is efficiently locating the node that stores a desired data item. The solution is a distributed lookup protocol called Chord, which maps a given key onto a node. By associating a key with each data item, data location can be easily implemented on top of Chord, with the key/data pair stored at the node to which the key maps. Chord is designed to adapt efficiently as nodes join and leave the system, and can still provide query responses even if the system is undergoing continuous changes. Theoretical analysis and simulations show that Chord is scalable, with communication cost and state maintained by each node scaling logarithmically with the number of Chord nodes.

### Steps to execute the project:

To execute you need multiple copies of the same script running simultaneously
During execution each script executed on cmd or terminal is one node
Multiple terminals are required

To execute one script:
Example: python3 MainNode.py 127.0.0.2 5000
	   python3 MainNode.py 127.0.0.1 6000
	   python3 MainNode.py 127.0.0.6 5050
	   python3 MainNode.py 127.0.0.4 6050
If command line arguments are not given the script will use the default values
On exeption a menu will be presented to the user 
Based on user input the program will provide prompts to enter information

Example: if asking to join network the user must input IP and PORT of the node they wish to join

When uploading a file from a node, the file must be present in the directory of the script
When downloading if the file is already present in the directory no change will happen
When downloading make sure the node you are downloading from does not have the same file in it's directory

If error occurs such as "socket not opened" or infinite loop error:
Unfortunately, the only way to fix these errors are to shut down the node and restart. 
If shutting down only one node doesn't fix the error, shutting down the entire network and restarting will solve

To simulate a network of nodes using the Chord DHT protocol, multiple scripts need to be executed


## Libraries used:

These are the libraries required.
 
 socket, random
 
 threading
 
 pickle
 
 sys
 
 time
 
 hashlib
 
 os
 
 from collections import OrderedDict
 
 Most are present by default however if one is unavailable:
 
`sudo pip install <name_of_library>`


