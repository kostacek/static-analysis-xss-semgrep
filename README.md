# Preventing Injection Attacks: Vulnerability Assessment & Mitigation

This project analyzes and remediates multiple injection vulnerabilities in a penetration‑testing training application. It includes proof‑of‑concept exploits, vulnerable code samples, secure coding fixes, and screenshots demonstrating successful mitigation.

The work aligns with OWASP recommendations and demonstrates practical secure‑coding, vulnerability analysis, and remediation skills.

---

## 📌 Project Objectives

1. Identify and exploit injection vulnerabilities in a Java/Spring application  
2. Document each vulnerability with screenshots and proof‑of‑concept payloads  
3. Apply secure‑coding fixes aligned with OWASP guidance  
4. Validate that each vulnerability is fully mitigated  

---

# 🧨 1. SQL Injection

### ✔ Vulnerability  
User input was concatenated directly into SQL queries:

```java
String queryString = "SELECT * FROM Employees WHERE username = " 
    + employee_username + " AND password = " + employee_password;
