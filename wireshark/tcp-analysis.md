
**wireshark/tcp-analysis.md**
```markdown
# TCP Packet Analysis (Wireshark)

## 3-way handshake
1. SYN
2. SYN/ACK
3. ACK

Filters:
```text
tcp
tcp.flags.syn == 1 && tcp.flags.ack == 0
