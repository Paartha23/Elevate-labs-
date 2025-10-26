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

✅ The firewall will now block all inbound connections using **Telnet** on port **23**.

---

### **Step 4: Test the Rule**
1. Open **Command Prompt**.  
2. Run the following command:
   ```cmd
   telnet localhost 23
