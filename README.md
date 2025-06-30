# Threat Intelligence & YARA Rule Creation

## Program Walkthrough

### Input Collection
- Compiled a list of suspicious file hashes (SHA-256).
- Used public and private samples from known ransomware datasets.

### VirusTotal API Integration
- Wrote a Python script to automate hash lookups using the VirusTotal API.
- Parsed key response fields: detection ratio, threat labels, AV engines, behavior tags.

### Threat Attribution
- Identified one sample as DarkSide Ransomware.
- Linked findings to threat actor FIN7 using threat intelligence sources.
- Referenced MITRE ATT&CK techniques used by DarkSide.

### YARA Rule Development
- Analyzed strings, file structure, and known indicators to draft a YARA rule for DarkSide.
- Included strings found in the binary and used logic conditions for precise detection.

### Testing in Virtual Environment
- Ran the malware sample in a controlled VM (sandbox).
- Scanned with the YARA rule to validate detection.

### Outcome and Reflection
- Successfully created a working threat-hunting workflow.
- Strengthened skills in malware attribution, Python automation, and rule-based detection.

## Tools Used
- Python (requests, JSON handling)
- VirusTotal API
- YARA
- MITRE ATT&CK Framework
- Virtual Machine


Test in VM: Use a virtual machine to test the malware sample and rule.

You can check the Wiki page for a better view of the project


Contributing

Contributions are encouraged! Submit pull requests or issues for enhancements.
