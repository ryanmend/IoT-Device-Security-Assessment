The following is the list of items required during the assessment:

`Status` column can be set for values similar to "Pass", "Fail", "N/A".

`Severity` column can be set for values "0-10" or "N/A" with 0 as the lowest to 10 being the highest potential magnitude of harm or damage if a risk event occurs (how bad). Refer to the [2.3. Validation Framework](./lib/02_framework/framework.md) for specific CVSS rating.

## 3.2 Network, API & Wireless Testing
| Test ID | Phase / Test Name | Status | Severity | Notes / Evidence |
| :--- | :--- | :--- | :--- | :--- |
| IDSA-NET-SCAN-01 | Service Discovery & Info (FR3, FR12, FR13) | | | **Nmap:** Enumerate open ports, service versions, and OS fingerprints. Use **NSE scripts** to check for known CVEs on identified services. |
| IDSA-NET-STRM-01 | Traffic Encryption (FR8, FR9, FR10) | | | **Wireshark:** Verify WebRTC/Blink stream encryption. Monitor Wi-Fi for unencrypted PII; use **Foremost** to attempt image recovery from captured packets. |
| IDSA-NET-RF-01 | Wireless Interface Security (FR14) | | | **Wireshark:** Analyze WPA2/3 handshakes. Perform de-authentication tests to check if the camera fails insecurely or stops recording during jamming. |
| IDSA-API-TEST-01 | API Interception & Auth (FR15, FR16) | | | **Burp Suite:** Intercept App-to-Cloud calls. Test for **BOLA** (changing Device IDs), session hijacking, and credential harvesting/phishing risks in UI. |
| IDSA-API-FUZZ-01 | API Fuzzing & Pattern Logging (FR17, FR18) | | | Run fuzzing on endpoints; test Blink App login for **rate limiting** and brute-force resistance. |
