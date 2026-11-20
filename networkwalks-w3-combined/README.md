# Week 3 — Password Cracking Modules (Networkwalks Internship)

This repo documents both Project Modules from Week 3 of the Networkwalks Cybersecurity & Ethical Hacking internship, both centered on recovering the password of the same protected PDF (`My Locked PDF1.pdf`) using two different approaches.

## Modules

### 📁 [Module 1 — Password Cracking with JTR](./module1-jtr)
Cracking the PDF's password locally using **John the Ripper (jumbo)** and its GUI front-end **Johnny**, after extracting a `pdf2john`-compatible hash via an online hash extractor.

### 📁 [Module 2 — Password Cracking with Networkwalks Tools](./module2-networkwalks-tools)
Cracking the same PDF's password using **Networkwalks' own browser-based Hash Calculator and Password Cracker** tools — no local install required. Includes the retry needed after the built-in 100-word list failed, succeeding once a larger wordlist was loaded.

## Result

Both modules independently recovered the same password and captured the same flag:

```
Password: good-luck
Flag: nw{cybersecurity_flag_captured_2608}
```

## Key Takeaway

Whether using a locally installed cracking tool (JTR) or a browser-based equivalent, the underlying technique is the same: extract a crackable hash from the protected file, then run a wordlist/dictionary attack against it. Module 2 also highlighted how much cracking success depends on wordlist coverage — a small default list isn't always enough.

---
*Part of the [Networkwalks](https://www.networkwalks.com) Cybersecurity & Ethical Hacking internship program.*
