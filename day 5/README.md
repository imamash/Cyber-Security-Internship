# 🔍 Wireshark Network Traffic Capture – Cybersecurity Internship Task

## 📚 About the Project
This repository documents a practical network traffic analysis performed using Wireshark. The task involved capturing live packets, applying specific protocol filters, and summarizing the results.

---

## 🗂 Project Deliverables
- ✅ Live packet capture (.pcapng)
- ✅ Filtered traffic analysis
- ✅ Protocol-specific packet count
- ✅ Screenshots of Wireshark statistics

---

## 🎯 Objectives
- Capture live traffic on the active network interface.
- Apply filters to analyze the following protocols:
  - ip.src
  - dns
  - http
  - icmp
  - tcp
  - udp
- Identify and summarize key traffic patterns.

---

## 📦 Files Included
| File Name                       | Description                       |
|---------------------------------|-----------------------------------|
| wireshark_capture.pcapng      | Packet capture file               |
| README.md                     | Project documentation             |
| protocol_hierarchy.png        | Protocol hierarchy statistics     |
| endpoints.png                 | Active IP sources                 |
| conversations.png             | Captured network conversations    |
| udp_filtered_packets.png      | UDP protocol traffic filter view  |

---

## ⚙ Environment
- *Tool:* Wireshark
- *System:* Windows
- *Capture Duration:* ~1 minute

---

## 📊 Key Results

### ✅ Protocol Summary
- *IPv4 Packets:* 53
- *IPv6 Packets:* 16
- *UDP Packets:* 41
- *TCP Packets:* Minimal/Negligible
- *DNS Packets:* 8
- *HTTP Packets:* Not observed
- *ICMP Packets:* Not observed

---

### ✅ Traffic Insights
- *Dominant Protocol:* UDP  
- *Major Services Identified:*
  - SSDP (Simple Service Discovery Protocol)
  - MDNS (Multicast DNS)
  - DNS Queries to Grammarly services
- *Uncaptured Traffic:* HTTP & ICMP (likely encrypted browsing via HTTPS)

---

## 🔬 Summary of Findings
- *UDP dominated the captured traffic.*
- *DNS lookups to Grammarly domains were present.*
- *Local discovery protocols like SSDP and MDNS were highly active.*
- *Minimal TCP traffic suggests low direct web traffic during capture.*
- *No ICMP (ping) traffic was captured.*

---

## 📌 Notes
- If HTTP browsing was conducted, the traffic may have been encrypted (HTTPS), which is not visible without TLS decryption.
- The analysis focuses on unencrypted protocols only.

---

## 🚀 Submission Checklist
- [x] Packet capture file uploaded
- [x] README report completed
- [x] Protocol screenshots attached
- [x] GitHub repository ready for review

---

## 🙌 Acknowledgements
This analysis was performed as part of the *Cybersecurity Internship: Network Traffic Capture Assignment*.
