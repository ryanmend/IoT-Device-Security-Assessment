<a href="https://github.com/ryanmend/IoT-Device-Security-Assessment"><img width="180px" align="right" style="float: right;" src="src/img/idsa_cover.png"></a>

# IoT Device Security Assessment

This IoT Device Security Assessment project presents the design and development aimed at evaluating the security posture of consumer Internet of Things (IoT) devices across network, application, and firmware layers. Motivated by the rapid expansion of IoT ecosystems and the corresponding rise in security risks, the project applies an evidence-driven methodology inspired by industry standards such as the OWASP IoT Top 10 and NIST guidelines. The assessment framework guides the structured analysis of device behaviour, cloud interactions, and internal software components, ultimately enabling a comprehensive understanding of vulnerabilities and their implications.

![Component Overview](src/img/Component_Overview.png)


## Table of Contents

1. [**Introduction**](./src/01_introduction/README.md)

2. [**IoT Security Testing Framework**](./src/02_framework/README.md)

   2.1. [IoT Device Model](./src/02_framework/device_model.md)

   2.2. [Threat Model](./src/02_framework/threat_model.md)

   2.3. [Testing Methodology](./src/02_framework/methodology.md)

3. [**Test Case Catalog**](./src/03_test_cases/README.md)

   3.1. [Firmware (IDSA-FW)](./src/03_test_cases/firmware/README.md)

      3.1.1. [Installed Firmware (IDSA-FW[INST])](./src/03_test_cases/firmware/installed_firmware.md)

      3.1.1. [Firmware Update Mechnanism (IDSA-FW[UPDT])](./src/03_test_cases/firmware/firmware_update_mechanism.md)

   3.2. [Data Exchange Services (IDSA-NET)](./src/03_test_cases/data_exchange_services/README.md)

   3.3. [Internal Interfaces (IDSA-INT)](./src/03_test_cases/internal_interfaces/README.md)

   3.4. [Physical Interfaces (IDSA-PHY)](./src/03_test_cases/physical_interfaces/README.md)

   3.5. [Wireless Interfaces (IDSA-RF)](./src/03_test_cases/wireless_interfaces/README.md)

   3.6. [User Interfaces (IDSA-UI)](./src/03_test_cases/user_interfaces/README.md)


## Project Collaborators and Acknowledgements

We would like to take this opportunity to acknowledge the contribution of our professor Mandeep Pannu for guiding us into the right direction. This framework would not have been possible without you.

* Amer Al Sous
* Waleed Kuvailid
* Ryan Mendoza
