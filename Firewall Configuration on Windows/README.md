# 🔐 Task 4: Firewall Configuration on Windows

## 💡 Objective
Configure Windows Defender Firewall to:
- ✅ Block all inbound traffic on **port 23 (Telnet)** — an insecure protocol
- ✅ Allow inbound traffic on **port 22 (SSH)** — a secure protocol for remote login

This demonstrates both traffic filtering and secure access setup.

---

## 🛠 Tools Used
- **Operating System:** Windows 10 / 11
- **Firewall Utility:** Windows Defender Firewall with Advanced Security

---

## 🧾 Steps Performed

### 🔴 1. Block Inbound Traffic on Telnet (Port 23)

- Opened Windows Defender Firewall → Advanced Settings → Inbound Rules → New Rule
- Selected:
  - **Protocol:** TCP
  - **Local Port:** 23
  - **Action:** Block the connection
  - **Profile:** All
  - **Rule Name:** `imam_rule_assignment`
  - **Description:** Blocks all inbound traffic coming from 23 TCP telnet

### 🟢 2. Allow Inbound Traffic on SSH (Port 22)

- Again opened New Inbound Rule wizard
- Selected:
  - **Protocol:** TCP
  - **Local & Remote Port:** 22
  - **Action:** Allow the connection
  - **Profile:** All
  - **Rule Name:** `ssh port22`

---

## 📸 Screenshots

| File Name | Description |
|-----------|-------------|
| `Screenshot_Telnet_Block_1.png` | Telnet block rule listed as `imam_rule_assignment` |
| `Screenshot_Telnet_Block_2.png` | Rule properties showing TCP port 23 |
| `Screenshot_SSH_Allow_1.png` | SSH rule showing port 22 in wizard |
| `Screenshot_SSH_Allow_2.png` | Rule named `ssh port22` |
| `Screenshot_SSH_Allow_3.png` | SSH rule visible in the Inbound Rules list |

---

## 🎯 Outcome
- ✅ Hardened the system by blocking Telnet (an outdated and insecure protocol).
- ✅ Allowed SSH securely, ensuring legitimate remote access when required.
- ✅ Demonstrated the ability to configure and validate custom inbound rules in Windows Firewall.

---

## 📚 Interview Q&A Summary

**Q1: What is a firewall?**  
A firewall filters traffic to/from your device based on rules. Windows Firewall blocks or allows specific traffic.

**Q2: Difference between stateful vs stateless firewall?**  
- *Stateful:* Tracks ongoing connections (Windows Firewall is stateful)  
- *Stateless:* Treats every packet as new

**Q3: What are inbound and outbound rules?**  
- *Inbound:* Traffic entering your system  
- *Outbound:* Traffic going out  
We used *inbound rules* in this task.

**Q4: Why block port 23 (Telnet)?**  
It’s insecure and sends credentials in plaintext — blocking it prevents unauthorized access.

**Q5: Why allow port 22 (SSH)?**  
SSH is secure and encrypted — essential for remote server access and administration.

**Q6: Common firewall mistakes?**  
Leaving critical ports open, misconfigured rules, allowing too many programs.

**Q7: What is NAT in firewalls?**  
Network Address Translation maps internal IPs to public IPs; firewall filters traffic post-mapping.

---
