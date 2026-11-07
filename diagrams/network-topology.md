
# Network Topology Diagram

This diagram shows the environment used for the Network Discovery & Security Assessment project.

```text
          MacBook (Host Computer)
                   |
                   |
              UTM Virtualization
                   |
                   |
             Ubuntu Linux VM
              192.168.64.2
                   |
          -------------------
          |        |        |
        Nmap   Wireshark   UFW
       Scanning  Traffic  Firewall
                 Analysis
```

## Environment Components

- **MacBook:** Physical computer hosting the virtual machine.
- **UTM:** Virtualization software used to run Ubuntu.
- **Ubuntu Linux:** Operating system used for the security lab.
- **Nmap:** Used to scan the virtual machine for open and closed ports.
- **Wireshark:** Used to capture and analyze ICMP, DNS, and TCP traffic.
- **UFW:** Configured to manage incoming and outgoing network traffic.

## Lab Target

- Operating system: Ubuntu Linux
- IP address: `192.168.64.2`
- Network scanning: Nmap
- Packet analysis: Wireshark
- Firewall: UFW
