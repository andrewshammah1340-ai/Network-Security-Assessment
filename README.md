# Network Discovery & Security Assessment

## Project Overview

This project is a hands-on cybersecurity lab designed to explore basic network discovery, traffic analysis, and Linux firewall configuration.

Using an Ubuntu virtual machine, I performed network scans with Nmap, analyzed network traffic with Wireshark, and configured UFW (Uncomplicated Firewall) to practice foundational network security concepts.

## Project Objectives

- Perform network discovery and port scanning.
- Identify open and closed network ports.
- Analyze ICMP, DNS, and TCP network traffic.
- Understand the TCP three-way handshake.
- Identify locally listening services.
- Configure basic Linux firewall rules.
- Document security findings and observations.

## Tools & Technologies

| Tool | Purpose |
|---|---|
| Ubuntu Linux | Lab operating system |
| UTM | Virtual machine environment |
| Nmap | Network discovery and port scanning |
| Wireshark | Network packet analysis |
| UFW | Linux firewall configuration |
| Terminal | Command-line administration |

## Project Activities

### 1. Network Discovery with Nmap

Performed service detection scans against my Ubuntu virtual machine.

- Identified the target IP address.
- Scanned the default 1,000 TCP ports.
- Saved scan results before and after firewall configuration.
- Observed that all 1,000 scanned ports were closed in both scans.

### 2. Network Traffic Analysis with Wireshark

Captured and analyzed three types of network traffic:

- **ICMP:** Examined network diagnostic traffic using ping.
- **DNS:** Observed domain name resolution when accessing websites.
- **TCP:** Identified the TCP three-way handshake (SYN, SYN-ACK, ACK).

Original packet capture files are included in the `captures` folder.

### 3. Linux Firewall Configuration

Configured UFW with the following policies:

- Default incoming
