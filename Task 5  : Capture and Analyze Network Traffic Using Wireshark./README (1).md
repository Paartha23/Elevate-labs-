# 🧾 Wireshark Packet Capture and Analysis

## 📘 Overview
This task demonstrates how to capture, analyze, and interpret network packets using **Wireshark**, a popular open-source network protocol analyzer.  
The objective is to observe real-time network traffic, identify common communication protocols, and understand their roles in the data transmission process.

---

## 🎯 Objective
- To capture network traffic using Wireshark.  
- To filter and analyze packets by protocol type.  
- To identify at least three different protocols observed during the capture.  
- To export and document the findings in a `.pcap` file.

---

## 🧰 Tools Used
- **Wireshark** (latest version)
- **Web Browser (Google Chrome / Firefox)**
- **Command Prompt / Terminal**

---

## ⚙️ Steps Performed

### Step 1: Install Wireshark
- Download Wireshark from the official website: [https://www.wireshark.org](https://www.wireshark.org)
- Complete the installation and ensure **Npcap** is installed to enable packet capturing.

### Step 2: Start Packet Capture
- Launch Wireshark.  
- Select the **active network interface** (e.g., Wi-Fi or Ethernet).  
- Click on the **blue shark fin icon** to start capturing packets.

### Step 3: Generate Network Traffic
- Open a web browser and visit multiple websites (e.g., `https://www.google.com`, `https://www.wikipedia.org`).  
- Alternatively, run a ping command in the terminal:
  ```bash
  ping google.com
  ```
- This generates network traffic for analysis.

### Step 4: Stop Capture
- After about **one minute**, click the **red square button** in Wireshark to stop the capture.

### Step 5: Filter Packets by Protocol
Use Wireshark’s **Display Filter Bar** to view specific protocol packets:
- For DNS packets → `dns`
- For TCP packets → `tcp`
- For HTTP packets → `http`
- For ICMP packets → `icmp`

### Step 6: Identify Common Protocols
During normal web browsing and ping operations, the following protocols are usually captured:

| **Protocol** | **Full Form** | **Purpose** |
|---------------|----------------|--------------|
| **DNS** | Domain Name System | Resolves domain names (e.g., `www.google.com`) into IP addresses. |
| **TCP** | Transmission Control Protocol | Ensures reliable and ordered data delivery between devices. |
| **HTTP / HTTPS** | HyperText Transfer Protocol (Secure) | Transfers web data between client and server. |
| **ICMP** | Internet Control Message Protocol | Used for network testing and ping requests. |
| **ARP** | Address Resolution Protocol | Maps IP addresses to MAC addresses in the local network. |

### Step 7: Export the Capture
- Go to **File → Export Specified Packets**.  
- Save the file as `NetworkCapture.pcap` or `Task5.pcapng` for later analysis.

---

## 📊 Summary of Findings
During the analysis, three primary protocols were identified:
1. **DNS:** Responsible for converting human-readable domain names to IP addresses.  
2. **TCP:** Used to establish reliable connections between devices.  
3. **HTTP/HTTPS:** Handles web data requests and responses for websites visited during the capture.  

Other supporting protocols such as **ARP** and **ICMP** were also observed, showing the underlying operations of local and internet-level communication.

---

## 📄 Conclusion
This experiment successfully demonstrated how network data travels between client and server systems.  
Wireshark provided a clear visualization of packet exchange, showing how different protocols interact within the TCP/IP stack.  
The task enhanced understanding of network behavior, data encapsulation, and real-time protocol operations.

---

## 💾 Files Included
- **Task5.pcapng** → Captured packet file containing DNS, TCP, and HTTP/HTTPS packets.  
- **README.md** → Documentation explaining steps, analysis, and conclusions.
