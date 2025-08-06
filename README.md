# phishing-analysis-task2
Analysis of a phishing email for cybersecurity internship

# Phishing Email Analysis Report

## Email Subject:
Urgent Action Required: Account Verification Needed

## Sender Address:
secure@natbank-finance.com

---

## Indicators of Phishing:

| Indicator              | Description                                                                 |
|------------------------|-----------------------------------------------------------------------------|
| **Spoofed sender**     | Sender domain mimics a real bank (natbank-finance.com), likely fake         |
| **Header mismatch**    | SPF, DKIM, and DMARC all **fail**, indicating forged email origin           |
| **Suspicious IP**      | Email originated from an unknown IP `123.45.67.89` not associated with the bank |
| **Urgent tone**        | Subject and body use threatening language to pressure quick action          |
| **Phishing link**      | Link leads to `secure-bank-login.com` which is not a known bank domain      |
| **Return-Path mismatch** | Differs from visible sender; uses bulk sender format                      |
| **Lack of personalization** | Uses “Dear User” instead of real name, a phishing red flag             |
| **Grammar & style**    | Basic structure and urgency resemble typical scam attempts                  |

---

## Conclusion:

This email demonstrates classic **phishing traits** and should be considered **malicious**. It fails email authentication checks (SPF, DKIM, DMARC), includes a fake login link, uses scare tactics, and tries to steal sensitive information.

**Recommendation:** Never click suspicious links or share personal details in such emails. Always verify the sender from the official website or customer support.

---

## Files Included:

- `phishing_sample.txt` – Email body containing suspicious content  
- `email_header.txt` – Raw spoofed email header  
- `header_analysis_result.txt` – Summary of header authentication and red flags
