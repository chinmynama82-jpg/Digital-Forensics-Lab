# Ex. No. 04 – Email Header Analysis and Spoofing Detection using MHA

## Aim

To analyse email headers using Mail Header Analyzer (MHA) and identify possible email spoofing by examining email routing information and authentication mechanisms such as SPF, DKIM, and DMARC.

## Tool Used

* Mail Header Analyzer (MHA)
* Gmail
* Web Browser
* Email Header

## Objective

The objectives of this experiment are:

* To obtain the original email header from Gmail.
* To analyse email header information using MHA.
* To examine the Received headers and IP addresses.
* To analyse SPF, DKIM, and DMARC authentication results.
* To examine the Message-ID and Return-Path.
* To identify possible anomalies related to email spoofing.

# Procedure

## Step 1: Access the Original Email Header

Gmail was opened and an email was selected for analysis.

The three-dot menu was opened and **Show original** was selected to view the complete email header.

The original message displayed important information such as:

* Message ID
* From
* To
* Subject
* SPF
* DKIM
* DMARC

### Screenshot

<img width="1901" height="666" alt="Screenshot 2026-08-26 202644" src="https://github.com/user-attachments/assets/e1428b88-dcaf-4b66-8fa2-1b9df7615972" />


---

## Step 2: Copy the Email Header

The **Copy to clipboard** option was selected from the Gmail Original Message page.

The complete email header was copied for further analysis using Mail Header Analyzer.

---

## Step 3: Open Mail Header Analyzer (MHA)

The Mail Header Analyzer (MHA) web tool was opened in a browser.

The copied email header was pasted into the message header input area.

The **Analyze headers** option was selected to analyse the email header.



<img width="1836" height="545" alt="image" src="https://github.com/user-attachments/assets/c2925b1b-5086-403e-af3d-753f93784d44" />

---

## Step 4: Analyse the Received Headers

The MHA result displayed the Received headers that describe the path followed by the email through different mail servers.

The following information was examined:

* Hop number
* Submitting host
* Receiving host
* Time
* Delay
* Connection type
* IP address and hostname information

The received header information was checked for unusual servers, IP addresses, or routing anomalies.

---

## Step 5: Analyse SPF, DKIM and DMARC

The email authentication results were examined.

The results obtained from the analysed email were:

* **SPF: PASS**
* **DKIM: PASS**
* **DMARC: PASS**

SPF was checked to determine whether the sending IP address was authorised to send email for the domain.

DKIM was checked to verify the email's cryptographic signature.

DMARC was checked to verify domain alignment and authentication policy.

These authentication results did not indicate an obvious spoofing attempt.

---

## Step 6: Examine Message-ID and Return-Path

The **Message-ID** and **Return-Path** fields were examined to identify the domain and routing information associated with the email.

The Message-ID was associated with the email delivery infrastructure, while the Return-Path provided the address used for handling bounced messages.

These fields were compared with the sender information to identify possible inconsistencies.

---

## Step 7: Analyse the Diagnostics Report

The MHA **Diagnostics Report** was opened to identify additional header-related issues.

The report indicated that the following header was missing:

```text
X-Microsoft-Antispam-Mailbox-Delivery
```

This was recorded as a missing header field in the MHA diagnostic report.

The missing header alone was not considered sufficient evidence of email spoofing because the SPF, DKIM, and DMARC authentication results were successful.

### Screenshot

<img width="1917" height="752" alt="image" src="https://github.com/user-attachments/assets/0912e353-7ff5-4560-a3c0-5b9d0e48fb04" />


---

# Observation

The email header was successfully obtained from Gmail and analysed using Mail Header Analyzer.

The MHA analysis displayed the email routing information, Received headers, Return-Path, Message-ID, SPF information, DKIM signatures, and authentication results.

The authentication results were:

```text
SPF   : PASS
DKIM  : PASS
DMARC : PASS
```

The MHA Diagnostics Report also indicated that the `X-Microsoft-Antispam-Mailbox-Delivery` header was missing.

Since SPF, DKIM, and DMARC passed successfully, no obvious evidence of email spoofing was identified from the analysed header.

# Result

**The email header was successfully analysed using Mail Header Analyzer. The Received headers, Message-ID, Return-Path, SPF, DKIM, and DMARC results were examined. SPF, DKIM, and DMARC were found to be PASS, and no obvious evidence of email spoofing was identified.**

# Conclusion

This experiment demonstrated how email headers can be analysed using Mail Header Analyzer to investigate the authenticity and routing of an email.

The experiment showed that SPF, DKIM, and DMARC are important authentication mechanisms for detecting suspicious or spoofed emails. The Received headers, IP addresses, Message-ID, and Return-Path can also provide useful information during email forensic investigations.
