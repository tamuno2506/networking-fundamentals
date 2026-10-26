# Week 1 CLI Lab Outputs

1. DNS Lookup (`nslookup`)
```bash
> nslookup crescent.com
Server:  UnKnown
Address:  fe80::90a2:5bff:fedd:4664

Non-authoritative answer:
Name:    crescent.com
Addresses:  64:ff9b::43e1:ff7e
          67.225.255.126

2. Active Connections & Listening Ports (>netstat -an)
Proto  Local Address          Foreign Address        State
  TCP    0.0.0.0:49705          0.0.0.0:0              LISTENING
  TCP    0.0.0.0:57621          0.0.0.0:0              LISTENING
  TCP    127.0.0.1:7768         0.0.0.0:0              LISTENING
  TCP    127.0.0.1:7768         127.0.0.1:49711        ESTABLISHED


3. HTTP Request Headers & TCP Handshake (curl -v)
 Host crescent.com:80 was resolved.
* IPv6: (none)
* IPv4: 67.225.255.126
*   Trying 67.225.255.126:80...
* Established connection to crescent.com (67.225.255.126 port 80) from 172.20.10.2 port 56495
* using HTTP/1.x
> GET / HTTP/1.1
> Host: crescent.com
> User-Agent: curl/8.21.0
> Accept: */*
>
* Request completely sent off
< HTTP/1.1 301 Moved Permanently
< Date: Mon, 26 Oct 2026 03:40:42 GMT
< Server: Apache
< Expires: Mon, 26 Oct 2026 04:40:42 GMT
< Cache-Control: max-age=3600
< X-Redirect-By: WordPress
< Strict-Transport-Security: max-age=31536000; includeSubDomains; preload
< X-Frame-Options: sameorigin
< Upgrade: h2,h2c
< Connection: Upgrade
< Location: https://crescent.com/
< Vary: Accept-Encoding
< Referrer-Policy: no-referrer-when-downgrade
< X-XSS-Protection: 1; mode=block
< X-Permitted-Cross-Domain-Policies: none
< X-Content-Type-Options: nosniff
< Content-Length: 0
< Content-Type: text/html; charset=UTF-8
<
* Connection #0 to host crescent.com:80 left intact
