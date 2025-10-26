# 🔒 Task 4: Setup and Use a Firewall on Windows

## 🎯 Objective
To configure and test firewall rules using **Windows Defender Firewall** in order to control and filter network traffic.  
The goal is to demonstrate how firewall rules can be used to allow or block specific ports, ensuring system security.

---

## 🧰 Tools Used
- **Windows Defender Firewall with Advanced Security**

---

## ⚙️ Step-by-Step Implementation

### **Step 1: Open Firewall Settings**
1. Go to **Control Panel → System and Security → Windows Defender Firewall**.  
2. Click **“Advanced Settings”** on the left sidebar.  
   This opens the **Windows Defender Firewall with Advanced Security** console.

---

### **Step 2: View Existing Rules**
- Click **Inbound Rules** to view a list of existing allowed or blocked connections.

---

### **Step 3: Create a Rule to Block Telnet (Port 23)**
1. In **Inbound Rules**, click **New Rule** on the right side.  
2. Select **Port**, then click **Next**.  
3. Choose **TCP**, and under **Specific local ports**, type `23`.  
4. Click **Next**, select **Block the connection**, and click **Next** again.  
5. Check all profiles (**Domain**, **Private**, and **Public**) and click **Next**.  
6. Give the rule a name such as **Block Telnet Port 23**, and click **Finish**.

 The firewall will now block all inbound connections using **Telnet** on port **23**.

---

### **Step 4: Test the Rule**
1. Open **Command Prompt**.  
2. Run the following command:
   ```cmd
   telnet localhost 23

**Commands used for completing the task**
1.For making sure it is blocked after creating the Inbound rule 
```cmd
telnet localhost 23
```

**How the Firewall filters traffic**
1.A firewall works like a security guard that checks every piece of data trying to enter or leave your computer. It decides what’s safe and what’s not based on a set of rules created by the user or the system. These rules act as filters that control network traffic, protecting your device from unwanted or harmful connections.

When data moves across a network, it travels in small packets. The firewall examines each packet’s source address, destination address, port number, and protocol to decide whether it should be allowed or blocked.

**Traffic Inspection**

Every packet that reaches your computer is inspected by the firewall. It checks where the packet is coming from, where it’s going, and what service or port it’s trying to use. For example, if a packet is trying to use port 23 (Telnet), and a rule exists to block that port, the firewall will immediately stop it.

**Rule Matching**

Firewalls operate based on a list of rules. Each rule defines conditions for allowing or blocking traffic.

If the packet matches an allow rule (like SSH on port 22), it is permitted to pass through.

If it matches a deny rule (like Telnet on port 23), it’s blocked right away.

If it doesn’t match any rule, the firewall applies its default policy (usually “deny all incoming traffic”).

 **Inbound and Outbound Filtering**

Inbound filtering controls data coming into your computer. It protects your system from unauthorized users or malware trying to connect.

Outbound filtering manages data leaving your computer. It prevents malicious software from sending information to the internet.

**Profiles and Context**

Firewalls can apply different rules depending on where you are connected:

Domain network: used in office or organizational settings.

Private network: home networks where you trust other devices.

Public network: open Wi-Fi or café networks, where stricter blocking is applied.

This ensures the right level of protection depending on your environment.

**Logging and Monitoring**

Most firewalls log their activity. These logs help users or administrators see which connections were allowed or blocked, making it easier to spot unusual or suspicious activity.



