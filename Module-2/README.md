# Module 2: Password Cracking with Networkwalks Web Tools & Technical Pivot

## Objective
Attempt password cracking using the web-based Networkwalks Hash Calculator and Password Cracker tools, analyze wordlist constraints, and perform a technical fallback if needed.

## Files & Evidence
* `hash1_extracted.txt` – The extracted PDF hash submitted to the web tool.
* `Screenshot1_WebTool_AccessDenied.png` – Networkwalks Password Cracker displaying `ACCESS DENIED: Not cracked with this wordlist`.
* `Screenshot2_LocalPivot_JTR.png` – Command Prompt showing local fallback cracking via John the Ripper (`john.exe --show hash1.txt`).
* `Screenshot3_Unlocked_PDF.png` – Target PDF file opened and readable.
* `Unlocked #5.jpg` – Captured completion flag (`nw{cybersecurity_flag_captured_2608}`).

## Execution Summary
1. Extracted the `$pdf$...` hash string and submitted it to the Networkwalks online Password Cracker.
2. Observed web tool failure due to default wordlist limitations (`ACCESS DENIED`).
3. Pivoted back to local CLI cracking using JTR's expanded wordlist (`password.lst`) to successfully recover the password and capture the flag.
