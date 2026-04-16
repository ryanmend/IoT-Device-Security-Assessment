The following is the list of items required during the assessment:

`Status` column can be set for values similar to "Pass", "Fail", "N/A".

`Severity` column can be set for values "0-10" or "N/A" with 0 as the lowest to 10 being the highest potential magnitude of harm or damage if a risk event occurs (how bad). Refer to the [2.3. Testing Methodology](./src/02_framework/methodology.md) for specific CVSS rating.

## 3.3 Firmware Analysis
| Test ID | Phase / Test Name | Status | Severity | Notes / Evidence |
| :--- | :--- | :--- | :--- | :--- |
| IDSA-FW-ACQ-01 | Acquisition & Backup (FR19, FR21) | | | Verify firmware is saved; analyze Blink updates via App and capture RPi boot logs. |
| IDSA-FW-EXTRACT-01| Extraction & Binwalk (FR20) | | | Use **Binwalk** on RPi filesystem and EEPROM to extract files and identify disclosure of source code or binaries. |
| IDSA-FW-SCRT-01 | Secrets & Hardcoded Keys (FR22) | | | Search extracted files for hardcoded keys/passwords. Check `/etc/` and config files for unencrypted secrets and local Blink caches. |
| IDSA-FW-CONF-01 | Insecure Configs & Libraries (FR23) | | | Check `apt` packages on RPi for outdated software. Evaluate security of the update mechanism (Blink App vs. `sudo apt full-upgrade`). |
