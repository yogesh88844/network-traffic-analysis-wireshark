# Network Traffic Analysis Using Wireshark

## Overview
This project focuses on capturing, analyzing, and understanding different types of network traffic using Wireshark in a controlled virtual lab environment.

Traffic is generated from a Kali Linux machine and captured on a Windows Server using Wireshark.

## Objective
- Capture live network traffic
- Analyze common network protocols
- Understand packet-level communication
- Identify security implications of unencrypted traffic

## Tools Used
- Wireshark
- Kali Linux
- Windows Server
- VMware Workstation (Host-only Network)

## Lab Environment
- Attacker/Traffic Generator: Kali Linux
- Packet Capture Machine: Windows Server
- Network Type: VMware Host-only
- IP Addresses:
  - Kali Linux: 192.168.76.133
  - Windows Server: 192.168.76.132

## Protocols Analyzed
- ICMP (Ping)
- DNS
- HTTP
- FTP
- Nmap Scan Traffic

## Analysis Performed
### ICMP
- Echo Request and Echo Reply packets captured
- Verified network connectivity between systems

### DNS
- DNS queries captured using nslookup
- No responses observed due to absence of DNS server

### HTTP
- HTTP GET and 200 OK responses analyzed
- Observed full TCP handshake and request-response flow

### FTP
- FTP traffic captured in plaintext
- Credentials and file contents visible
- Demonstrates insecurity of unencrypted protocols

### Nmap Scan
- TCP SYN scan traffic captured
- Identified open and closed ports based on SYN-ACK and RST responses

## Security Insights
- Unencrypted protocols expose sensitive data
- Network scans are detectable via packet analysis
- Wireshark is essential for network monitoring and incident analysis

## Documentation
A detailed step-by-step analysis is available in:
Wireshark_Network_Traffic_Analysis_Report.docx

## Disclaimer
This project was performed in a controlled lab environment for educational and ethical purposes only.
