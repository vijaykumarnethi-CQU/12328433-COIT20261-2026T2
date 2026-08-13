# Week 03 | Netcat and Packet Capture

## Overview

In this week's lab, I used **GNS3** to test application communication using Netcat and capture network packets using GNS3 packet capture.

## Task 1 - Netcat

I used two Linux Hosts to demonstrate client-server communication.

The server was started on Host B using:

```bash
nc -l -p 23456
```

The client on Host A connected using:

```bash
nc 10.1.1.2 23456
```

I sent my name from the client to the server and my student ID from the server to the client.

![Netcat Client and Server](images/Netcat-Basics-client-server.png)

## Task 2 - Packet Capture

I started a packet capture on the link between Host A and the switch.

I then sent three ping requests from Host A to Host B:

```bash
ping -c 3 10.1.1.2
```

I also used Netcat to send my name from Host A to Host C.

The captured packets were saved as:

```text
Capture-Basics-YOURSTUDENTID-ping-netcat.pcap
```

## Reflection

This lab helped me understand application-level communication using Netcat and how GNS3 can capture network traffic for further analysis.
