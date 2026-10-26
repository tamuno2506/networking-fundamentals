# Week 1: Networking Foundations & OSI Model

## Core Objectives Completed
-  Mastered the 7 layers of the OSI model and 4 layers of the TCP/IP model.
-  Studied data encapsulation and PDU transitions (Data -> Segment -> Packet -> Frame -> Bit).
-  Memorized essential TCP/UDP port numbers (SSH, HTTP, HTTPS, DNS, DHCP).
-  Executed CLI micro-labs using `nslookup`, `netstat`, and `curl`.
-  Captured live traffic in Wireshark to analyze the TCP 3-way handshake.

## Key Takeaways & Reflections
- **Encapsulation:** As data moves down the OSI stack, each layer adds its own header (and trailer at Layer 2), wrapping the payload securely.
- **Port Behavior:** Ports act as application identifiers at Layer 4, ensuring traffic reaches the correct service daemon.
