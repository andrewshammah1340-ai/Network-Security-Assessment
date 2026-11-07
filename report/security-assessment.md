# Network Security Assessment Report

## 1. Objective
The objective of this project was to build a beginner cybersecurity lab using Ubuntu Linux, Nmap, Wireshark, and UFW to explore network scanning, packet analysis, and basic firewall configuration.

## 2. Lab Environment
- Host computer: MacBook
- Virtualization software: UTM
- Operating system: Ubuntu Linux
- Target IP address: 192.168.64.2

## 3. Network Scanning
I used Nmap 7.98 to scan my Ubuntu virtual machine.

Command used:
`nmap -sV 192.168.64.2`

**Initial scan findings:**
- Host was online.
- 1,000 default TCP ports were scanned.
- 1,000 ports were closed.
- 0 open ports were identified.

I saved the results in `scans/first-scan.txt`.

## 4. Firewall Configuration
I checked the initial UFW firewall status and found that it was inactive.

I then configured UFW with:
- Default incoming policy: Deny
- Default outgoing policy: Allow

I enabled the firewall and verified that it was active.

## 5. Second Nmap Scan
After enabling UFW, I performed another Nmap scan.

The results were:
- Host was online.
- 1,000 default TCP ports were scanned.
- 1,000 ports were closed.
- 0 open ports were identified.

The results were consistent with the initial scan. Since all scanned ports were already closed, I cannot conclude that enabling UFW caused the ports to close.

## 6. Wireshark Packet Analysis

I used Wireshark to capture and examine three types of network traffic.

**ICMP**
- Used ping to observe network requests and replies.
- Learned how ICMP helps with network diagnostics.

**DNS**
- Used a domain name to generate DNS traffic.
- Observed how DNS translates domain names into IP addresses.

**TCP**
- Used curl to connect to a website.
- Observed the TCP three-way handshake:
  - SYN
  - SYN-ACK
  - ACK

## 7. Skills Developed
- Linux command-line administration
- Nmap network scanning
- Wireshark packet analysis
- TCP/IP networking fundamentals
- DNS and ICMP concepts
- Linux firewall configuration
- Basic security documentation

## 8. Conclusion
This project gave me practical experience with networking and cybersecurity tools. I learned how to scan a Linux system, analyze network traffic, configure a firewall, and document security testing results.

It also helped me better understand how network protocols operate and how basic security controls are used in a Linux environment.

## Key Findings & Lessons Learned

### Nmap Network Scanning
- The Ubuntu virtual machine was reachable at 192.168.64.2.
- The first scan identified all 1,000 default TCP ports as closed.
- The second scan, performed after enabling UFW, also showed all 1,000 ports as closed.
- This demonstrated how Nmap can identify the status of network ports.

### Wireshark Packet Analysis
- ICMP packets demonstrated network connectivity testing.
- DNS packets showed how domain names are resolved into IP addresses.
- TCP analysis revealed the three-way handshake: SYN, SYN-ACK, and ACK.

### Firewall Configuration
- Configured UFW to deny incoming connections by default.
- Configured UFW to allow outgoing connections.
- Verified that the firewall was active.
- Learned how basic firewall policies help control network traffic.

### Lessons Learned
Through this project, I gained practical experience with:
- Linux command-line tools.
- Network discovery using Nmap.
- Packet analysis using Wireshark.
- Understanding TCP/IP networking.
- Basic Linux firewall administration.
- Documenting technical findings.

### Future Improvements
- Investigate additional network services.
- Explore firewall logging and traffic filtering.
- Perform additional authorized network scans.
- Develop deeper knowledge of network security and vulnerability assessment.
