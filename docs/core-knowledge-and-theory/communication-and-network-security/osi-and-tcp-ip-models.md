# OSI and TCP/IP Models

## Why These Models Matter

The **OSI (Open Systems Interconnection)** and **TCP/IP** models are foundational frameworks for understanding how networks communicate. They help cybersecurity professionals design, troubleshoot, and secure networks by defining how data is transmitted, routed, and received across systems.

## OSI Model: 7 Layers

The OSI model is a **conceptual framework** that standardizes network functions into seven layers. Each layer has a specific role and interacts with the layers directly above and below it.

| Layer   | Name         | Function                                                                                       | Security Considerations                                  |
| ------- | ------------ | ---------------------------------------------------------------------------------------------- | -------------------------------------------------------- |
| Layer 7 | Application  | Provides network services to end-user applications (e.g., HTTP, FTP, SMTP).                    | Vulnerabilities in protocols (e.g., SQL injection, XSS). |
| Layer 6 | Presentation | Translates data between the application layer and the network (e.g., encryption, compression). | Data integrity, encryption (e.g., TLS/SSL).              |
| Layer 5 | Session      | Manages sessions/connections between applications (e.g., NetBIOS, RPC).                        | Session hijacking, man-in-the-middle (MITM) attacks.     |
| Layer 4 | Transport    | Ensures end-to-end communication and data integrity (e.g., TCP, UDP).                          | Port scanning, SYN floods, packet sniffing.              |
| Layer 3 | Network      | Handles routing and forwarding of data packets (e.g., IP, ICMP, routers).                      | IP spoofing, routing attacks, DDoS.                      |
| Layer 2 | Data Link    | Manages data framing and physical addressing (e.g., MAC addresses, switches, Ethernet).        | MAC flooding, ARP spoofing, VLAN hopping.                |
| Layer 1 | Physical     | Transmits raw bit streams over physical media (e.g., cables, hubs, repeaters).                 | Physical tampering, eavesdropping, cable tapping.        |

## TCP/IP Model: 4 Layers

The **TCP/IP model** is the practical implementation of the OSI model, used in modern networks (e.g., the Internet). It consolidates the OSI layers into four layers.

| Layer   | Name           | Function                                                                                   | Security Considerations                              |
| ------- | -------------- | ------------------------------------------------------------------------------------------ | ---------------------------------------------------- |
| Layer 4 | Application    | Combines OSI Layers 5-7. Handles high-level protocols (e.g., HTTP, DNS, SSH).              | Application-layer attacks (e.g., DDoS, malware).     |
| Layer 3 | Transport      | Combines OSI Layer 4. Ensures data delivery (e.g., TCP, UDP).                              | Port scanning, SYN attacks, packet injection.        |
| Layer 2 | Internet       | Combines OSI Layer 3. Handles addressing and routing (e.g., IP, ICMP).                     | IP spoofing, routing attacks, fragmentation attacks. |
| Layer 1 | Network Access | Combines OSI Layers 1-2. Manages physical and data link functions (e.g., Ethernet, Wi-Fi). | MAC spoofing, ARP poisoning, physical attacks.       |

## Mapping OSI to TCP/IP

| OSI Layer    | TCP/IP Layer   |
| ------------ | -------------- |
| Application  | Application    |
| Presentation | Application    |
| Session      | Application    |
| Transport    | Transport      |
| Network      | Internet       |
| Data Link    | Network Access |
| Physical     | Network Access |
