# Network-Security-Assessment
Beginner cybersecurity project using Ubuntu, Nmap, and Wireshark.
# Network Security Assessment

## Project Overview
This project demonstrates a beginner cybersecurity lab built using Ubuntu Linux, Nmap, and Wireshark. The goal was to explore network discovery, analyze network traffic, identify listening services, and practice basic system hardening.

## Tools Used
- Ubuntu Linux
- UTM Virtual Machine
- Nmap
- Wireshark
- UFW Firewall
- Linux Terminal

## Project Activities

### 1. Network Scanning with Nmap
- Scanned my Ubuntu virtual machine using Nmap.
- Used service detection with `nmap -sV`.
- Identified the status of the 1,000 default TCP ports scanned.
- Saved scan results before and after firewall configuration.

### 2. Network Traffic Analysis with Wireshark
Captured and analyzed three types of network traffic:

- **ICMP:** Observed ping requests and replies.
- **DNS:** Examined how domain names are resolved into IP addresses.
- **TCP:** Observed the TCP three-way handshake (SYN, SYN-ACK, ACK).

### 3. Firewall Configuration
- Checked the initial UFW firewall status.
- Configured the firewall to deny incoming connections by default.
- Allowed outgoing connections.
- Enabled UFW and verified its status.

## Results
- Nmap identified the virtual machine as online.
- All 1,000 default TCP ports scanned were closed in both scans.
- Successfully captured and analyzed ICMP, DNS, and TCP traffic.
- Enabled UFW firewall protection with default incoming-deny and outgoing-allow policies.

## What I Learned
- How to use Linux command-line tools.
- How network scanning works.
- How to recognize common network protocols.
- How DNS, ICMP, and TCP traffic work.
- How to configure a basic Linux firewall.
- How to document cybersecurity testing results.

## Conclusion
This project provided hands-on experience with basic network security concepts, Linux administration, network traffic analysis, and firewall configuration.
