The following is the list of items to test during the physical interfaces assessment:

`Status` column can be set for values similar to "Pass", "Fail", "N/A".

`Severity` column can be set for values "0-10" with 0 as the lowest to 10 being the highest potential magnitude of harm or damage if a risk event occurs (how bad). Refer to the [2.3. Testing Methodology](../../02_framework/methodology.md) for specific CVSS rating.

## 3.4 Physical Interfaces (IDSA-PHYS)
|Test ID|Test Name|Status|Severity|Notes|
|-|-|-|-|-|
|IDSA-PHYS-001|USB Host Detection (Win/Lin/Mac)|||Does it mount as a camera/webcam or a storage device?|
|IDSA-PHYS-002|Unauthorized Peripheral Access|||Does plugging it in provide a serial shell or unintended file access?|
|IDSA-PHYS-003|HID Attack Surface|||Can the device be spoofed to act as a keyboard when plugged in?|
