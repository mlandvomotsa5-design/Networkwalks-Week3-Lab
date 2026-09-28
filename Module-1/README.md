# Module 1: Local Password Cracking with John the Ripper (CLI)

## Objective
Extract the internal encryption hash from `My Locked PDF1.pdf` and perform an offline dictionary attack using John the Ripper (`john.exe`) via Windows Command Prompt.

## Files & Evidence
* `hash1.txt` – The extracted raw PDF encryption hash starting with `$pdf$...`.
* `Screenshot1_Attack_Execution.png` – Command Prompt window running `john.exe hash1.txt` showing loaded hash.
* `Screenshot2_Cracked_Password.png` – Command Prompt window running `john.exe --show hash1.txt` displaying the recovered plain-text password.
* `Screenshot3_Unlocked_PDF.png` – The target PDF document opened and unlocked on screen.

## Execution Summary
1. Extracted hash to `hash1.txt`.
2. Executed `john.exe hash1.txt` using the default dictionary (`password.lst`).
3. Verified recovered credentials and unlocked the document.
