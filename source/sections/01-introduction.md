# 1. Introduction

NutriAdmin, owned by Magosoft Ltd ("NutriAdmin") is committed to ensuring the confidentiality, privacy, integrity, and availability of all electronic protected health information (ePHI) it receives, maintains, processes and/or transmits on behalf of its Customers. As providers of compliant, hosted software used by nutritionists, dietitians, health coaches, personal trainers, fitness professionals, health and medical professionals, NutriAdmin strives to maintain compliance, proactively address information security, mitigate risk for its Customers, and assure known breaches are completely and effectively communicated in a timely manner. The following documents address core policies used by NutriAdmin to maintain compliance and assure the proper protections of infrastructure used to store, process, and transmit ePHI for NutriAdmin Customers.

NutriAdmin provides secure and compliant cloud-based software. This hosted software falls into one broad category: **Software as a Service (SaaS)**. This Category is cited throughout polices as either *Software as a Service* or *SaaS* for short.

## 1.1 Attributtion

NutriAdmin's policies are based on [Datica's policies](https://github.com/catalyzeio/policies). Datica's policies have been used as a template to create NutriAdmin's policies – as allowed by their license. All policies are licensed under [CC BY-SA 4.0](http://creativecommons.org/licenses/by-sa/4.0/).

## 1.2 Software as a Service (SaaS)

SaaS Customers utilize hosted software and infrastructure from NutriAdmin to manage their nutrition practice and clients/patients or nutrition-related businesses. These customers make use of software running in compliant hosting. NutriAdmin makes every effort to reduce the risk of unauthorized disclosure, access, and/or breach of SaaS Customer data through network (firewalls, network security groups, etc) and web-app/database settings (encryption at rest and in transit, etc).

## 1.3 NutriAdmin Organizational Concepts

The physical infrastructure environment is hosted at [Microsoft Azure](https://azure.microsoft.com/). The network components and supporting network infrastructure are contained within Azure infrastructure and managed by Microsoft. NutriAdmin does not have physical access into the network components. The NutriAdmin environment consists mainly of Azure Web Apps, a CosmosDB database, Azure Logging, and an Application Gateway. We use Azure compliant managed solutions like Web-Apps as opposed to hosting custom servers when possible. This delegates many security considerations (e.g. physical safeguards) to Microsoft, who offers security guarantees.

Within the NutriAdmin Platform on Azure, data transmission over the internet is encrypted, and data transmission within our private networks is also encrypted when deemed appropriate and reasonable. All hard drive partitions, databases, or blob storage containing ePHI are encrypted so data at rest is also encrypted; this applies to our CosmosDb account where the bulk of all the ePHI we manage is stored.

NutriAdmin has implemented strict logical access controls so that only authorized personnel are given access to the infrastructure. The environment is configured so that data is transmitted from the web server to the application server over a TLS encrypted session.

Access to the internal database is restricted to a limited number of personnel and strictly controlled to only those personnel with a business-justified reason.

## 1.4 Summary of NutriAdmin infrastructure

NutriAdmin aims to use managed solutions from Microsoft that are covered under their HIPAA BAA with NutriAdmin. This abstracts away the burden of many of the physical and organizational security measures required for production systems and effectively delegates it to Microsoft. For example, NutriAdmin uses a managed database (CosmosDB) as opposed to hosting a custom solution. Microsoft offers many guarantees under SLAs and the HIPAA BAA regarding this database.

In terms of physical infrastructure, NutriAdmin only owns workstations (e.g. laptops, desktop computers, smartphones). All production systems that may contain ePHI are hosted by Microsoft Azure. NutriAdmin systems do not store or maintain ePHI, and they may only rarely have access to ePHI when working to resolve a technical support issue as requested by a SaaS customer.

## 1.5 Version Control

Refer to the Azure DevOps repository at [https://dev.azure.com/nutriadmin/NutriAdmin%20Policies](https://dev.azure.com/nutriadmin/NutriAdmin%20Policies) for the full version history of these policies.
