# PCI Data Security Standard

## Introduction and Overview

PCI DSS provides a baseline of technical and operational requirements designed to protect account data.

| Category | Item | Standard |
| -- | -- | -- |
| Build and Maintain a Secure Network and Systems | 1 | Install and maintain a firewall configuration to protect cardholder data |
| Build and Maintain a Secure Network and Systems | 2 | Do not use vendor-supplied defaults for system passwords and other security parameters |
| Protect Cardholder Data | 3 | Protect stored cardholder data |
| Protect Cardholder Data | 4 | Encrypt transmission of cardholder data across open, public networks |
| Maintain a Vulnerability Management Program | 5 | Protect all systems against malware and regularly update anti-virus software or programs |
| Maintain a Vulnerability Management Program | 6 | Develop and maintain secure systems and applications |
| Implement Strong Access Control Measures | 7 | Restrict access to cardholder data by business need to know |
| Implement Strong Access Control Measures | 8 | Identify and authenticate access to system components |
| Implement Strong Access Control Measures | 9 | Restrict physical access to cardholder data |
| Regularly Monitor and Test Networks | 10 | Track and monitor all access to network resources and cardholder data |
| Regularly Monitor and Test Networks | 11 | Regularly test security systems and processes |
| Maintain an Information Security Policy | 12 | Maintain a policy that addresses information security for all personnel |

PCI DSS comprises a minimum set of requirements for protecting account data, and may be enhanced by additional controls and practices to further mitigate risks, as well as local, regional and sector laws and regulations.


## PCI DSS Applicability information

PCI DSS applies to all entities involved in payment card processing—including merchants, processors, acquirers, issuers, and service providers. PCI DSS also applies to all other entities that store, process, or transmit cardholder data and/or sensitive authentication data.

Cardholder data and sensitive authentication data are defined as follows:
* Cardholder Data includes:
  * Primary Account Number (PAN)
  * Cardholder Name
  * Expiration Date
  * Service Code
* Sensitive Authentication Data includes:
  * Full track data (magnetic-stripe data or equivalent on a chip)
  * CAV2/CVC2/CVV2/CID
  * PINs/PIN blocks

The primary account number is the defining factor for cardholder data. If cardholder name, service code, and/or expiration date are stored, processed or transmitted with the PAN, or are otherwise present in the cardholder data environment (CDE), they must be protected in accordance with applicable PCI DSS requirements.

The table on the following page illustrates commonly used elements of cardholder and sensitive authentication data, whether storage of each data element is permitted or prohibited, and whether each data element must be protected.

| Account Data | Data Element |  Storage Permitted | Should Be Unreadable |
| -- | -- | -- | -- |
| Cardholder Data | Primary Account Number (PAN) | Yes | Yes |
| Cardholder Data | Cardholder Name | Yes | No |
| Cardholder Data | Service Code | Yes | No |
| Cardholder Data | Expiration Date | Yes | No |
| Sensitive Authentication Data | Full Track Data | No | Cannot store |
| Sensitive Authentication Data | CAV2/CVC2/CVV2/CID | No | Cannot store |
| CAV2/CVC2/CVV2/CID | PIN/PIN block | No | Cannot store |
