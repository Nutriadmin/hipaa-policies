# 3. Policy Management Policy

NutriAdmin implements policies and procedures to maintain compliance and integrity of data. The Security Officer and Privacy Officer are responsible for maintaining policies and procedures and assuring all NutriAdmin workforce members, business associates, customers, and partners are adherent to all applicable policies. Previous versions of policies are retained to assure ease of finding policies at specific historic dates in time.

## 3.1 Applicable Standards from the HIPAA Security Rule

* 164.316(a) - Policies and Procedures
* 164.316(b)(1)(i) - Documentation

## 3.2 Maintenance of Policies

1. All policies are stored and up to date to maintain NutriAdmin compliance with HIPAA, and other relevant standards. Updates and version control are done similar to source code control.
2. Policy update requests can be made by any workforce member at any time. Furthermore, all policies are reviewed annually by both the Security and Privacy Officer to assure they are accurate and up-to-date.
3. NutriAdmin employees may request changes to policies using the following process:
    1. The NutriAdmin employee initiates a policy Change Request by creating a User Story on the Azure DevOps Compliance Review Activity (CRA) Project and by sending an email detailing the proposed change to the Security Officer or to the Privacy Officer. The Change Request may optionally include a GitHub pull request from a separate branch or repository containing the desired changes.
    2. The Security Officer or the Privacy Officer is assigned to review the policy Change Request.
    3. Once the review is completed, the Security Officer or Privacy Officer approves or rejects the Change Request. If the Change Request is rejected, it goes back for further review and documentation.
    4. If the review is approved, the Security Officer or Privacy Officer implements the Change Request to the policy or assigns an authorized employee to publish the changes. The Security Officer or Privacy officer may add any pertinent notes required.
    5. If the policy change requires technical modifications to production systems, those changes are carried out by authorized personnel.
4. All policies are made accessible to all NutriAdmin workforce members. The current master policies are published at [https://nutriadmin.com/policy](https://nutriadmin.com/policy).
   * The Security Officer communicates policy changes to all employees via email. These emails include a high-level description of the policy change using terminology appropriate for the target audience plus a link to the Github repository where the employees can see the changes in detail.
5. All policies, and associated documentation, are retained for 6 years from the date of its creation or the date when it last was in effect, whichever is later
   1. Version history of all NutriAdmin policies is done via GitHub.
   2. Backup storage of all policies is done with Microsoft's Azure DevOps.
6. The policies and information security policies are reviewed and audited annually, or after significant changes occur to NutriAdmin's organizational environment. Issues that come up as part of this process are reviewed by NutriAdmin management to assure all risks and potential gaps are mitigated and/or fully addressed. The process for reviewing polices is outlined below:
    1. The Security Officer initiates the policy review by recording a User Story in the Azure DevOps Compliance Review Activity (CRA) Project.
    2. The Security Officer or the Privacy Officer is assigned to review the current NutriAdmin policies ([https://nutriadmin.com/policy/](https://nutriadmin.com/policy/)).
    3. If changes are made, the above process is used. All changes are documented in the User Story.
    4. Once the review is completed, the Security Officer or Privacy Officer approves or rejects the User Story. If the User Story is rejected, it goes back for further review and documentation.
    5. If the review is approved, the Security Officer or Privacy Officer then marks the User Story as Closed, adding any pertinent notes required.
    6. Policy review is monitored on a yearly basis using the Azure DevOps Compliance Review Activity (CRA) Project to assess compliance with above policy.
7. NutriAdmin tracks compliance with HIPAA and publishes results at [https://nutriadmin.com/hipaa](https://nutriadmin.com/hipaa). In order to track and measure adherence on an annual basis, NutriAdmin uses the following process to track HIPAA audits, both full and interim:
    1. The Security Officer initiates the HIPAA audit activity by recording a User Story in the Azure DevOps Compliance Review Activity (CRA) Project.
    2. The Security Officer or the Privacy Officer is assigned to own and manage the HIPAA activity.
    3. Once the HIPAA activity is completed, the Security Officer approves or rejects the User Story.
    4. If the review is approved, the Security Officer then marks the User Story as Closed, adding any pertinent notes required.
    5. Compliance with annual compliance assessments is monitored on a quarterly basis using the Azure DevOps Compliance Review Activity (CRA) Project to assess compliance with above policy.

Additional documentation related to maintenance of policies is outlined in [§5.3.1](#5.3-security-officer).
