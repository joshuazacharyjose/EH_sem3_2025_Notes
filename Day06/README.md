# The OWASP Top 10 Security Risks

The OWASP Top 10 is a standard awareness document for developers and web application security professionals. It represents a broad consensus within the security community about the most critical risks that modern web applications face. By highlighting the top categories of vulnerabilities, it serves as both an educational resource and a practical guide for organizations to prioritize their security efforts. Developers, architects, and security teams use it as a baseline for building more secure applications and for evaluating existing systems against common attack vectors.

## 1. **A01:2021 – Broken Access Control**
- Weak or missing restrictions allow users to act outside their permissions.
- Example: a regular user accessing admin functions.

## 2. **A02:2021 – Cryptographic Failures**
- Poor handling of sensitive data (no encryption, weak algorithms, misconfigured TLS).
- Example: passwords stored in plain text.

## 3. **A03:2021 – Injection**
- Untrusted data is sent to an interpreter (SQL, NoSQL, OS, LDAP).
- Example: SQL injection with `'; DROP TABLE users;--`.

## 4. **A04:2021 – Insecure Design**
- Fundamental flaws in architecture or logic, not just coding mistakes.
- Example: relying solely on client-side validation for security.

## 5. **A05:2021 – Security Misconfiguration**
- Default accounts, unnecessary services, misconfigured HTTP headers, or verbose error messages.
- Example: leaving admin panels publicly accessible. 

## 6. **A06:2021 – Vulnerable and Outdated Components**
- Using old libraries, frameworks, or software with known vulnerabilities.
- Example: running an outdated CMS plugin with a public exploit.

## 7. **A07:2021 – Identification and Authentication Failures**
- Weak authentication systems, poor session management, or missing MFA.
- Example: predictable session IDs or brute-forceable logins.

## 8. **A08:2021 – Software and Data Integrity Failures**
- Code and infrastructure not protected against integrity attacks.
- Example: using insecure CI/CD pipelines or trusting unsigned updates.

## 9. **A09:2021 – Security Logging and Monitoring Failures**
- Lack of detection, alerting, or monitoring for suspicious activities.
- Example: attackers go unnoticed because login failures aren’t logged.

## 10. **A10:2021 – Server-Side Request Forgery (SSRF)**
- Application fetches remote resources without validating user input.
- Example: attacker tricks the server into making requests to internal services (e.g., AWS metadata endpoint).

<hr>

### OWASP Top 10 (2021) – Cheat Sheet

| #  | Risk                                         | Quick Summary                                                                  |
|----|----------------------------------------------|--------------------------------------------------------------------------------|
| 1  | **Broken Access Control**                    | Users can access things they shouldn’t (e.g., privilege escalation).           |
| 2  | **Cryptographic Failures**                   | Sensitive data isn’t protected properly (weak/no encryption, bad TLS).         |
| 3  | **Injection**                                | Untrusted input breaks queries/commands (SQLi, OS command injection, etc.).    |
| 4  | **Insecure Design**                          | Flaws in system design/logic; security not built into the architecture.        |
| 5  | **Security Misconfiguration**                | Defaults, unnecessary features, or poor configuration expose the system.       |
| 6  | **Vulnerable & Outdated Components**         | Using old/unpatched libraries, frameworks, or software.                        |
| 7  | **Identification & Authentication Failures** | Weak login/session handling (no MFA, predictable tokens).                      |
| 8  | **Software & Data Integrity Failures**       | Trusting unverified code, updates, or CI/CD pipelines.                         |
| 9  | **Security Logging & Monitoring Failures**   | Attacks go undetected due to missing/incomplete logging.                       |
| 10 | **Server-Side Request Forgery (SSRF)**       | App fetches attacker-controlled URLs, leading to internal access.              |
