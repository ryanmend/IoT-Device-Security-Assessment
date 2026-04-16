The following is the list of items required during the assessment:

`Status` column can be set for values similar to "Pass", "Fail", "N/A".

`Severity` column can be set for values "0-10" or "N/A" with 0 as the lowest to 10 being the highest potential magnitude of harm or damage if a risk event occurs (how bad). Refer to the [2.3. Testing Methodology](./src/02_framework/methodology.md) for specific CVSS rating.

## 3.5 Correlation & Risk Evaluation
| Test ID | Phase / Test Name | Status | Severity | Notes / Evidence |
| :--- | :--- | :--- | :--- | :--- |
| IDSA-CORR-01 | Vulnerability Correlation (FR25, FR26) | | | Cross-reference network findings (e.g., open ports) with firmware findings (e.g., outdated packages). |
| IDSA-RISK-01 | Risk Matrix & Severity (FR27, FR28) | | | Map all identified vulnerabilities (BOLA, Hardcoded Keys, etc.) to a risk matrix. |
| IDSA-MITIG-01 | Mitigation Recommendations (FR29) | | | Develop NIST and FIRST (CVSS) fix strategies for all identified risks. |
