The following is the list of items to test during the firmware assessment:

`Status` column can be set for values similar to "Pass", "Fail", "N/A".

`Severity` column can be set for values "0-10" with 0 as the lowest to 10 being the highest potential magnitude of harm or damage if a risk event occurs (how bad). Refer to the [2.3. Testing Methodology](.../framework/methodology.md) for specific CVSS rating.

## 3.1 Firmware (IDSA-FW)
|Test ID|Test Name|Status|Severity|Notes|
|-|-|-|-|-|
|**IDSA-FW-INFO**|**Information Gathering**||||
|IDSA-FW-INFO-001|Disclosure of Source Code and Binaries|||Analyze Blink updates via App; Use binwalk on RPi filesystem/EEPROM.|
|IDSA-FW-INFO-002|Disclosure of Implementation Details|||Check for exposed hardware specs or boot logs.|
|**IDSA-FW-CONF**|**Configuration and Patch Management**||||
|IDSA-FW-CONF-001|Usage of Outdated Software|||Check apt packages on RPi; Verify Blink firmware version in-app.|
|IDSA-FW-CONF-002|Update Mechanism Security|||Test Blink app-based updates vs. RPi sudo apt full-upgrade security|
|**IDSA-FW-SCRT**|**Secrets**||||
|IDSA-FW-SCRT-001|Secrets Stored in Public Storage|||Search for hardcoded keys in binwalk extracted files.|
|IDSA-FW-SCRT-002|Unencrypted Storage of Secrets|||Check /etc/ or config files on RPi; Check local cache for Blink.|
