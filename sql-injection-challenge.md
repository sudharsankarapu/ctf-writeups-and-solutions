# SQL Injection Challenge

## Challenge Description
The target application has a login form vulnerable to SQL injection. The goal is to bypass authentication and retrieve user information.

---

## Steps to Solve
1. **Identify the Vulnerability:**  
   - Entered `' OR '1'='1` in the username field and observed a successful login.  
   - The application does not sanitize user input.

2. **Extract Data:**  
   - Used the payload: `' UNION SELECT null, username, password FROM users--`  
   - Retrieved all usernames and passwords.

---

## Lessons Learned
- Always validate and sanitize user inputs to prevent SQL injection.
- Use prepared statements to handle dynamic queries.

---
