#  LanaICms - Reflected XSS Vulnerability

## 📄 Summary
A **Reflected Cross-Site Scripting (XSS)** vulnerability was identified in a specific endpoint of **LanaICms**.  
This vulnerability allows attackers to inject malicious JavaScript, which can be used to **redirect users to attacker-controlled websites**.

---

##  Impact
Successful exploitation of this vulnerability may allow an attacker to:
- Execute arbitrary JavaScript in the victim's browser  
- Redirect users to malicious websites  
- Potentially steal sensitive information (e.g., session cookies)

---

##  Proof of Concept (PoC)
```bash
https://www.lanaicms.com/module.php?modname=%3Cscript%3Edocument.location=%22https://google.com%22%3C/script%3E&mf=install
