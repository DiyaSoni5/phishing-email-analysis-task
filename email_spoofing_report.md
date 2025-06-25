# 📧 Phishing Email Analysis Report

## 👤 Analyst: Diya  
## 📅 Date: 24 June 2025

---

### 1️⃣ Sample Used

- **Subject**: 🔒 Security Alert: Unusual Sign-in Activity Detected  
- **Sender**: Microsoft Support <micr0soft-support@micr0soft-security-support.com>  
- **Type**: Credential phishing email (Microsoft impersonation)

---

### 2️⃣ Email Content Indicators

This phishing email was designed to impersonate official Microsoft security alerts. Key phishing characteristics in the email content include:

- A fake domain that replaces “o” with “0” to resemble a legitimate Microsoft address.
- Claims of suspicious sign-in activity to scare the recipient.
- A prompt to click a verification link to "unlock" the account.
- Use of urgency and fear ("account will be permanently suspended") to force action.
- No personalized greeting — begins generically with “Dear User.”

📌 **Summary of Traits**:
- Misleading sender address
- Social engineering through fear
- Urgent tone encouraging unsafe action
- Suspicious link to an unverified website

---

### 3️⃣ Header Analysis

- **Tool Used**: Google Admin Toolbox – Message Header Analyzer

**Extracted Header Details:**

- **Message ID**: `B3ACF3544F8F3@micr0soft-security-support.com`
- **From**: `micr0soft-support@micr0soft-security-support.com`
- **To**: `victim@example.com`
- **Date**: 15 May 2024, 10:41:44 PM (GMT+5:30)
- **Delivered After**: 1 second

**Authentication Results:**

| Check     | Result  | Notes                                                                 |
|-----------|---------|-----------------------------------------------------------------------|
| SPF       | ❌ Fail | Sending IP is not authorized by the domain owner                     |
| DKIM      | ❌ Fail | No valid DKIM signature was found                                     |
| DMARC     | ❌ Fail | Domain’s policy requires rejection of unauthenticated messages        |

📌 **Conclusion**:  
The header analysis confirms that the message fails all major email authentication checks. The domain used is spoofed, and the email was likely sent using bulk-sending or automated phishing tools. This strongly indicates that the message is a phishing attempt designed to deceive the user and steal credentials.

