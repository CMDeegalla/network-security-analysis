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

## Quick Diagram: DNS → TCP Flow

```mermaid
sequenceDiagram
participant C as Client
participant D as DNS Server
participant S as Server
C->>D: DNS Query (UDP/53)
D-->>C: DNS Response (IP)
C->>S: TCP SYN
S-->>C: TCP SYN-ACK
C->>S: TCP ACK
C<->>S: Web Data
