# john-the-ripper
Password Cracking through john the ripper
# Password Security & Authentication Analysis

## Overview
This project is part of a Cyber Security Internship task focused on understanding how passwords are stored, attacked, and protected.  
The objective was to analyze password hashing mechanisms, perform controlled cracking of weak passwords, and study authentication defenses such as MFA.

---

## Objectives
- Understand how passwords are stored using hashing
- Identify common hash types (MD5, SHA1)
- Generate password hashes
- Crack weak password hashes using dictionary attacks
- Analyze why weak passwords fail
- Study the importance of Multi-Factor Authentication (MFA)
- Document best practices for strong authentication

---

## Tools Used
- **John the Ripper** – password cracking
- **Linux command-line utilities**
- **RockYou wordlist**

---

## Methodology
1. Generated a weak password hash using MD5.
2. Stored the hash in a file for analysis.
3. Used John the Ripper with a dictionary attack (RockYou wordlist) to crack the hash.
4. Verified the cracked password using John’s `--show` option.
5. Analyzed the results and documented security implications.

---

## Result
- The password `password123` was cracked instantly.
- This demonstrates that:
  - Weak passwords are trivial to break
  - MD5 is insecure for password storage
  - Dictionary attacks are highly effective against common passwords

---

## Key Learnings
- Hashing is a one-way function and differs from encryption.
- Fast hash algorithms like MD5 are unsuitable for password storage.
- Dictionary attacks are faster and more practical than brute-force attacks for weak passwords.
- Strong password policies, slow hashing algorithms (bcrypt/Argon2), and MFA significantly improve security.

---

## Recommendations
- Use strong, unique passwords (12+ characters).
- Avoid outdated hash algorithms like MD5 and SHA1.
- Implement bcrypt or Argon2 for password hashing.
- Enable Multi-Factor Authentication (MFA).
- Apply rate limiting and monitor failed login attempts.

---

## Disclaimer
All activities were performed in a controlled environment for educational purposes only. No unauthorized systems were targeted.

---

## Author
Bishal Das
