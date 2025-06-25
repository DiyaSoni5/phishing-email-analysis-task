# phishing-email-analysis-task
# 🛡️ Phishing Email Analysis: Fake Microsoft Security Alert

## 📌 Objective

The goal of this task is to analyze a suspicious email pretending to be from Microsoft Support and identify phishing indicators using email header analysis tools. The focus is on recognizing spoofed sender addresses, failed authentication mechanisms, and social engineering techniques.


## 📥 Email Sample Overview

**Subject:** 🔒 Security Alert: Unusual Sign-in Activity Detected  
**From:** "Microsoft Support" <micr0soft-support@micr0soft-security-support.com>  
**To:** <victim@example.com>  
**Date:** May 15, 2024, 10:41 PM IST  
**Tool Used:** [Google Admin Toolbox - Messageheader](https://toolbox.googleapps.com/apps/messageheader/)

---

## 🔍 Phishing Indicators Identified

| Indicator                 | Description |
|---------------------------|-------------|
| **📛 Spoofed Sender**      | Email uses a misleading domain `micr0soft-security-support.com` instead of a real Microsoft domain. |
| **📉 SPF Check Failed**    | SPF failed — the IP address is not authorized to send on behalf of the domain. |
| **🔐 DKIM Failed**         | DKIM signature verification failed, indicating a lack of message integrity. |
| **❌ DMARC Failed**        | DMARC failed — domain policy requires rejection of unverified messages. |
| **⚠️ Urgent Language**     | Threatens permanent account suspension to create fear and urgency. |
| **🧠 Social Engineering**  | Exploits fear of account compromise to trick users into clicking a fake verification link. |
| **🚫 Suspicious Link**     | URL in the email points to a fake Microsoft site not affiliated with the company. |
| **🧩 Email Sent via Script** | Header analysis indicates it was likely sent using automated tools or bots. |

---

## 🧰 Tools Used

- **Google Admin Toolbox: Messageheader**  
  👉 [https://toolbox.googleapps.com/apps/messageheader/](https://toolbox.googleapps.com/apps/messageheader/)

---

## 📚 Key Concepts Demonstrated

- Email Spoofing Detection  
- SPF, DKIM, and DMARC Header Analysis  
- Social Engineering Identification  
- Phishing Threat Recognition

---

## ✅ Conclusion

This phishing email is a textbook case of sender spoofing, impersonation, and social engineering. It fails all key email authentication checks and uses scare tactics to pressure the recipient. Analyzing this message enhanced my ability to identify email threats, interpret headers, and understand real-world phishing indicators.
