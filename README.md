#TCPDump Capture Lab – CLI-Based Packet Analysis

This repository documents my hands-on lab using **tcpdump** for capturing and analyzing network traffic on Linux. I used **netcat** to simulate TCP connections between two systems in an isolated lab to observe real-time packet behavior, including the TCP 3-way handshake.

---

## Objectives

- Capture real-time network traffic using `tcpdump`
- Simulate TCP traffic using `netcat`
- Understand the TCP 3-way handshake (SYN, SYN-ACK, ACK)
- Apply BPF (Berkeley Packet Filter) expressions
- Analyze raw packet headers and protocol behavior

---

## Tools Used

-  Kali Linux (tcpdump CLI tool)
-  Windows VM (netcat client)
-  Netcat for simulating TCP traffic
-  VirtualBox / UTM for VM networking

---

## Files Included

- `TCPDump Analysis Report.pdf` – Full lab report with step-by-step explanation and screenshots
- (Optional) `.pcap` files and example outputs

---

##  Sample tcpdump Commands

```bash
tcpdump -i eth0
tcpdump -nn -v -X port 80
tcpdump -i eth0 src host 192.168.1.5
tcpdump -w capture.pcap
tcpdump -r capture.pcap

⚠️ Disclaimer

All traffic was generated in a safe, controlled, offline lab environment.
No unauthorized scanning or data capture was performed.
This lab is for educational and ethical learning purposes only.
