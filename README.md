# Network Security & Traffic Analysis

This repository focuses on network traffic analysis and basic security concepts
using packet captures and theoretical analysis.

## Topics Covered
- TCP/DNS Packet Analysis
- ARP Spoofing (Theory)
- Network Vulnerabilities
- Mitigation Techniques

## Tools
- Wireshark
- Linux

## Learning Outcomes
- Traffic interpretation
- Security awareness
- Defensive networking concepts

---

This repository demonstrates entry-level SOC and NOC analytical skills,
including packet inspection, protocol analysis, and security awareness.


## Quick Diagram: DNS → TCP Flow

```mermaid
sequenceDiagram
Participant C as Client
Participant D as DNS Server
Participant S as Server

C->>D: DNS Query (UDP/53)
D-->>C: DNS Response (IP)
C->>S: TCP SYN
S-->>C: TCP SYN-ACK
C->>S: TCP ACK
C->>S: Web Data
S-->>C: Web Response
