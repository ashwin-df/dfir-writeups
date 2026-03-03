# DFIR Writeups

This repository contains structured digital forensics and incident response (DFIR) practice cases. Each case demonstrates proper evidence handling, forensic imaging, data recovery, and documentation workflows.

## Repository Structure

- **case-01-usb-deleted-files/** – Deleted files recovery from a USB device. Contains:
  - `evidence/` – Recovered test files analyzed for this case.
  - `screenshots/` – Visual proof of recovered files and folder structure.
  - `README.md` – Case-specific report detailing methodology, findings, and conclusion.

Future cases will follow the same organized structure to maintain clarity and consistency.

## Methodology Highlights (Applicable Across Cases)

- Evidence acquisition via full disk or partition imaging using `dd`.  
- Hashing of source devices and images to verify integrity (SHA-256).  
- Recovery performed on forensic images to preserve original evidence.  
- Analysis focused on selected file types to simulate realistic DFIR workflow.  
- Screenshots provided to document evidence handling and recovery.

## Contribution / Practice Notes

- This repository is intended for **practice and learning purposes only**.  
- Only test files are included; personal or sensitive data is excluded.  
- Each case is self-contained and demonstrates a full DFIR workflow from acquisition to reporting.
