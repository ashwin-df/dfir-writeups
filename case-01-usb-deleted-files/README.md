# USB Deleted Files Analysis – Case 01

## Overview
- This case focuses on recovering deleted files from a USB storage device.

## Objective
- To analyze the USB device and attempt recovery of deleted data.

## Tools Used
- PhotoRec

## Methodology
- Initial files were copied to the USB device inside a DFIR_PRACTICE directory. 
- Selected test files (images, PDF, and text files) were permanently deleted using the rm command in Linux.
- The USB device was safely ejected after deletion to prevent data overwriting.
- A full disk forensic image of the USB device (/dev/sdc) was created using the dd utility.
- SHA-256 hash values were calculated for both the original device and the acquired image.
- The hash values of the source device and the acquired image were compared and found to be identical, confirming acquisition integrity.
- All analysis and recovery were performed on the image file to preserve the original evidence.

## Findings
- PhotoRec recovered all deleted files of selected types (JPG, PNG, PDF) from the forensic image.
- Recovered files:
    - photo_trip_01.jpg
    - photo_trip_02.jpg
    - bank_statement_2025.pdf
- Only the files intentionally deleted for this practice were included in the analysis.
- Screenshots of recovered files are included in the `screenshots/` folder.
- Total recovered files: 9992 (includes junk files), but analysis focused on the relevant images and PDFs.

## Conclusion
- PhotoRec successfully recovered the intentionally deleted files (JPG and PDF) from the forensic image.
- The exercise demonstrates key DFIR workflows, including evidence acquisition, integrity verification, recovery, and documentation.
- Recovered files were organized in a dedicated folder to simulate real-world evidence handling practices.
- Screenshots provide visual proof of the recovered files without exposing private or irrelevant data. 
