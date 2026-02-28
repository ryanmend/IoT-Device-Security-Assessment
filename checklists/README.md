# Testing Checklist

The following is the list of items to test during the assessment:

Note: The `Status` column can be set for values similar to "Pass", "Fail", "N/A".

## Processing Units (IDSA-PU)
|Test ID|Test Name|Status|Notes|
|-|-|-|-|
|**IDSA-PU-AUTHZ**|**Authorization**|||
|IDSA-PU-AUTHZ-001|Unauthorized Access to the Processing Unit|||
|IDSA-PU-AUTHZ-002|Privilege Escalation|||
|**IDSA-PU-LOGIC**|**Business Logic**|||
|IDSA-PU-LOGIC-001|Insecure Implementation of Instructions|||
|**IDSA-PU-SIDEC**|**Side-Channel Attacks**|||
|IDSA-PU-SIDEC-001|Insufficient Protection Against Side-Channel Attacks|||

## Memory (IDSA-MEM)
|Test ID|Test Name|Status|Notes|
|-|-|-|-|
|**IDSA-MEM-INFO**|**Information Gathering**|||
|IDSA-MEM-INFO-001|Disclosure of Source Code and Binaries|||
|IDSA-MEM-INFO-002|Disclosure of Implementation Details|||
|IDSA-MEM-INFO-003|Disclosure of Ecosystem Details|||
|IDSA-MEM-INFO-004|Disclosure of User Data|||
|**IDSA-MEM-SCRT**|**Secrets**|||
|IDSA-MEM-SCRT-001|Unencrypted Storage of Secrets|||
|**IDSA-MEM-CRYPT**|**Cryptography**|||
|IDSA-MEM-CRYPT-001|Usage of Weak Cryptographic Algorithms|||

## Firmware (IDSA-FW)
|Test ID|Test Name|Status|Notes|
|-|-|-|-|
|**IDSA-FW-INFO**|**Information Gathering**|||
|IDSA-FW-INFO-001|Disclosure of Source Code and Binaries|||
|IDSA-FW-INFO-002|Disclosure of Implementation Details|||
|IDSA-FW-INFO-003|Disclosure of Ecosystem Details|||
|**IDSA-FW-CONF**|**Configuration and Patch Management**|||
|IDSA-FW-CONF-001|Usage of Outdated Software|||
|IDSA-FW-CONF-002|Presence of Unnecessary Software and Functionalities|||
|**IDSA-FW-SCRT**|**Secrets**|||
|IDSA-FW-SCRT-001|Secrets Stored in Public Storage|||
|IDSA-FW-SCRT-002|Unencrypted Storage of Secrets|||
|IDSA-FW-SCRT-003|Usage of Hardcoded Secrets|||
|**IDSA-FW-CRYPT**|**Cryptography**|||
|IDSA-FW-CRYPT-001|Usage of Weak Cryptographic Algorithms|||

### Installed Firmware (IDSA-FW[INST])
|Test ID|Test Name|Status|Notes|
|-|-|-|-|
|**IDSA-FW[INST]-AUTHZ**|**Authorization**|||
|IDSA-FW[INST]-AUTHZ-001|Unauthorized Access to the Firmware|||
|IDSA-FW[INST]-AUTHZ-002|Privilege Escalation|||
|**IDSA-FW[INST]-INFO**|**Information Gathering**|||
|IDSA-FW[INST]-INFO-001|Disclosure of User Data|||
|**IDSA-FW[INST]-CRYPT**|**Cryptography**|||
|IDSA-FW[INST]-CRYPT-001|Insufficient Verification of the Bootloader Signature|||

### Firmware Update Mechanism (IDSA-FW[UPDT])
|Test ID|Test Name|Status|Notes|
|-|-|-|-|
|**IDSA-FW[UPDT]-AUTHZ**|**Authorization**|||
|IDSA-FW[UPDT]-AUTHZ-001|Unauthorized Firmware Update|||
|**IDSA-FW[UPDT]-CRYPT**|**Cryptography**|||
|IDSA-FW[UPDT]-CRYPT-001|Insufficient Firmware Update Signature|||
|IDSA-FW[UPDT]-CRYPT-002|Insufficient Firmware Update Encryption|||
|IDSA-FW[UPDT]-CRYPT-003|Insecure Transmission of the Firmware Update|||
|IDSA-FW[UPDT]-CRYPT-004|Insufficient Verification of the Firmware Update Signature|||
|**IDSA-FW[UPDT]-LOGIC**|**Business Logic**|||
|IDSA-FW[UPDT]-LOGIC-001|Insufficient Rollback Protection|||

