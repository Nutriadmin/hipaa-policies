# 17. Data Integrity Policy

NutriAdmin takes data integrity very seriously. As stewards and partners of NutriAdmin Customers, we strive to assure data is protected from unauthorized access and that it is available when needed. The following policies drive many of our procedures and technical settings in support of the NutriAdmin mission of data protection.

Production systems that create, receive, store, or transmit Customer data (hereafter "Production Systems") must follow the guidelines described in this section.

## 17.1 Applicable Standards from the HIPAA Security Rule

* 164.308(a)(8) - Evaluation

## 17.2 Disabling Non-Essential Services

1. All Production Systems must disable services that are not required to achieve the business purpose or function of the system.

## 17.3 Monitoring Log-in Attempts

1. All access to Production Systems must be logged. This is done following the NutriAdmin Auditing Policy.

## 17.4 Prevention of Malware on Production Systems

1. All Production Systems are managed Azure solutions that are covered under NutriAdmin's HIPAA BAA with Microsoft. Microsoft is responsible for securing the systems to ensure data integrity.
2. If NutriAdmin were to implement a custom production system solution, such system must have OSSEC running (or equivalent), and set to scan system every 2 hours and at reboot to assure not malware is present. Detected malware is evaluated and removed.
3. Where appropriate, virus scanning software is run on all Production Systems for anti-virus protection.
   * Hosts are scanned daily for malicious binaries in critical system paths.
   * The malware signature database is checked hourly and automatically updated if new signatures are available.
   * Logs of virus scans are maintained according to the requirements outlined in [§8.6](#8.6-audit-log-security-controls-and-backup).
4. All Production Systems are to only be used for NutriAdmin business needs.

## 17.5 Patch Management

1. Software patches and updates will be applied to all systems in a timely manner. In the case of routine updates, they will be applied after thorough testing. In the case of updates to correct known vulnerabilities, priority will be given to testing to speed the time to production. Critical security patches are applied within 30 days from testing and all security patches are applied within 90 days after testing.
2. New updates to the software in NutriAdmin's application are peer-reviewed using a pull request strategy with Git. A member of NutriAdmin's management other than the initiator of the change must explicitly approve and review changes before they can be released in production.
3. NutriAdmin implements an automated build process that runs automated tests prior to a release in a production system. The process will only allow the release of changes that pass all the tests configured in the automated pipeline.

## 17.6 Intrusion Detection and Vulnerability Scanning

1. Production systems are monitored using IDS systems. Suspicious activity is logged and alerts are generated.
2. Vulnerability scanning of Production Systems is detailed in NutriAdmin's Vulnerability Scanning Policy.

## 17.7 Production System Security

1. System, network, and server security is managed and maintained by the Security Officer in conjunction with the Dev Ops team.
2. Up to date system lists are kept for all production environments automatically via the Azure Portal.
3. Access to Production Systems is controlled using centralized tools and two-factor authentication.

## 17.8 Production Data Security

1. Reduce the risk of compromise of Production Data.
2. Implement and/or review controls designed to protect Production Data from improper alteration or destruction.
3. Ensure that confidential data is stored in a manner that supports user access logs and automated monitoring for potential security incidents.
4. Ensure NutriAdmin Customer Production Data is segmented and only accessible to Customer authorized to access data. We use strategies such as access control, automated tests, and application code limitations to ensure this.
5. All Production Data at rest is stored on encrypted volumes using encryption keys managed by NutriAdmin.
6. Any systems that store ePHI are encrypted. 
7. Any relevant encryption keys or other type of secret keys are stored securely within an Azure Keyvault.
8. Encrypted volumes use AES encryption with a minimum of 256-bit keys, or keys and ciphers of equivalent or higher cryptographic strength. Where reasonable and available, the strongest encryption strategy will be used.

## 17.9 Transmission Security

1. All data transmission is encrypted from user to internet-facing web server using encryption keys managed by NutriAdmin.
2. Transmission encryption keys and machines that generate keys are protected from unauthorized access. Transmission encryption key material is protected with access controls such that the key material is only accessible by privileged accounts.
3. Transmission encryption keys are limited to use for a pre-determined amount of time and then must be regenerated.
4. In the case of NutriAdmin provided APIs, provide mechanisms to assure person sending or receiving data is authorized to send and save data.
5. NutriAdmin internal systems in Microsoft Azure are protected from the web via an application gateway
