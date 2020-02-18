# 6. Data Management Policy

NutriAdmin has procedures to create and maintain retrievable exact copies of electronic protected health information (ePHI) for all of our SaaS Customers. The policy and procedures will assure that complete, accurate, retrievable, and tested backups are available for all systems used by NutriAdmin.

Data backup is an important part of the day-to-day operations of NutriAdmin. To protect the confidentiality, integrity, and availability of ePHI, both for NutriAdmin and NutriAdmin Customers, complete backups are done daily to assure that data remains available when it is needed and in case of a disaster.

Violation of this policy and its procedures by workforce members may result in corrective disciplinary action, up to and including termination of employment.

## 6.1 Applicable Standards from the HIPAA Security Rule

* 164.308(a)(7)(ii)(A) - Data Backup Plan
* 164.310(d)(2)(iii) - Accountability
* 164.310(d)(2)(iv) - Data Backup and Storage

## 6.2 Backup Policy and Procedures

1. An automatic configuration is in place to perform daily snapshot backups of all systems that process, store, or transmit ePHI for all NutriAdmin Customers.
2. The NutriAdmin Ops Team is designated to be in charge of backups.
3. Dev Ops Team members are trained and assigned to complete backups and manage the backup media.
4. Backups are stored in encrypted storage, and kept in at least two different places for redundancy. Currently, daily backups are stored in Microsoft Azure, and another copy in AWS.
5. Securely encrypt stored backups in a manner that protects them from loss or environmental damage.
6. Backups are tested periodically during normal operations by the Dev Ops Team. Every time a Customer requests that data is restored from a backup, the Dev Ops team will verify as part of the request that backups contain accurate data that can be retrieved to meet the Customer's request. If any aspect of backups is found to be inadequate, then this is notified to the Security Office who will decide a course of action to rectify the problem.
7. Monitor once a year that backups have been generated appropriately and track this activity on the Azure DevOps Compliance Review Activity (CRA) Spreadsheet with ID #CRA-8. If there have been no request for backup restoration by Customers during the previous year, then the Dev Ops team tests backups separately to ensure their proper functioning.
8. In addition to daily snapshots of the database, the NutriAdmin software also stores incremental changes for critical data, e.g. changes to client records, questionnaires, or reports.
