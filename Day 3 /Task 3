# 🛡️ Cybersecurity Internship – Task 3: Vulnerability Scan Report

## 📌 Objective
Conduct a basic vulnerability assessment of a personal computer using **Nessus Essentials**, identify risks, and document mitigation steps based on severity and CVSS scores.

---

## 🛠️ Tools Used

- **Scanner:** Nessus Essentials (by Tenable)
- **Scan Type:** Basic Network Scan
- **Target:** Localhost (IP: 192.168.125.154)
- **Report Format:** HTML Export

---

## ✅ Task Execution Steps

1. **Install Nessus Essentials**
   - Downloaded from [https://www.tenable.com/products/nessus](https://www.tenable.com/products/nessus)
   - Registered for a free activation key via email

2. **Configure and Launch Scan**
   - Accessed via `https://localhost:8834`
   - Selected **"Basic Network Scan"** template
   - Set scan target as `192.168.125.154`
   - Started and monitored the scan (~40 minutes duration)

3. **Export and Analyze Report**
   - Exported results in **HTML format**
   - Reviewed summary of vulnerabilities and severity distribution
   - Researched top issues for appropriate fixes

---

## 🔍 Scan Summary

| Severity       | Count |
|----------------|-------|
| **Critical**   | 0     |
| **High**       | 0     |
| **Medium**     | 1     |
| **Low**        | 0     |
| **Informational** | 26  |

---

## 🚨 Most Critical Finding

- **Vulnerability:** SSL Certificate Cannot Be Trusted  
- **CVSS Score:** 6.5 (Medium)  
- **Description:** The target system is using an untrusted or self-signed SSL certificate, which could be intercepted or spoofed.  
- **Recommendation:** Replace the certificate with one issued by a **trusted Certificate Authority (CA)**.  

---

## 🧰 Additional Observations

- **WMI Not Available:** Suggests potential remote management issues  
- **SMB Info Disclosure:** Basic enumeration was possible over SMB  
- **No high-risk vulnerabilities found**, but routine hardening is suggested

---

## 🛡️ Fix Recommendations

- Use valid SSL/TLS certificates from trusted authorities
- Disable or firewall unused services like SMB if not required
- Ensure WMI is properly configured if remote administration is needed
- Keep system software and OS up to date

---

## 🖼️ Screenshots (for Evidence)
_Include the following in your `/screenshots` folder:_
- Scan summary dashboard
- CVSS severity distribution chart
- SSL Certificate vulnerability detail
- Any plugin-level insights

---

## 📂 Repository Structure

