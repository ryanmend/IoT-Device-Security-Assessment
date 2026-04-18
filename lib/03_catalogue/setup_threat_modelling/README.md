The following is the list of items required during the assessment:

`Status` column can be set for values similar to "Pass", "Fail", "N/A".

`Severity` column can be set for values "0-10" or "N/A" with 0 as the lowest to 10 being the highest potential magnitude of harm or damage if a risk event occurs (how bad). Refer to the [2.3. Validation Framework](./lib/02_framework/framework.md) for specific CVSS rating.

## 3.1 Setup & Threat Modelling
| Test ID | Phase / Test Name | Status | Severity | Notes / Evidence |
| :--- | :--- | :--- | :--- | :--- |
| IDSA-SETUP-01 | Device Selection & Inventory (FR1, FR2) | | | Record device specs, hardware version, and identify exposed boot logs or hardware implementation details. |
| IDSA-MODEL-01 | IoT Threat Model (FR4, FR5) | | | Map all identified attack vectors (USB, Wi-Fi, Cloud API, Physical) to the threat model. |
| IDSA-MODEL-02 | Visual Threat Diagram (FR6) | | | Confirm diagram shows all attack surfaces including RPi, Blink App, and Cloud Endpoints. |
| IDSA-MODEL-03 | Threat Impact Rating (FR7) | | | Assign likelihood/impact scores to identified threats based on technical exploitability. |
