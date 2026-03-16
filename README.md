# Task2-Recon-scanning
Network Reconnaissance, Scanning, Packet Analysis and Firewall Testing

## Objective
Learn reconnaissance, scanning, and network traffic analysis 
using industry standard cybersecurity tools on Kali Linux.

## Tools Used
| Tool | Purpose |
|---|---|
| Kali Linux | Main operating system |
| Nmap 7.98 | Port and service scanning |
| Wireshark | Packet capture and analysis |
| hping3 | SYN flood attack simulation |
| iptables | Firewall rule configuration |
| Shodan | Passive reconnaissance |
| Google Dorking | Passive reconnaissance |
| Nslookup | DNS reconnaissance |

## Target Machine
| Detail | Value |
|---|---|
| Machine | Metasploitable 2 |
| IP Address | 192.168.56.101 |
| Attacker IP | 192.168.56.102 |
| Operating System | Linux kernel 2.6.9 to 2.6.33 |

## Task Overview

### 1. Reconnaissance
- Used ip a to identify Kali Linux network interfaces
- Performed ping test to confirm target is alive
- Used Nslookup on scanme.nmap.org
- Performed Google Dorking on testphp.vulnweb.com
- Used Shodan to find exposed FTP devices worldwide

### 2. Port and Service Scanning
- TCP SYN Scan using nmap -sS
- Service Version Detection using nmap -sV
- OS Detection using nmap -O
- UDP Scan using nmap -sU

### 3. Packet Analysis
- Captured DNS traffic in Wireshark
- Captured HTTP traffic in Wireshark
- Simulated SYN flood attack using hping3
- Analyzed attack traffic in Wireshark

### 4. Firewall Testing
- Created iptables rules to block port 80
- Verified firewall using Nmap before and after

## Key Findings
- 23 open TCP ports discovered on target
- Multiple outdated and vulnerable service versions found
- Unencrypted HTTP and FTP traffic visible in plaintext
- SYN flood attack successfully simulated and captured
- iptables firewall successfully blocked port 80
