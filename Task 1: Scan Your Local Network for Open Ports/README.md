# Task 1: Local Network Scan for Open Ports

## Objective
Learned how to discover open ports and identify potential security risks within a local network.

## Tools Used
- Nmap
- Wireshark 

## Steps Performed
1. Installed Nmap.
2. Found local IP range using `ifconfig`.
3. Ran TCP SYN scan:
   ```bash
   nmap -sS 192.168.1.0/24 -oN scan_results.txt
4. ran the command -oN scan-results.txt to save  as file 
5. Found open ports which are
     http(80)-Web server running
     ssh(22)-secure shell acess
     smb(445)-file sharing on windows/linux systems
     135-Microsoft Remote Procedure Call
     53-DNS
     20/21/22-TCP
## Potential Security Risks from Open Ports
1.Open ports can be entry points for attackers if the services behind them are not properly secured.
2.Each open port increases the attack surface for potential exploits.
3.HTTP/Proxy ports (8080) may expose admin panels or unencrypted data.
4.Access should be restricted to trusted internal systems or via VPN.
5.If these protocols are found open, data is transmitted in plain text and can be intercepted.  
     
