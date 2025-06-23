# 🔐 Cyber Security Internship – Task 1

**👤 Intern:** Imam Ashraf  
**📧 Email:** ashrafimam121@gmail.com  
**📅 Date:** 23-06-2025  

---

## 🎯 Objective

This task focused on using open-source tools like **Nmap** and **Wireshark** for **network reconnaissance**. The main objectives were to:

- Discover devices and open ports within a local network.
- Analyze security implications of open services.
- Gain hands-on experience in interpreting scan results and analyzing packet-level data.

---

## 🧰 Tools Used

| Tool      | Purpose                               |
|-----------|----------------------------------------|
| **Nmap**  | Network scanning and port detection    |
| **Wireshark** | Packet capture and traffic analysis |

---

## 🧪 Step-by-Step Process

### 🔹 Step 1: Discover Local Network Range
Used `ifconfig` (Linux) to identify the system’s IP and network block.

### 🔹 Step 2: Run a SYN Scan Using Nmap

**Command:**
```bash
nmap -sS 192.168.125.0/24
Nmap scan report for 192.168.125.211
Host is up (0.0031s latency).

PORT   STATE SERVICE
53/tcp open  domain
