# W3-PM2 — Password Cracking with NetworkWalks Tools

**NetworkWalks Cybersecurity & Ethical Hacking Internship — Week 3**

**Intern:** Litik Aswani  
**Module:** W3-PM2  
**Status:** Completed

---

## Objective

Recover the password of the supplied password-protected PDF using the NetworkWalks Hash Calculator and Password Cracker.

The objective was to understand how PDF password hashes can be extracted and tested using browser-based cybersecurity tools.

## Tools Used

- NetworkWalks Hash Calculator
- NetworkWalks Password Cracker
- Web Browser
- Windows 11
- Kali Linux (VirtualBox)
- VirtualBox Shared Folders

## Lab Procedure

### Step 1 — Prepare the Protected PDF

Extracted the lab file:

`My Locked PDF1 (for NW Tools Lab WK3-PM2).pdf`

The file was placed in the `Week3/PM2` directory inside the shared Downloads folder.

### Step 2 — Open NetworkWalks Hash Calculator

Accessed the NetworkWalks Hash Calculator:

https://networkwalks.com/hash-calculator/

Selected the **PDF** tab to access the PDF password hash extraction functionality.

### Step 3 — Extract PDF Hash

1. Selected the protected PDF file.
2. Loaded the file into the PDF Hash Calculator.
3. Confirmed successful hash extraction.
4. Copied the extracted hash beginning with `$pdf$`.

The tool identified the following PDF encryption properties:

| Property | Value |
|---|---|
| PDF Revision | R4 |
| PDF Version | V4 |
| Encryption Key Length | 128-bit |
| Hash Format | `$pdf$` |
| Hash Extraction | Successful |

### Step 4 — Open NetworkWalks Password Cracker

Accessed the NetworkWalks Password Cracker:

https://networkwalks.com/password-cracker/

The tool provides a browser-based interface for testing password candidates against supported hashes.

### Step 5 — Configure Dictionary Attack

1. Pasted the extracted PDF hash into the password hash field.
2. Selected the dictionary attack method.
3. Chose the built-in wordlist containing 100 candidate passwords.
4. Verified that the hash had been entered correctly.
5. Started the password recovery process.

### Step 6 — Recover Password

The Password Cracker tested candidate passwords from the selected dictionary.

The tool successfully identified the matching password.

**Result:** Password cracked successfully using the built-in dictionary.

### Step 7 — Verify Recovered Password

Opened the supplied encrypted PDF using the recovered password.

The PDF opened successfully and displayed the NetworkWalks completion page, including the first lab flag.

This confirmed that the recovered password was valid.

## Results

| Test | Result |
|---|---|
| Protected PDF extraction | Successful |
| PDF hash extraction | Successful |
| Encryption information identification | Successful |
| Dictionary attack configuration | Successful |
| Password recovery | Successful |
| PDF unlock verification | Successful |
| First lab flag displayed | Successful |

**Final Status: Completed Successfully**

## Evidence

| File | Description |
|---|---|
| `PM2_01_Hash_Extracted.png` | Hash Calculator displaying the extracted PDF hash |
| `PM2_02_Password_Cracked.png` | Password Cracker showing successful password recovery |
| `PM2_03_PDF_Unlocked_Flag1.png` | Unlocked PDF displaying the first lab flag |

Evidence screenshots are stored in the `screenshots/` directory.

## Learning Outcomes

- Learned how to extract PDF password hashes using browser-based tools.
- Understood the relationship between password-protected files and password verification data.
- Practiced dictionary-based password recovery.
- Gained experience using the NetworkWalks Hash Calculator and Password Cracker.
- Identified basic PDF encryption properties.
- Verified a recovered password by unlocking the encrypted file.
- Understood the security risks associated with predictable passwords.

## Security Observations

The built-in dictionary attack successfully recovered the password of the training PDF.

This demonstrates that passwords included in common password lists may be vulnerable to dictionary-based recovery attempts.

The exercise emphasizes the importance of strong, unique passwords and avoiding easily predictable credentials.

## Conclusion

Successfully completed the Week 3 PM2 exercise using the NetworkWalks Hash Calculator and Password Cracker.

The module provided practical experience in PDF hash extraction, dictionary attacks, and password recovery using browser-based cybersecurity tools.

The recovered password was verified by successfully opening the supplied protected PDF and accessing its contents.

## Disclaimer

This exercise was completed using an authorized training PDF supplied as part of the NetworkWalks Cybersecurity & Ethical Hacking Internship.

The tools and procedures documented here are intended solely for educational purposes and authorized cybersecurity testing.

---

**Organization:** NetworkWalks Academy  
**Website:** https://networkwalks.com/
