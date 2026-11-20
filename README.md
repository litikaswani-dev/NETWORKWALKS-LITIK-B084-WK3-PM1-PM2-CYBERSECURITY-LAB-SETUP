# NetworkWalks Cybersecurity Internship — Week 3

## Password Cracking & Hash Analysis Labs

**Intern:** Litik Aswani  
**Organization:** NetworkWalks Academy  
**Program:** Cybersecurity & Ethical Hacking Internship  
**Week:** 3  
**Environment:** Kali Linux (VirtualBox), Windows 11

---

## Project Overview

During Week 3 of my NetworkWalks Cybersecurity & Ethical Hacking Internship, I completed two compulsory practical modules focused on password cracking, hash extraction, and password security.

The exercises involved recovering passwords from encrypted PDF files using John the Ripper, Johnny GUI, and NetworkWalks' browser-based cybersecurity tools.

Both labs were performed using the password-protected practice files supplied for the internship.

## Completed Modules

| Module | Description | Status |
|---|---|---|
| W3-PM1 | Password Cracking with John the Ripper and Johnny GUI | Completed |
| W3-PM2 | Password Cracking with NetworkWalks Tools | Completed |

## Tools and Technologies

- **Kali Linux:** Linux environment for cybersecurity exercises.
- **VirtualBox:** Virtualization platform used to run Kali Linux.
- **John the Ripper:** Password auditing and recovery tool.
- **pdf2john:** Utility for extracting password hashes from encrypted PDF files.
- **Johnny GUI:** Graphical interface for John the Ripper.
- **NetworkWalks Hash Calculator:** Browser-based tool for extracting PDF password hashes.
- **NetworkWalks Password Cracker:** Browser-based dictionary attack tool.
- **Git and GitHub:** Documentation and evidence management.

---

## Module 1 — Password Cracking with John the Ripper

### Objective

Recover the password of the provided `My Locked PDF1.pdf` file using John the Ripper and demonstrate the recovered result through Johnny GUI.

### Procedure

1. Verified that John the Ripper was installed in Kali Linux.
2. Installed and launched Johnny GUI.
3. Extracted the supplied password-protected PDF.
4. Used `pdf2john` to extract the PDF password hash.
5. Saved the extracted hash in a text file.
6. Used John the Ripper to perform password recovery.
7. Displayed the successfully recovered password.
8. Loaded the hash into Johnny GUI to verify the recovery result.
9. Opened the protected PDF using the recovered password.
10. Captured screenshots documenting the successful exercise.

### Commands Used

**Check John the Ripper installation:**

```bash
john --list=build-info
```

**Install Johnny GUI:**

```bash
sudo apt install johnny
```

**Extract the PDF hash:**

```bash
pdf2john "My Locked PDF1.pdf" > pdf_hash.txt
```

**Start password recovery:**

```bash
john pdf_hash.txt
```

**Display the recovered result:**

```bash
john --show pdf_hash.txt
```

### Results

- Successfully extracted the password hash from the encrypted PDF.
- Recovered the PDF password using John the Ripper.
- Confirmed the recovered result using Johnny GUI.
- Verified that the protected PDF could be opened.
- John the Ripper reported one successfully cracked hash with zero remaining.

**Status: Successfully completed.**

### Evidence

| Screenshot | Description |
|---|---|
| PM1_01_John_Password_Cracked.png | Successful password recovery in the Kali terminal |
| PM1_02_PDF_Unlocked.png | Protected PDF opened successfully |
| PM1_03_Johnny_GUI_Cracked.png | Johnny GUI displaying the recovered result |

---

## Module 2 — Password Cracking with NetworkWalks Tools

### Objective

Recover the password of the supplied protected PDF using the NetworkWalks Hash Calculator and Password Cracker tools.

### Procedure

1. Extracted the PDF specifically supplied for the Week 3 PM2 lab.
2. Opened the NetworkWalks Hash Calculator.
3. Selected the PDF hash extraction feature.
4. Loaded the password-protected PDF.
5. Extracted its password hash in `$pdf$` format.
6. Copied the extracted hash.
7. Opened the NetworkWalks Password Cracker.
8. Pasted the hash into the input field.
9. Selected the built-in dictionary containing 100 candidate passwords.
10. Started the dictionary attack.
11. Successfully recovered the PDF password.
12. Opened the protected PDF and captured the first flag.
13. Saved evidence of the recovery and verification process.

### Tools Used

**NetworkWalks Hash Calculator:**  
https://networkwalks.com/hash-calculator/

**NetworkWalks Password Cracker:**  
https://networkwalks.com/password-cracker/

### Results

- Successfully extracted an encrypted PDF password hash.
- Identified PDF Revision R4, Version V4, with 128-bit encryption.
- Completed the dictionary attack using the tool's built-in wordlist.
- Successfully recovered the password.
- Verified that the recovered password opened the PDF.
- Captured the first flag displayed in the unlocked document.

**Status: Successfully completed.**

### Evidence

| Screenshot | Description |
|---|---|
| PM2_01_Hash_Extracted.png | NetworkWalks Hash Calculator displaying the extracted hash |
| PM2_02_Password_Cracked.png | Password Cracker displaying the successful dictionary attack |
| PM2_03_PDF_Unlocked_Flag1.png | Successfully unlocked PDF displaying the first flag |

---

## Repository Structure

```text
NETWORKWALKS-WEEK3-CYBERSECURITY-LABS/
│
├── README.md
│
├── W3-PM1-John-the-Ripper/
│   ├── README.md
│   └── screenshots/
│       ├── PM1_01_John_Password_Cracked.png
│       ├── PM1_02_PDF_Unlocked.png
│       └── PM1_03_Johnny_GUI_Cracked.png
│
└── W3-PM2-NetworkWalks-Tools/
    ├── README.md
    └── screenshots/
        ├── PM2_01_Hash_Extracted.png
        ├── PM2_02_Password_Cracked.png
        └── PM2_03_PDF_Unlocked_Flag1.png
```

## Key Learning Outcomes

Through these exercises, I gained practical experience in:

1. Understanding password hashes and their role in password-protected files.
2. Extracting PDF password hashes using command-line and browser-based tools.
3. Performing dictionary attacks to evaluate password strength.
4. Using John the Ripper for password recovery.
5. Understanding the purpose and operation of Johnny GUI.
6. Comparing command-line and browser-based password recovery workflows.
7. Verifying successful password recovery by opening encrypted files.
8. Documenting cybersecurity lab procedures and collecting technical evidence.

## Security Observations

These exercises demonstrated that passwords present in common wordlists can be vulnerable to dictionary attacks.

The labs reinforced the importance of using strong, unique passwords, avoiding predictable credentials, and understanding how password complexity affects resistance to recovery attempts.

They also demonstrated the value of cybersecurity tools in authorized password auditing and security education.

## Conclusion

Week 3 of the NetworkWalks Cybersecurity & Ethical Hacking Internship provided practical exposure to password recovery and hash analysis.

Both compulsory project modules were completed successfully using the supplied training materials.

The exercises strengthened my understanding of password-based security, dictionary attacks, cybersecurity tools, and technical documentation.

## Disclaimer

All password recovery exercises were performed as part of an authorized educational cybersecurity internship using supplied lab files.

The techniques demonstrated in this repository are intended strictly for ethical hacking education, password security assessment, and authorized security testing.

## Acknowledgments

Special thanks to **NetworkWalks Academy** and the internship instructors for providing the resources, lab exercises, and practical cybersecurity learning opportunities.

**NetworkWalks Academy:** https://networkwalks.com/
