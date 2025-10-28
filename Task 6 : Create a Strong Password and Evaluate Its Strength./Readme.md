# Passwords Chosen for the Task5

**Purpose:** These are the passwords I have chosen to complete the password-security task. This README lists the chosen passwords, a short evaluation of each, safe-handling guidance, and best-practice tips learned from the evaluation.

---

## Chosen Passwords
1. `qwerty`  
2. `MyHouse89`  
3. `Pa$$word!`  
4. `C@tH0use89!`  
5. `Blue$Mountain!River47`

---

## Short Evaluation (security summary)
- `qwerty` — **Very Weak.** Most commonly Used Passwords ; vulnerable to dictionary attacks and credential stuffing. Do not use for any real account.  
- `MyHouse89` — **Weak to Moderate.** Uses mixed case and numbers but contains a dictionary word and a likely personal-style pattern. Vulnerable to targeted guessing if an attacker knows personal details.  
- `Pa$$word!` — **Weak.**  common used Passwords, predictable substitutions (e -> $), which many cracking tools and lists already include. Offers little real protection.  
- `C@tH0use89!` — **Strong.** Mixed case, numbers, and symbols; less predictable than dictionary words. Shorter than ideal but reasonably strong if unique and not reused.  
- `Blue$Mountain!River47` — **Very Strong (passphrase).** Long, uses multiple unrelated words plus symbols and numbers. High entropy and easier to remember than equivalent-length random strings.  

---

## Best-Practice Guidance & Tips
- **Prefer length and randomness.** A long passphrase (3–5 unrelated words + symbols/numbers) is both strong and memorable.  
- **Use unique passwords for each site.** Reusing passwords risks credential stuffing after a breach.  
- **Avoid dictionary words or personal data.** Attackers often try names, locations, birth years, and common phrases.  
- **Avoid predictable substitutions.** Replacing `a` with `@` or `s` with `$` is common and appears in many wordlists used by attackers.  
- **Use a reputable password manager.** Let the manager generate and store long random passwords so you don’t have to remember them.  
- **Enable multi-factor authentication (MFA)** wherever possible — it greatly reduces account takeover risk, even if the password is compromised.  
- **Rotate/change passwords** when a service you use has a confirmed breach. Use the service’s notifications or check haveibeenpwned.com (or equivalent) for breaches.  

---

## Handling and Storage (safety warning)
- **Do not store these passwords in plaintext** on shared systems, public repos, or unsecured notes. If this file is being used as a lab artifact, mark it as a demonstration only and avoid real credentials.  
- If you must keep a record for testing, store it in an encrypted vault or in a password manager’s secure notes.  

---
## Brute Force Attack
A brute force attack is when an attacker tries every possible combination of letters, numbers, and symbols until the correct password is found.  
It’s like guessing every key on a keychain until one opens a lock.

- **Example:** Trying passwords like `a`, `aa`, `aaa`, `aaaa`... until it works.  
- **Weak passwords** (short or simple ones) can be cracked very fast.  
- **Strong passwords** (long with uppercase, lowercase, numbers, and symbols) take much longer to break.

**How to protect yourself:**
- Use long and complex passwords.
- Enable account lockouts or two-factor authentication (MFA).
- Avoid short or simple passwords.

---

## Dictionary Attack
A dictionary attack uses a list of common passwords or words found in the dictionary to guess passwords.  
Attackers know many people use easy or common passwords like `password`, `123456`, or `qwerty`.

- **Example:** Trying passwords from a list such as `password`, `Pa$$word`, `123456`, `welcome`.  
- It’s faster than brute force because it focuses on likely choices first.  

**How to protect yourself:**
- Avoid using real words or common passwords.
- Use a mix of random words, numbers, and symbols.
- Try a passphrase (example: `Blue$Mountain!River47`).

---

## Summary
- **Brute Force:** Tries every possible combination. Defend with long, complex passwords.  
- **Dictionary:** Tries common words and known passwords. Defend by avoiding simple or common words.  

**Tip:**  
The best defense is to use long, unique, and random passwords and turn on multi-factor authentication for extra security.


*This README was generated to summarize the passwords you selected and to provide concise guidance on their strengths and safe handling.*


