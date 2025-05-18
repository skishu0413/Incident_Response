# 🕵️‍♂️ Project 3: Second Compromise Report (Phishing Investigation)

## 📌 Overview

This project simulates a suspected phishing incident within the **North American Lumber Coalition (NALC)**. As a member of the NALC Security Operations Center (SOC), you are tasked with investigating a suspicious email reported by an employee, determining the scope of the compromise, and providing detailed documentation of your findings.

## 🧑‍💻 Project Details

- **Type:** Individual Assignment  
- **Platform Used:** Splunk (or other log analysis tools)  
- **Dataset Provided:** HTTP metadata log, Mail log, NALC IT user inventory

## 📥 Background

A user reported receiving the following suspicious email:

```
From: Jason Robinson <jrobinson@northamericanlumbercoalition.com>
To: Stephanie Morgan <smorgan@northamericanlumbercoalition.com>

You have one (1) new message
Click here <http://srv-61.kim.johnson.biz/login>
```

Your role is to:
- Analyze mail and HTTP logs
- Trace any potential compromise
- Determine attacker behavior and timing
- Document the findings in a professional format

## 📝 Deliverables

This project requires submission of **two documents**:

### 1. Incident Report
Structured using the provided template, including:
- **Executive Summary:** High-level summary of the incident and impact  
- **Timeline:** Detailed chronology of the attack and response  
- **Containment & Eradication:** Hypothetical steps taken to stop and clean the attack  
- **Financial Impact:** Estimated cost of investigation and potential losses  
- **Lessons Learned:** How to improve defenses and prevent recurrence  
- **Report Format:** Adheres to executive/business audience expectations

### 2. Investigation Log
A chronological log of your steps, queries, decisions, and findings while investigating the incident. Must follow guidance from Lesson 10.

## 🔍 Tools & Resources

- **Primary Tool:** Splunk (https://splunk.class.security.gatech.edu)
  - Use VPN and GT credentials
  - Navigate to "Search and Reporting"
  - Relevant Indexes:
    - `p3-http` — HTTP metadata
    - `p3-mail` — Mail logs
- **Alternate Tools:** ELK, grep, or other log parsers (not recommended for scale)
- **Files Provided:**
  - `http.log`
  - `mail.log`
  - `inventory.csv`


## 🧠 Lessons From the Project

This project strengthened skills in:
- Detecting phishing campaigns via log forensics
- Building a timeline of compromise using mail and HTTP data
- Writing executive-level incident reports
- Maintaining detailed investigative documentation

---

> *Note: All data, names, and estimated financial values in this project are fictional and used solely for academic purposes.*
