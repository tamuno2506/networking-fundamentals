# Week 1: Essential Ports and Protocols Cheat Sheet

## Common Networking & Security Ports

 Port Number | Protocol | Transport Layer | Description / Use Case |

 **20 / 21** | FTP (File Transfer Protocol) | TCP | Legacy unencrypted file transfer (Port 21 = Control, Port 20 = Data). 
 
 **22** | SSH (Secure Shell) / SFTP | TCP | Secure encrypted remote command-line access and secure file transfers. 
 
 **23** | Telnet | TCP | Unencrypted legacy remote command-line management (avoid in production). 
 
 **25** | SMTP | TCP | Simple Mail Transfer Protocol for mail server-to-server relay. 
 
 **53** | DNS (Domain Name System) | UDP / TCP | Resolves human-readable domain names to numerical IP addresses. 
 
 **67 / 68** | DHCP (Dynamic Host Configuration Protocol) | UDP | Automatic IP address and network configuration assignment. 
 
 **80** | HTTP | TCP | Unencrypted web traffic (Hypertext Transfer Protocol). 
 
 **123** | NTP (Network Time Protocol) | UDP | Synchronizes clocks across enterprise network devices and servers. 
 
 **389** | LDAP (Lightweight Directory Access Protocol) | TCP / UDP | Protocol for querying and managing directory services. 
 
 **443** | HTTPS | TCP | Secure encrypted web traffic (HTTP over TLS/SSL). 
 
 **445** | SMB (Server Message Block) | TCP | Network file sharing and printer sharing in Windows environments. 
 
 **636** | LDAPS (Secure LDAP) | TCP / UDP | Encrypted directory service queries over TLS/SSL. 
 
 **587 / 465** | SMTP Secure (Submission) | TCP | Secure email submission from clients to mail servers. 
 
 **993** | IMAPS | TCP | Secure email retrieval protocol (Internet Message Access Protocol over TLS). 
 
 **995** | POP3S | TCP | Secure email download protocol (Post Office Protocol v3 over TLS). 
 
 **3389** | RDP (Remote Desktop Protocol) | TCP / UDP | Graphical remote administration for Windows systems. 

## Key Rules of Thumb for Security
- **Encrypt by Default:** Always prefer secure ports over unencrypted legacy ports (e.g., use SSH [22] instead of Telnet [23]; use HTTPS [443] instead of HTTP [80]).
- 
- **Transport Selection:**
- Use **TCP** when data integrity and reliable delivery are mandatory (handshakes, error checks).
- 
-  Use **UDP** when speed and minimal latency override delivery guarantees (DNS queries, NTP sync).
