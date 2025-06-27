#  Firewall Configuration Report – Task 4

## Objective
Configure the Windows Defender Firewall to block a specific port (Port 23 – Telnet) and demonstrate how firewall rules affect network traffic.

---

##  Tool Used
- **Windows Defender Firewall with Advanced Security** (built into Windows)

---

## What Was Done

### 1. Viewed Existing Inbound Rules
- Opened the firewall management interface via "Windows Defender Firewall with Advanced Security".
- Inspected default rules to understand what's currently allowed.

### 2. Created a Rule to Block Port 23 (Telnet)
- In **Inbound Rules**, created a **New Rule**.
- Selected **TCP**, specific port **23**, and chose **“Block the connection”**.
- Named the rule: `Block Telnet Port 23`.

### 3. Verified Rule Existence
- Ensured the rule was listed and enabled.
- Attempted to test the port using `telnet 127.0.0.1 23`.

### 4. Removed the Rule
- Located the custom rule in **Inbound Rules**.
- Deleted it to restore original firewall behavior.

---

## Screenshots
- Screenshot 1: After creating the block rule for port 23
- Screenshot 2: While deleting the custom rule

(All screenshots are saved inside the `/screenshots/` folder.)

---

## Conclusion

Windows Firewall can effectively control network traffic by blocking specific ports.  
In this task, we successfully created and tested a rule to block port 23 (commonly used for Telnet), demonstrating the ability to filter traffic and enforce local security policies.

---
 **Learning Outcome:**
- Understood how to navigate Windows Firewall settings  
- Learned how to create, test, and remove port-specific rules  
- Saw how firewall behavior impacts communication on specific ports
