# HomeLab-NetworkScan-Capture

## Project Overview

In this project, I created a virtualized environment using Oracle VM VirtualBox to simulate network scanning and traffic analysis. The setup involved two virtual machines: one running Ubuntu (as the target) and the other running Kali Linux (as the attacker). The main objective was to demonstrate how network scanning tools like Nmap can be used to map out open ports and services on a target machine, and how Wireshark can be employed to capture and analyze the network traffic generated by such scans.

## Tools Used

- **Oracle VM VirtualBox:** Virtualization software to create isolated environments.
- **Ubuntu:** The target machine for network scanning.
- **Kali Linux:** The attacker machine used to perform the scan.
- **Nmap:** A network scanning tool to discover open ports and services.
- **UFW (Uncomplicated Firewall):** A firewall management tool for configuring security on Ubuntu.
- **Wireshark:** A network protocol analyzer used to capture and analyze traffic.

## Step-by-Step Breakdown

### 1. Setting Up the Virtual Environment

I created two virtual machines using Oracle VM VirtualBox:

- **Ubuntu (Target Machine):** The VM with IP address `10.0.2.15`.
- **Kali Linux (Attacker Machine):** The VM used to perform the network scan.

### 2. Network Mapping with Nmap

On the Kali Linux VM, I ran the following command to scan the Ubuntu machine:

```bash
nmap -A 10.0.2.15
