# 21. 3rd Party Policy

NutriAdmin makes every effort to assure all 3rd party organizations are compliant and do not compromise the integrity, security, and privacy of NutriAdmin or NutriAdmin Customer data. 3rd Parties include Customers, Partners, Subcontractors, and Contracted Developers.

## 21.1 Applicable Standards from the HIPAA Security Rule

* 164.314(a)(1)(i) - Business Associate Contracts or Other Arrangements

## 21.2 Policies to Assure 3rd Parties Support NutriAdmin Compliance

1. NutriAdmin does not allow 3rd party access to production systems containing ePHI.
2. All connections and data in transit between the NutriAdmin Platform and 3rd parties are encrypted end to end.
3. A standard business associate agreement with Customers and Partners is defined and includes the required security controls in accordance with the organization's security policies. Additionally, responsibility is assigned in these agreements.
4. NutriAdmin has Service Level Agreements (SLAs) with Subcontractors with an agreed service arrangement addressing liability, service definitions, security controls, and aspects of services management.
   * Subcontractors must coordinate, manage, and communicate any changes to services provided to NutriAdmin.
   * Substantial changes to services provided by 3rd parties will invoke a Risk Assessment as described in [§4.2](#4.2-risk-management-policies).
5. No NutriAdmin Customers or Partners have access outside of their own environment, meaning they cannot access, modify, or delete anything related to other 3rd parties.
7. NutriAdmin maintains and annually reviews a list all current Partners and Subcontractors.
   * The list of current Partners and Subcontractors is maintained by the NutriAdmin Privacy Officer, includes details on all provided services (along with contact information), and is recorded in several places, including [§1.4](#1.4-nutriadmin-organizational-concepts), the list below, our GDPR policy, and the risk assessment.
   * The annual review of Partners and Subcontractors is conducted as a part of the security, compliance, and SLA review referenced below.
8. NutriAdmin assesses security, compliance, and SLA requirements and considerations with all Partners and Subcontractors. This includes annual assessment of SOC2 Reports for all NutriAdmin infrastructure partners.
   * NutriAdmin leverages recurring calendar invites to assure reviews of all 3rd party services are performed annually. These reviews are performed by the NutriAdmin Security Officer and Privacy Officer. The process for reviewing 3rd party services is outlined below:
     1. The Security Officer initiates the SLA review by creating a Task in the Compliance Review Activity (CRA) Spreadsheet with ID #CRA-17.
     2. The Security Officer, or Privacy Officer, is assigned to review the SLA and performance of 3rd parties. The list of current 3rd parties, including contact information, is also reviewed to assure it is up to date and complete.
     3. SLA, security, and compliance performance is documented in the Task.
     4. Once the review is completed and documented, the Security Officer approves or rejects the Task. If the Task is rejected, it goes back for further review and documentation.
     5. Compliance with annual third party review is monitored on a yearly basis using the Compliance Review Activity (CRA) Spreadsheet to assess compliance with above policy. This monitoring activity is recorded using ID #CRA-18.
9. Regular review is conducted as required by SLAs to assure security and compliance. These reviews include reports, audit trails, security events, operational issues, failures and disruptions, and identified issues are investigated and resolved in a reasonable and timely manner.
10. Any changes to Partner and Subcontractor services and systems are reviewed before implementation.
11. For all partners, NutriAdmin reviews activity annually to assure partners are in line with SLAs in contracts with NutriAdmin.

## 21.3 List of NutriAdmin subcontractors which may have access to ePHI

* **Microsoft Azure**. Azure is used to host the majority of the NutriAdmin infrastructure, including web apps and a database. Azure also stores backups, logs, analytics, and networking components.
* **Google**. Google G Suite is used, amongst other things, for email communication via Gmail. Automated emails from the application never contain ePHI by default. Google analytics also records web traffic data when the user of the website accepts the relevant cookies.
* **AWS**. Amazon Web Services (AWS) is used to keep encrypted backups of production data in S3 (as a double-redundancy mechanism, since backups are also kept in Azure). Additionally, AWS is used as part of the NutriAdmin application to send text codes for phone verification to access NutriAdmin's client portal.
* **Twilio**. Twilio is used as a backup mechanism to send text codes for verification when clients access the client portal in the application.
* **Stripe**. Stripe is used for payment processing for users of NutriAdmin. 

More information about third parties can be found at [our GDPR information page](https://nutriadmin.com/docs/nutriadmin-gdpr-general-data-protection-regulation-information).
