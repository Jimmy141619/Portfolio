# A4: Discover a Vulnerable Website (OWASP Juice Shop)

## **Overview**

This activity explores vulnerabilities in OWASP Juice Shop, a deliberately insecure web application designed for cybersecurity training. The platform simulates real-world web application flaws in a safe and controlled environment.

---

## Vulnerability Identified: SQL Injection

* The login functionality is vulnerable to SQL injection attacks.

**Description:**

* SQL injection occurs when user input is not properly validated or sanitized, allowing attackers to manipulate backend database queries.

* This vulnerability is part of the **OWASP Top 10 (Injection category)**, one of the most critical web security risks.

---

## Example Attack

* Example input used in the login field:

  ```
  ' OR 1=1 --
  ```

**Result:**

* The application bypasses authentication and grants access without valid credentials.

---

## Security Impact

* Unauthorized access to user accounts
* Exposure or modification of sensitive data
* Potential full database compromise

---

## Why This Vulnerability Exists

* The application constructs SQL queries using unsanitized user input
* Lack of input validation and secure query handling

---

## Mitigation Strategies

* Use parameterized queries (prepared statements)
* Implement proper input validation and sanitization
* Apply secure authentication mechanisms

---

## Ethical Consideration

* This activity was conducted using OWASP Juice Shop, a purposely vulnerable application designed for learning
* No real systems were targeted or exploited

---

## Conclusion

SQL injection is a critical vulnerability that can lead to complete system compromise. This example highlights the importance of secure coding practices and input validation in modern web applications.