## Data Exchange Services (IDSA-NET)
|Test ID|Test Name|Status|Notes|
|-|-|-|-|
|**IDSA-NET-AUTHZ**|**Authorization**|||
|IDSA-NET-AUTHZ-001|Unauthorized Access to the Data Exchange Service|||
|IDSA-NET-AUTHZ-002|Privilege Escalation|||
|**IDSA-NET-INFO**|**Information Gathering**|||
|IDSA-NET-INFO-001|Disclosure of Implementation Details|||
|IDSA-NET-INFO-002|Disclosure of Ecosystem Details|||
|IDSA-NET-INFO-003|Disclosure of User Data|||
|**IDSA-NET-CONF**|**Configuration and Patch Management**|||
|IDSA-NET-CONF-001|Usage of Outdated Software|||
|IDSA-NET-CONF-002|Presence of Unnecessary Software and Functionalities|||
|**IDSA-NET-SCRT**|**Secrets**|||
|IDSA-NET-SCRT-001|Access to Confidential Data|||
|**IDSA-NET-CRYPT**|**Cryptography**|||
|IDSA-NET-CRYPT-001|Usage of Weak Cryptographic Algorithms|||
|**IDSA-NET-LOGIC**|**Business Logic**|||
|IDSA-NET-LOGIC-001|Circumvention of the Intended Business Logic|||
|**IDSA-NET-INPV**|**Input Validation**|||
|IDSA-NET-INPV-001|Insufficient Input Validation|||
|IDSA-NET-INPV-002|Code or Command Injection|||

## Internal Interfaces (IDSA-INT)
|Test ID|Test Name|Status|Notes|
|-|-|-|-|
|**IDSA-INT-AUTHZ**|**Authorization**|||
|IDSA-INT-AUTHZ-001|Unauthorized Access to the Interface|||
|IDSA-INT-AUTHZ-002|Privilege Escalation|||
|**IDSA-INT-INFO**|**Information Gathering**|||
|IDSA-INT-INFO-001|Disclosure of Implementation Details|||
|IDSA-INT-INFO-002|Disclosure of Ecosystem Details|||
|IDSA-INT-INFO-003|Disclosure of User Data|||
|**IDSA-INT-CONF**|**Configuration and Patch Management**|||
|IDSA-INT-CONF-001|Usage of Outdated Software|||
|IDSA-INT-CONF-002|Presence of Unnecessary Software and Functionalities|||
|**IDSA-INT-SCRT**|**Secrets**|||
|IDSA-INT-SCRT-001|Access to Confidential Data|||
|**IDSA-INT-CRYPT**|**Cryptography**|||
|IDSA-INT-CRYPT-001|Usage of Weak Cryptographic Algorithms|||
|**IDSA-INT-LOGIC**|**Business Logic**|||
|IDSA-INT-LOGIC-001|Circumvention of the Intended Business Logic|||
|**IDSA-INT-INPV**|**Input Validation**|||
|IDSA-INT-INPV-001|Insufficient Input Validation|||
|IDSA-INT-INPV-002|Code or Command Injection|||

## Physical Interfaces (IDSA-PHY)
|Test ID|Test Name|Status|Notes|
|-|-|-|-|
|**IDSA-PHY-AUTHZ**|**Authorization**|||
|IDSA-PHY-AUTHZ-001|Unauthorized Access to the Interface|||
|IDSA-PHY-AUTHZ-002|Privilege Escalation|||
|**IDSA-PHY-INFO**|**Information Gathering**|||
|IDSA-PHY-INFO-001|Disclosure of Implementation Details|||
|IDSA-PHY-INFO-002|Disclosure of Ecosystem Details|||
|IDSA-PHY-INFO-003|Disclosure of User Data|||
|**IDSA-PHY-CONF**|**Configuration and Patch Management**|||
|IDSA-PHY-CONF-001|Usage of Outdated Software|||
|IDSA-PHY-CONF-002|Presence of Unnecessary Software and Functionalities|||
|**IDSA-PHY-SCRT**|**Secrets**|||
|IDSA-PHY-SCRT-001|Access to Confidential Data|||
|**IDSA-PHY-CRYPT**|**Cryptography**|||
|IDSA-PHY-CRYPT-001|Usage of Weak Cryptographic Algorithms|||
|**IDSA-PHY-LOGIC**|**Business Logic**|||
|IDSA-PHY-LOGIC-001|Circumvention of the Intended Business Logic|||
|**IDSA-PHY-INPV**|**Input Validation**|||
|IDSA-PHY-INPV-001|Insufficient Input Validation|||
|IDSA-PHY-INPV-002|Code or Command Injection|||

## Wireless Interfaces (IDSA-RF)
|Test ID|Test Name|Status|Notes|
|-|-|-|-|
|**IDSA-RF-AUTHZ**|**Authorization**|||
|IDSA-RF-AUTHZ-001|Unauthorized Access to the Interface|||
|IDSA-RF-AUTHZ-002|Privilege Escalation|||
|**IDSA-RF-INFO**|**Information Gathering**|||
|IDSA-RF-INFO-001|Disclosure of Implementation Details|||
|IDSA-RF-INFO-002|Disclosure of Ecosystem Details|||
|IDSA-RF-INFO-003|Disclosure of User Data|||
|**IDSA-RF-CONF**|**Configuration and Patch Management**|||
|IDSA-RF-CONF-001|Usage of Outdated Software|||
|IDSA-RF-CONF-002|Presence of Unnecessary Software and Functionalities|||
