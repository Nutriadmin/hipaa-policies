# 7. System Access Policy

Access to NutriAdmin systems and application is limited for all users, including but not limited to workforce members, volunteers, business associates, contracted providers, consultants, and any other entity, is allowable only on a minimum necessary basis. All users are responsible for reporting an incident of unauthorized user or access of the organization's information systems. These safeguards have been established to address the HIPAA Security regulations including the following:

## 7.1 Applicable Standards from the HIPAA Security Rule

* 164.308a4iiC Access Establishment and Modification
* 164.308a3iiB Workforce Clearance Procedures
* 164.308a4iiB Access Authorization
* 164.312d Person or Entity Authentication
* 164.312a2i Unique User Identification
* 164.308a5iiD Password Management
* 164.312a2iii Automatic Logoff
* 164.310b Workstation Use
* 164.310c Workstation Security
* 164.308a3iiC Termination Procedures

## 7.2 Access Establishment and Modification

1. Requests for access to NutriAdmin Platform systems and applications is made formally using the following process:
    1. A NutriAdmin workforce member initiates the access request by emailing the Security Officer or Privacy Officer.
    2. The Security Officer or Privacy Officer creates a Task Compliance Review Activity (CRA) Spreadsheet with ID #CRA-9.
     * User identities must be verified prior to granting access to new accounts.
     * Identity verification must be done in person where possible; for remote employees, identities must be verified over the phone.
     * For new accounts, the method used to verify the user's identity must be recorded on the notes for the task.
    2. The Security Officer or Privacy Officer will grant access to systems as dictated by the employee's job title. If additional access is required outside of the minimum necessary to perform job functions, the requester must include a description of why the additional access is required as part of the access request.
    3. Once the review is completed, the Security Officer or Privacy Officer approves or rejects the Task. If the Task is rejected, it goes back for further review and documentation.
    4. If the review is approved, the Security Officer or Privacy Officer then marks the Task as Done, adding any pertinent notes required. The Security Officer or Privacy Officer then grants requested access.
     * New accounts will be created with a temporary secure password that meets all requirements from [§7.12](#7.12-password-management), which must be changed on the initial login.
     * All password exchanges must occur over an authenticated channel.
     * For production systems, access grants are accomplished by adding the appropriate user account to the corresponding LDAP group.
     * For non-production systems, access grants are accomplished by leveraging the access control mechanisms built into those systems. Account management for non-production systems may be delegated to a NutriAdmin employee at the discretion of the Security Officer or Privacy Officer.
2. Access is not granted until receipt, review, and approval by the NutriAdmin Security Officer or Privacy Officer ;
3. The request for access is retained for future reference.
4. All access to NutriAdmin systems and services are reviewed and updated on an annual basis to ensure proper authorizations are in place commensurate with job functions. The process for conducting reviews is outlined below:
   1. The Security Officer initiates the review of user access by creating a Task in the Compliance Review Activity (CRA) Spreadsheet with ID #CRA-10.
   2. The Security Officer is assigned to review levels of access for each NutriAdmin workforce member.
   3. If user access is found during review that is not in line with the least privilege principle, the process below is used to modify user access and notify the user of access changes. Once those steps are completed, the activity is then reviewed again.
   4. Once the review is completed, the Security Officer approves or rejects the Task. If the Task is rejected, it goes back for further review and documentation.
   5. If the review is approved, the Security Officer then marks the Task as Done, adding any pertinent notes required.
   6. Review of user access is monitored on an annual basis using the Compliance Review Activity (CRA) Spreadsheet to assess compliance with above policy. This monitoring activity is recorded using ID #CRA-11.
5. Any NutriAdmin workforce member can request change of access using the process outlined in [§7.2 paragraph 1](#7.2-access-establishment-and-modification).
6. Access to production systems is controlled using centralized user management and authentication.
7. Temporary accounts are not used unless absolutely necessary for business purposes. Temporary accounts are deleted as soon as they are no longer needed.
8. Privileged users must first access systems using standard, unique user accounts before switching to privileged users and performing privileged tasks.
   * For production systems, this is enforced by creating non-privileged user accounts that must invoke `sudo` to perform privileged tasks.
   * Rights for privileged accounts are granted by the Security Officer or Privacy Officer using the process outlined in [§7.2 paragraph 1](#7.2-access-establishment-and-modification).
9. Access is granted through SSH that utilizes two-factor authentication.
    * Two-factor authentication is accomplished using a Time-based One-Time Password (TOTP) as the second factor.
    * SSH sessions are automatically disconnected after 30 minutes of inactivity.
10. In cases of increased risk or known attempted unauthorized access, immediate steps are taken by the Security and Privacy Officer to limit access and reduce risk of unauthorized access.
11. Direct system to system, system to application, and application to application authentication and authorization are limited and controlled to restrict access.

## 7.3 Workforce Clearance

1. The level of security assigned to a user to the organization's information systems is based on the minimum necessary amount of data access required to carry out legitimate job responsibilities assigned to a user's job classification and/or to a user needing access to carry out treatment, payment, or healthcare operations.
2. All access requests are treated on a "least-access principle."
3. NutriAdmin maintains a minimum necessary approach to access to Customer data.

## 7.4 Access Authorization

1. Role based access categories for each NutriAdmin system and application are pre-approved by the Security Officer, or an authorized delegate of the Security Officer.
2. NutriAdmin utilizes firewalls to segment data, prevent unauthorized access, and monitor traffic for denial of service attacks.

## 7.5 Person or Entity Authentication

1. Each workforce member has and uses a unique user ID and password that identifies him/her as the user of the information system.
2. Each Customer and Partner has and uses a unique user ID and password that identifies him/her as the user of the information system.
3. All Customer support desk interactions must be verified before NutriAdmin support personnel will satisfy any request having information security implications.
   * Support issues submitted via NutriAdmin's dashboard require that users authenticate with their NutriAdmin account before submitting support tickets. The support team can clearly verify that a user is authenticated when submitting a support request.
   * Support issues submitted by email must be verified by NutriAdmin personnel. This verification involves confirming that the email address of the sender matches the email address of the registered NutriAdmin account.


## 7.6 Unique User Identification

1. Access to the NutriAdmin Platform systems and applications is controlled by requiring unique User Login IDs and passwords for each individual user and developer.
2. Passwords requirements mandate strong password controls (see below).
3. Passwords are not displayed at any time and are not transmitted or stored in plain text.
4. Default accounts on all production systems, including root, are disabled.
5. Shared accounts are not allowed within NutriAdmin systems or networks unless entirely necessary to conduct normal business practices. In those instances, the sharing will be granted amongst the minium number of workforce members required.

## 7.7 Automatic Logoff

1. Users are required to make information systems inaccessible by any other individual when unattended by the users (ex. by using a password protected screen saver or logging off the system).
2. Information systems automatically log users off the systems, or locks the session (requiring a password to login again) after 15 minutes of inactivity.
3. The Security Officer pre-approves exceptions to automatic log off requirements. These exceptions are recorded in the "Automatic Log-off exceptions" document.

## 7.8 Employee Workstation Use

All workstations at NutriAdmin are company owned, and all are either laptop Apple products running Mac OSX, One Plus smartphones running Android, or Desktops running Windows 10. The complete list of these devices, as well as relevant security details is maintained in the "Company owned devices" spreadsheet by the Security Office. The list of assets is also reviewed yearly during the Security Risk Assessment. This spreadsheet is updated when new devices are introduced or significant changes are made to existing devices. The spreadsheet and associated devices are monitored yearly and this monitoring activity is tracked on the Compliance Review Activity (CRA) spreadsheet with ID #CRA-29. 

1. Workstations may not be used to engage in any activity that is illegal or is in violation of organization's policies.
2. Access may not be used for transmitting, retrieving, or storage of any communications of a discriminatory or harassing nature or materials that are obscene or "X-rated". Harassment of any kind is prohibited. No messages with derogatory or inflammatory remarks about an individual's race, age, disability, religion, national origin, physical attributes, sexual preference, or health condition shall be transmitted or maintained. No abusive, hostile, profane, or offensive language is to be transmitted through organization's system.
3. Information systems/applications also may not be used for any other purpose that is illegal, unethical, or against company policies or contrary to organization's best interests. Messages containing information related to a lawsuit or investigation may not be sent without prior approval.
4. Solicitation of non-company business, or any use of organization's information systems/applications for personal gain is prohibited.
5. Transmitted messages may not contain material that criticizes the organization, its providers, its employees, or others.
6. Users may not misrepresent, obscure, suppress, or replace another user's identity in transmitted or stored messages.
7. Workstation hard drives will be encrypted using FileVault 2.0 (for Mac), Bitlocker (in the case of Windows 10), or equivalent.
8. All workstations have firewalls enabled to prevent unauthorized access unless explicitly granted.
9. All workstations are to have the following messages added to the lock screen and login screen: *This computer is owned by NutriAdmin (Magosoft Ltd). By logging in, unlocking, and/or using this computer you acknowledge you have seen, and follow, these policies (https://dev.azure.com/nutriadmin/NutriAdmin%20Policies) and have completed this training (https://nutriadmin.com/training). Please contact us if you have problems with this - diego@nutriadmin.com*

## 7.9 Wireless Access Use
			
1. NutriAdmin production systems are not accessible directly over wireless channels.
2. Wireless access is disabled on all production systems.
3. When accessing production systems via remote wireless connections, the same system access policies and procedures apply to wireless as all other connections, including wired.
4. Wireless networks managed within NutriAdmin non-production facilities (offices, etc.) are secured with the following configurations:
   * All data in transit over wireless is encrypted using WPA2 encryption;
   * Passwords are rotated on a regular basis, presently annually. This process is managed by the NutriAdmin Security Officer. This Task is tracked in the Compliance Review Activity (CRA) Spreadsheet with ID #CRA-28.

## 7.10 Employee Termination Procedures

1. The Human Resources Department (or other designated department), users, and their supervisors are required to notify the Security Officer upon completion and/or termination of access needs.
2. The Human Resources Department, users, and supervisors are required to notify the Security Officer to terminate a user's access rights if there is evidence or reason to believe the following (these incidents are also reported on an incident report and is filed with the Privacy Officer):
   * The user has been using their access rights inappropriately;
   * A user's password has been compromised (a new password may be provided to the user if the user is not identified as the individual compromising the original password);
   * An unauthorized individual is utilizing a user's User Login ID and password (a new password may be provided to the user if the user is not identified as providing the unauthorized individual with the User Login ID and password).
3. The Security Officer will terminate users' access rights immediately upon notification, and will coordinate with the appropriate NutriAdmin employees to terminate access to any non-production systems managed by those employees.
4. The Security Officer audits and may terminate access of users that have not logged into organization's information systems/applications for an extended period of time.

## 7.11 Paper Records

NutriAdmin does not use paper records for any sensitive information. Use of paper for recording and storing sensitive data is against NutriAdmin policies.

## 7.12 Password Management

1. User IDs and passwords are used to control access to NutriAdmin systems and may not be disclosed to anyone for any reason.
2. Users may not allow anyone, for any reason, to have access to any information system using another user's unique user ID and password.
3. On all production systems and software used by NutriAdmin personnel for work-related purposes, password configurations require:
   * a minimum length of 8 characters;
   * a mix of upper case characters, lower case characters, and numbers or special characters (if permitted by the system);
   * for production servers, rules are in place to enforce users changing password at least every 365 days.
4. All system and application passwords must be stored and transmitted securely.
   * Where possible, passwords should be stored in a hashed format.
   * Passwords that must be stored in non-hashed format must be encrypted at rest pursuant to the requirements in [§17.8](#17.8-production-data-security).
   * Transmitted passwords must be encrypted in flight pursuant to the requirements in [§17.9](#17.9-transmission-security).
6. Passwords are inactivated immediately upon an employee's termination (refer to the [Employee Termination Procedures in §7.10](#7.10-employee-termination-procedures)).
7. All default system, application, and Partner passwords are changed before deployment to production.
8. Upon initial login, users must change any passwords that were automatically generated for them.
9. Password change methods must use a confirmation method to correct for user input errors where possible.
10. All passwords used in configuration scripts are secured and encrypted.
11. If a user believes their user ID has been compromised, they are required to immediately report the incident to the Security Office.
12. In cases where a user has forgotten their password, the following procedure is used to reset the password.
    * The user submits a password reset request to diego@nutriadmin.com. The request should include the system to which the user has lost access and needs the password reset.
    * An administrator with password reset privileges is notified and connects directly with the user requesting the password reset.
    * The administrator verifies the identity of the user either in-person or through a separate communication channel such as phone or email.
    * Once verified, the administrator resets the password.

The password-reset email inbox (currently diego@nutriadmin.com) is used to track and store password reset requests. The Security Officer is the owner of this email address and modifies membership as needed.

## 7.13 Access to ePHI

1. Employees may not download ePHI to any workstations used to connect to production systems.
    - An exception to this rule is when, as part of resolving a technical support issue for a Customer, it is required to download some data in order to test data downloading functionality in the software. In these circumnstances, approval from the Customer must be obtained in writing (e.g. email), and the minimum amount of data required to resolve the support issue should be downloaded. The workstation's disk where data will be download must be encrypted, and the data must be securely destroyed as soon as the support issue is resolved, or as soon as the data is no longer needed to fix the support issue. Under no circumstances will this data be shared outside to any third parties without prior consent from the owner of the data.
