# TCP/IP Model

## Learning objectives

By the end of this lesson, you should be able to:

- explain what the TCP/IP model is
- compare it with the OSI model
- describe the layers in the TCP/IP model
- understand why real networks use this model more than the OSI model

## 1. What is the TCP/IP model?

The TCP/IP model is a networking model based on the real protocols used on the Internet.

It is the model most network engineers and operating systems actually use in practice.

Unlike the OSI model, which is conceptual, the TCP/IP model describes the way actual network systems are built.

## 2. Why is it called TCP/IP?

The name comes from two important protocols:

- TCP: Transmission Control Protocol
- IP: Internet Protocol

These are among the most important protocols in the Internet stack.

## 3. The layers in the TCP/IP model

The TCP/IP model is usually described with four layers:

| Layer | Common name | Main role |
|---|---|---|
| 4 | Application | HTTP, DNS, SSH, email, etc. |
| 3 | Transport | TCP and UDP |
| 2 | Internet | IP routing and addressing |
| 1 | Link | Ethernet, Wi-Fi, local network delivery |

This is a simpler model than OSI, and it maps more directly to how real implementations behave.

## 4. What each layer does

### Link layer
This layer handles local communication, including:

- Ethernet
- Wi-Fi
- MAC addressing
- local switching

This is where frames are sent on a local network.

### Internet layer
This layer focuses on logical addressing and forwarding.

It is responsible for IP addressing and routing between networks.

Examples:

- IPv4
- IPv6
- routers

### Transport layer
This layer manages end-to-end communication between hosts.

Important protocols:

- TCP: reliable, ordered, connection-oriented
- UDP: simple, fast, connectionless

### Application layer
This layer contains protocols that users and programs actually use.

Examples:

- HTTP
- HTTPS
- DNS
- SSH
- SMTP

## 5. How it compares with OSI

The OSI model has seven layers. The TCP/IP model has four.

A rough comparison looks like this:

```text
OSI                      TCP/IP
--------------------------------------
Application              Application
Presentation             |
Session                  |
Transport                Transport
Network                  Internet
Data Link                Link
Physical                 Link
```

The exact mapping is not perfect, but the basic idea is:

- OSI is a teaching model
- TCP/IP is a practical implementation model

## 6. Why OSI is still useful

Even though TCP/IP is more practical, OSI is still helpful because it makes the networking stack easier to teach and troubleshoot.

Someone learning networking can understand:

- what layer handles local delivery
- what layer handles routing
- what layer handles reliability
- what layer handles user apps

This helps when diagnosing problems.

## 7. Real-world data flow example

When you open a website, the process roughly follows the TCP/IP model:

1. Your browser uses HTTP or HTTPS at the Application layer
2. TCP or UDP at the Transport layer manages data delivery
3. IP addresses and routing happen at the Internet layer
4. Ethernet or Wi-Fi handles local transmission at the Link layer

This is why a network engineer often thinks in terms of layers even when the implementation is not perfectly separated.

## 8. Simple analogy

Imagine sending a letter from one city to another.

- the application layer is the actual message you want to send
- the transport layer is the postal service that ensures the package is properly handled
- the internet layer is the routing decision about which road or path to use
- the link layer is the local road or address system of the final neighborhood

The analogy is not exact, but it helps explain why different jobs happen in different layers.

## 9. Common beginner misunderstandings

### Mistake 1: Thinking TCP/IP is the same as a protocol
It is a model and a suite of protocols, not one single protocol.

### Mistake 2: Thinking OSI is "wrong"
It is not wrong. It is simply more conceptual than practical.

### Mistake 3: Thinking the Internet uses only one protocol
The Internet uses many protocols together, including IP, TCP, UDP, DNS, HTTP, and TLS.

## 10. Quick review questions

1. Why is the TCP/IP model important?
2. How many layers are usually described in the TCP/IP model?
3. Which layer handles IP routing?
4. Which layer is used by HTTP and DNS?

## 11. Short quiz

1. What is the difference between OSI and TCP/IP?
2. Which TCP/IP layer handles TCP and UDP?
3. Which layer handles IP addresses?
4. Which model is more connected to real Internet implementations?

## 12. Summary

The TCP/IP model is the practical model used in real networking systems. It groups communication into application, transport, internet, and link layers. It is simpler than the seven-layer OSI model, but it is often more useful when discussing actual networks, protocols, and troubleshooting.
