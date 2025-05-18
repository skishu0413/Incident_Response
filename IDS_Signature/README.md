# 🛡️ IDS Signature Development (Suricata Rules)

## 📌 Overview

This project focuses on developing intrusion detection system (IDS) signatures using the Suricata rule language. You are provided with various network threat scenarios, and your goal is to create Suricata rules that correctly detect these threats.

## 🧑‍💻 Project Details

- **Type:** Individual Assignment  
- **Platform:** Suricata IDS  
- **Testing Tool:** [Signature Testing API](https://mzfrri3b1j.execute-api.us-east-1.amazonaws.com/)  
- **Documentation:** [Suricata Rule Language (v6.0.4)](https://suricata.readthedocs.io/en/suricata-6.0.4/)

## 📝 Assignment

Write Suricata signatures for the following threat scenarios. Each rule must use the **item number as the SID** and assume the following predefined variables are available:

- `HOME_NET`
- `EXTERNAL_NET`
- `HTTP_PORTS`

No other variables are defined.

### 🔧 Scenarios

1. **Suspicious IP Targeting Web Services**  
   Alert on HTTP traffic from IP `27.43.100.29` to any local web server.

2. **phpMyAdmin Scan with No User-Agent**  
   Alert when an external IP attempts to access `/phpMyAdmin/scripts/setup.php` **without** a User-Agent header.

   - **Test File:** [`http.pcap`](#)

3. **OAuth2 Phishing Link in Email**  
   Alert on emails containing the link `https://accounts.google.com/o/oauth2/auth`.

   - **Test File:** [`smtp.pcap`](#)

4. **[Extra Credit] Yahoo Messenger Friends List Detection**  
   Identify Yahoo Messenger packets using the undocumented service code `00 f1`.

   - **Protocol Spec:** [YMSG-9 Protocol](http://libyahoo2.sourceforge.net/ymsg-9.txt)  
   - **Test File:** [`ymsg2.pcap`](#)


## 🧪 Testing Your Rules

Test your rules using the public Suricata testing site:

🔗 https://mzfrri3b1j.execute-api.us-east-1.amazonaws.com/

> Note: If the test page shows a timeout, refresh it after a few seconds due to AWS caching.

## 📘 Suricata Rule Guidelines

- Focus on sections **6.1 to 6.7** of the [Suricata documentation](https://suricata.readthedocs.io/en/suricata-6.0.4/)
- Include content matches, header checks, protocol identifiers, and correct sid/rev values
- Avoid overlapping rule conditions that might suppress other alerts

---

## 🧠 Lessons From the Project

This project strengthens the ability to:
- Write customized Suricata signatures for real-world threats
- Understand and utilize HTTP, email, and proprietary protocol structures
- Evaluate the effectiveness of rules through testing tools and PCAPs

---

> *All provided data and traffic samples are fictional and intended for educational purposes only.*
