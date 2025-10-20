# Task 1: Local Network Scan for Open Ports

## Objective
Learned how to discover open ports and identify potential security risks within a local network.

## Tools Used
- Nmap
- Wireshark (optional)

## Steps Performed
1. Installed Nmap.
2. Found local IP range using `ip addr show`.
3. Ran TCP SYN scan:
   ```bash
   nmap -sS 192.168.1.0/24 -oN scan_results.txt
4. ran the command -oN scan-results.txt as file 
