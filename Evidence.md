## Volatile Evidence Collection

Live-response acquisition procedures were performed to preserve volatile system artifacts prior to shutdown or alteration. Memory captures, registry hives, and user-related artifacts were collected and stored within a dedicated forensic evidence directory.

The collected evidence included:

- Physical memory image
- SAM registry hive
- SYSTEM registry hive
- User profile artifacts

This approach ensured preservation of volatile and semi-volatile evidence required for later forensic analysis.

![Collected volatile evidence artifacts](Assets/screenshots/memory-acquisition-artifacts-collected.png)

## Evidence Integrity Validation

Cryptographic hashes were generated for acquired artifacts to verify forensic integrity throughout the collection process. PowerShell scripts were used to compare original and acquired hash values.

Hash comparison results demonstrated that collected artifacts remained unchanged following acquisition and storage.

![PowerShell hash comparison results](Assets/screenshots/powershell-hash-validation-results.png)

## Hash Inventory Review

Generated hash inventories were reviewed using OpenOffice Calc to validate completeness and document artifact-level integrity information. MD5 and SHA-1 hashes were recorded for each acquired artifact to support future verification and chain-of-custody requirements.

![Hash inventory review](Assets/screenshots/hash-list-review-openoffice-calc.png)
