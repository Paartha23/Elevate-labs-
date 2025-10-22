# Phishing Email Analysis - Task 2

This repository contains a safe sample phishing email and its analysis.  
All analysis is based on a fake `.eml` file (`phish-sample.eml`). **No real malware is included.**  

---

## 2. Examine sender's email address for spoofing
- Display name: **"Account Security Team"**  
- From address: `support@secure-bankalerts.com`  
- Reply-To: `verify@secure-bankalerts.com`  
- Return-Path: `bounce@secure-bankalerts.com`  
- **Finding:** The domain does not match the claimed organization;  

---

## 3. Check email headers for discrepancies
- SPF: **Fail** (sending IP not authorized)   
- Sending IP: `84.17.23.45` (not official)  
- **Finding:** Multiple mismatches in headers confirms  a phished email sender.  

---

## 4. Identify suspicious links or attachments
- Link displayed as: `https://www.bankofamerica.com/security-update`  
- Actual href: `http://secure-login-update.info/boa`  
- Attachment: `Account_Verify.docx` (placeholder safe file)  
- **Finding:** Mismatched links and suspicious attachment indicates as  phishing mail .  

---

## 5. Look for urgent or threatening language
-  it includes Phrases like :  
  - "Failure to verify within 24 hours will result in permanent account closure"  
  - "To restore access immediately"  
- **Finding:** Uses urgency to pressure the recipient into action which is not usually done in emails.  

---

## 6. Note any mismatched URLs
- Hovering over link shows `http://secure-login-update.info/boa`  
- Visible URL appears legitimate but actual URL is attacker-controlled  
- **Finding:** Fake link it doen't matches with the real  one .  

---

## 7. Verify presence of spelling or grammar errors
- Examples: `"unusal"` instead of "unusual", `"suspanded"` instead of "suspended"  
- **Finding:** speeling mistakes found which makes it a phishing mail.  

---

## 8. Phishing traits summary
- The sender is fake and the email comes from a suspicious domain.  
- Links and attachments are unsafe or misleading.  
- The message uses urgent language and has spelling mistakes.  
- Overall risk is HIGH — do not click links or open attachments.

---


- Evidence screenshots, headers, and URL analysis are stored in the `evidence/` folder.  

