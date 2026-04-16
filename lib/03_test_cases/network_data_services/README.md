The following is the list of items to test during the network data services assessment:

`Status` column can be set for values similar to "Pass", "Fail", "N/A".

`Severity` column can be set for values "0-10" with 0 as the lowest to 10 being the highest potential magnitude of harm or damage if a risk event occurs (how bad). Refer to the [2.3. Testing Methodology](../../02_framework/methodology.md) for specific CVSS rating.

## 3.2 Network Data Services (IDSA-NET)
|Test ID|Test Name|Status|Severity|Notes|
|-|-|-|-|-|
|**IDSA-NET-SCAN**|**Service Discovery**||||
|IDSA-NET-SCAN-001|Open Port & Service Enumeration|||Use nmap to identify listening ports, service versions, and OS fingerprints.|
|IDSA-NET-SCAN-002|Vulnerability Scanning (NSE)|||Use nmap scripting engine (NSE) to check for known CVEs on open services.|
|**IDSA-NET-STRM**|**Stream Encryption**||||
|IDSA-NET-STRM-001|Encrypted Media Streaming|||Use Wireshark to verify if Blink/RPi (WebRTC) streams are encrypted.|
|IDSA-NET-STRM-002|LAN Data Transmission|||Monitor Wi-Fi traffic for unencrypted PII or command packets. **Convert captured packets to images using Foremost.**|
|**IDSA-NET-AUTH**|**Authentication Security**||||
|IDSA-NET-AUTH-001|Brute Force / Rainbow Table|||Test Blink App login and RPi SSH/Local login for rate limiting.|
|IDSA-NET-AUTH-002|Phishing & Session Hijacking|||Evaluate Blink UI for credential harvesting risks.|
