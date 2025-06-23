# Cyber-Security-Internship
Elevate Labs Assignment
# Cyber Security Internship – Task 1

**Intern:** Imam Ashraf  
**Email:** ashrafimam121@gmail.com  
**Date:** 23-06-2025  

## Objective

The objective of this task was to explore **network reconnaissance techniques** using open-source tools such as **Nmap** and **Wireshark**. The goal was to:

- Discover devices and open ports in a local network.
- Understand the security implications of exposed services.

---

## Tools Used

| Tool      | Purpose                               |
|-----------|----------------------------------------|
| Nmap      | Network scanning & open port detection |
| Wireshark | Packet-level traffic capture & analysis |

---

## Step-by-Step Process

### Step 1: Discover Local Network Range
Used `ifconfig` (Linux) to identify the system's local IP address.

### Step 2: Run a SYN Scan Using Nmap
**Command Used:**
```bash
nmap -sS 192.168.125.0/24
```

- `-sS` performs a TCP SYN (half-open) scan.
- Detected live hosts and open services.

**Example Output:**
```
Nmap scan report for 192.168.125.211
Host is up (0.0031s latency).

PORT   STATE SERVICE
53/tcp open  domain
```
> Indicates that a DNS service is running on port 53.

### Step 3: Analyze Traffic Using Wireshark
- Observed IPv6 multicast packets and ICMPv6 Neighbor Discovery.
- Helped identify devices and understand their communication.

---

## Interview Questions & Answers

1. **What is an open port?**  
   A network interface actively listening for incoming connections. (e.g., port 53 = DNS)

2. **How does Nmap perform a TCP SYN scan?**  
   Sends SYN → receives SYN-ACK (open) or RST (closed). It doesn’t complete the handshake.

3. **What risks are associated with open ports?**  
   Unauthorized access, information leakage, and exploitation of vulnerabilities.

4. **Difference between TCP and UDP scanning?**  
   TCP is reliable and connection-based; UDP is connectionless and harder to detect.

5. **How can open ports be secured?**  
   Close unused ports, configure firewalls, restrict access, and update services.

6. **What is a firewall’s role regarding ports?**  
   Filters network traffic based on port/protocol rules to block unauthorized access.

7. **What is a port scan and why do attackers perform it?**  
   It discovers open ports to identify exploitable services.

8. **How does Wireshark complement port scanning?**  
   It verifies Nmap results by analyzing actual traffic and detecting anomalies.

---

## Learning Outcomes

- Performed network reconnaissance using Nmap.
- Interpreted scan results and understood the associated security risks.
- Analyzed packet-level data using Wireshark.
- Practiced real-world documentation and analysis of network scans.
