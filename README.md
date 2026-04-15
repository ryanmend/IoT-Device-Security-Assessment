<a href="https://github.com/ryanmend/IoT-Device-Security-Assessment"><img width="180px" align="right" style="float: right;" src="src/img/idsa_cover.png"></a>

# IoT Device Security Assessment

This IoT Device Security Assessment project presents the design and development aimed at evaluating the security posture of consumer Internet of Things (IoT) devices across network, application, and firmware layers. Motivated by the rapid expansion of IoT ecosystems and the corresponding rise in security risks, the project applies an evidence-driven methodology inspired by industry standards such as the OWASP IoT Top 10 and NIST guidelines. The assessment framework guides the structured analysis of device behaviour, cloud interactions, and internal software components, ultimately enabling a comprehensive understanding of vulnerabilities and their implications.

![Component Overview](src/img/component_overview.png)


## Table of Contents

1. [**Introduction**](./src/01_introduction/README.md)

2. [**IoT Security Testing Framework**](./src/02_framework/README.md)

   2.1. [IoT Device Model](./src/02_framework/device_model.md)

   2.2. [Threat Model](./src/02_framework/threat_model.md)

   2.3. [Testing Methodology](./src/02_framework/methodology.md)

3. [**Test Case Catalog**](./src/03_test_cases/README.md)

   3.1. [Firmware (IDSA-FW)](./src/03_test_cases/firmware/README.md)

   3.2. [Network Data Services (IDSA-NET)](./src/03_test_cases/network_data_services/README.md)

   3.3. [API & Cloud Integration (IDSA-API)](./src/03_test_cases/api_&_cloud/README.md)

   3.4. [Physical Interfaces (IDSA-PHYS)](./src/03_test_cases/physical_interfaces/README.md)

   3.5. [Wireless Interfaces (IDSA-RF)](./src/03_test_cases/wireless_interfaces/README.md)

   3.6. [Operating System & UI (IDSA-OS)](./src/03_test_cases/os_&_ui/README.md)


# Testing Checklist

The following is the list of items to test during the assessment:

`Status` column can be set for values similar to "Pass", "Fail", "N/A".

`Severity` column can be set for values "0-10" with 0 as the lowest to 10 being the highest potential magnitude of harm or damage if a risk event occurs (how bad). Refer to the [2.3. Testing Methodology](./src/02_framework/methodology.md) for specific CVSS rating.

## 1.0 Setup & Threat Modeling
| Test ID | Phase / Test Name | Status | Severity | Notes / Evidence |
| :--- | :--- | :--- | :--- | :--- |
| FR-SETUP-01 | Device Selection & Inventory (FR1, FR2) | | | Verify device specs and firmware version recorded. |
| FR-MODEL-01 | OWASP IoT Threat Model (FR4, FR5) | | | Ensure attack vectors are identified and documented. |
| FR-MODEL-02 | Visual Threat Diagram (FR6) | | | Confirm diagram shows all attack surfaces. |
| FR-MODEL-03 | Threat Impact Rating (FR7) | | | Verify likelihood/impact scores assigned to threats. |

## 2.0 Network & API Testing
| Test ID | Phase / Test Name | Status | Severity | Notes / Evidence |
| :--- | :--- | :--- | :--- | :--- |
| IDSA-NET-SCAN-01 | Service Discovery & Info (FR3, FR12, FR13) | | | Use Nmap; record all open ports/services found. |
| IDSA-NET-STRM-01 | Traffic Encryption (FR8, FR9, FR10) | | | Wireshark analysis: check for plaintext/weak TLS. |
| IDSA-API-TEST-01 | API Interception & Auth (FR15, FR16) | | | Burp Suite: test tokens, session, and validation. |
| IDSA-API-FUZZ-01 | API Fuzzing & Pattern Logging (FR17, FR18) | | | Run fuzzing; log request/response patterns. |

## 3.0 Firmware Analysis
| Test ID | Phase / Test Name | Status | Severity | Notes / Evidence |
| :--- | :--- | :--- | :--- | :--- |
| FR-FW-ACQ-01 | Acquisition & Backup (FR19, FR21) | | | Verify firmware is saved and versioned correctly. |
| IDSA-FW-EXTRACT-01| Extraction & Binwalk (FR20) | | | Confirm successful filesystem extraction. |
| IDSA-FW-SCRT-01 | Secrets & Hardcoded Keys (FR22) | | | Search extracted files for keys, passwords, API keys. |
| IDSA-FW-CONF-01 | Insecure Configs & Libraries (FR23) | | | Check for outdated libraries/insecure settings. |

## 4.0 Correlation & Risk Evaluation
| Test ID | Phase / Test Name | Status | Severity | Notes / Evidence |
| :--- | :--- | :--- | :--- | :--- |
| FR-CORR-01 | Vulnerability Correlation (FR25, FR26) | | | Cross-reference network findings with firmware results. |
| FR-RISK-01 | Risk Matrix & Severity (FR27, FR28) | | | Map all identified vulnerabilities to a risk matrix. |
| FR-MITIG-01 | Mitigation Recommendations (FR29) | | | Develop OWASP-aligned fix strategies. |

## 5.0 Reporting & Deliverables
| Test ID | Phase / Test Name | Status | Severity | Notes / Evidence |
| :--- | :--- | :--- | :--- | :--- |
| FR-REPT-01 | Technical Report Compilation (FR30, FR32) | | | Final report with all screenshots and logs attached. |
| FR-REPT-02 | Executive Summary & Presentation (FR31) | | | Prepare non-technical summary for stakeholders. |

## Project Collaborators and Acknowledgements

We would like to take this opportunity to acknowledge the contribution of our professor Mandeep Pannu for guiding us into the right direction. This framework would not have been possible without you.

* Amer Al Sous
* Waleed Kuvailid
* Ryan Mendoza
