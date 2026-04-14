The following is the list of items to test during the operating system and UI assessment:

`Status` column can be set for values similar to "Pass", "Fail", "N/A".

`Severity` column can be set for values "0-10" with 0 as the lowest to 10 being the highest potential magnitude of harm or damage if a risk event occurs (how bad). Refer to the [2.3. Testing Methodology](../../02_framework/methodology.md) for specific CVSS rating.

## 3.6 Operating System & UI (IDSA-OS)
|Test ID|Test Name|Status|Severity|Notes|
|-|-|-|-|-|
|**IDSA-OS-HARD**|**System Hardening**||||
|IDSA-OS-HARD-001|Raspberry Pi OS Hardening|||Check for default pi credentials or unnecessary services.|
|IDSA-OS-HARD-002|Blink App UI Logic|||Test for bypasses in the app's lock screen or biometric auth.|
|**IDSA-OS-CAM**|**Camera Subsystem Security**||||
|IDSA-OS-CAM-001|Unauthorized Stream Capture|||Use OpenCV to see if a secondary script can hijack the camera while the main app is running.|
|IDSA-OS-CAM-002|Video Injection / Spoofing|||Use OpenCV to attempt to inject a pre-recorded video loop into the stream buffer.|
|IDSA-OS-CAM-003|Buffer Privacy / Local Leaks|||Use OpenCV to check if sensitive frames are left in /dev/shm or tmp directories after a capture.|
