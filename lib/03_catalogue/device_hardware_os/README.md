The following is the list of items required during the assessment:

`Status` column can be set for values similar to "Pass", "Fail", "N/A".

`Severity` column can be set for values "0-10" or "N/A" with 0 as the lowest to 10 being the highest potential magnitude of harm or damage if a risk event occurs (how bad). Refer to the [2.3. Testing Methodology](./src/02_framework/methodology.md) for specific CVSS rating.

## 3.4 Device Hardware & OS Security
| Test ID | Phase / Test Name | Status | Severity | Notes / Evidence |
| :--- | :--- | :--- | :--- | :--- |
| IDSA-OS-HARD-01 | System Hardening (FR24) | | | Check RPi OS for default `pi` credentials and unnecessary services. Test Blink App UI for bypasses in lock screen or biometric auth. |
| IDSA-OS-CAM-01 | Camera Subsystem Security (FR25) | | | **OpenCV:** Attempt to hijack the stream via secondary scripts, inject pre-recorded video loops, and check `/dev/shm` or `/tmp` for leaked frames. |
| IDSA-PHYS-01 | Physical Interface Attack Surface (FR26) | | | **USB Testing:** Check if device mounts as storage/webcam; test for unauthorized serial shells; test if device can be spoofed as an **HID (Keyboard)** attack. |
