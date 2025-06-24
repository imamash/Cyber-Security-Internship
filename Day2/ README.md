# 🛡️ Task 2: Analyze a Phishing Email Sample

## 🎯 Objective
Identify phishing characteristics in a suspicious email sample and demonstrate email threat analysis skills.

## 🛠 Tools Used
- Email client (Gmail)
- Online email header analyzer: [MxToolbox](https://mxtoolbox.com/EmailHeaders.aspx)
- Web browser (for URL inspection)

---

## 📩 Sample Phishing Email: IRCTC Refund Scam

**Subject:** Refund Pending  
**From:** IRCTC Helpdesk `<irctc-helpdesk@securesupportcloud.com>`  
**To:** `ashrafimam@gmail.com`  
**Claim:** You’re owed a refund of ₹4,240 from IRCTC  
**Action Requested:** Scan a QR code or click a “secure” link to verify your mobile number

---

## 🔍 Phishing Indicators Identified

1. **Spoofed Email Address**  
   - Domain `securesupportcloud.com` is not affiliated with IRCTC.

2. **Failed Email Authentication**  
   - Email headers fail SPF/DKIM verification (likely sent from an untrusted IP).

3. **Suspicious Links/QR Code**  
   - Link redirects to a phishing site, masked as a legitimate IRCTC refund page.

4. **Urgent Language**  
   - "This link will expire in 2 business days" is a pressure tactic.

5. **Mismatched URLs**  
   - Hovered link destination does not match the text shown.

6. **Well-Written but Malicious**  
   - No grammar or spelling errors — designed to appear trustworthy.

---

## ✅ Conclusion

This is a **highly deceptive phishing email** attempting to steal sensitive information using:
- A familiar government entity (IRCTC)
- Fake refund bait
- Urgent call-to-action

**Action Taken:** Do not interact with the link or QR code. Report and delete the email.

---

## 📚 Interview Questions Answered

1. **What is phishing?**  
   A cyberattack using fake emails/websites to steal sensitive information.

2. **How to identify a phishing email?**  
   Check for spoofed sender, urgency, suspicious links, and mismatched URLs.

3. **What is email spoofing?**  
   Faking an email's "From" address to appear as a legitimate sender.

4. **Why are phishing emails dangerous?**  
   They can steal data, install malware, or trick you into payments.

5. **How can you verify the sender’s authenticity?**  
   Verify the domain, hover over links, check SPF/DKIM, and contact the sender via official channels.

6. **What tools can analyze email headers?**  
   - [MxToolbox](https://mxtoolbox.com/EmailHeaders.aspx)  
   - [Google Admin Toolbox](https://toolbox.googleapps.com/apps/messageheader/)

7. **What actions should be taken on suspected phishing emails?**  
   - Don’t click links  
   - Mark as phishing  
   - Report to IT/security  
   - Delete the message

8. **How do attackers use social engineering in phishing?**  
   They use fear, urgency, and familiarity to trick victims into clicking or submitting info.

---

## 📌 Key Concepts
- Phishing
- Email spoofing
- Header analysis
- Social engineering
- Threat detection

--



