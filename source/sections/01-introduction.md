# 1. Introduction

NutriAdmin, owned by Magosoft Ltd ("NutriAdmin") is committed to ensuring the confidentiality, privacy, integrity, and availability of all electronic protected health information (ePHI) it receives, maintains, processes and/or transmits on behalf of its Customers. As providers of compliant, hosted software used by nutritionists, dietitians, health coaches, personal trainers, fitness professionals, health and medical professionals, NutriAdmin strives to maintain compliance, proactively address information security, mitigate risk for its Customers, and assure known breaches are completely and effectively communicated in a timely manner. The following documents address core policies used by NutriAdmin to maintain compliance and assure the proper protections of infrastructure used to store, process, and transmit ePHI for NutriAdmin Customers.

NutriAdmin provides secure and compliant cloud-based software. This hosted software falls into one broad category: **Software as a Service (SaaS)**. This Category is cited throughout polices as either *Software as a Service* or *SaaS* for short.

## 1.1 Attributtion

NutriAdmin's policies are based on [Datica's policies](https://github.com/catalyzeio/policies). Datica's policies have been used as a template to create NutriAdmin's policies – as allowed by their license. All policies are licensed under [CC BY-SA 4.0](http://creativecommons.org/licenses/by-sa/4.0/).

## 1.2 Software as a Service (SaaS)

SaaS Customers utilize hosted software and infrastructure from NutriAdmin to manage their nutrition practice and clients/patients or nutrition-related businesses. These customers make use of software running in compliant hosting. NutriAdmin makes every effort to reduce the risk of unauthorized disclosure, access, and/or breach of SaaS Customer data through network (firewalls, network security groups, etc) and server settings (encryption at rest and in transit, OSSEC throughout the Platform, etc).

## 1.3 NutriAdmin Organizational Concepts

The physical infrastructure environment is hosted at [Microsoft Azure](https://azure.microsoft.com/). The network components and supporting network infrastructure are contained within Azure infrastructure and managed by Microsoft. NutriAdmin does not have physical access into the network components. The NutriAdmin environment consists of nginx web servers; NodeJs application servers; MongoDb database servers; Logstash logging servers; Linux Ubuntu servers; OSSEC IDS services; and developer/support tool servers running on Linux Ubuntu.

Within the NutriAdmin Platform on Azure, all data transmission is encrypted and all hard drive partitions containing ePHI are encrypted so data at rest is also encrypted; this applies to all servers - those hosting databases, logs, application servers, etc.

NutriAdmin has implemented strict logical access controls so that only authorized personnel are given access to the internal management servers. The environment is configured so that data is transmitted from the web server to the application server over a TLS encrypted session.

Access to the internal database is restricted to a limited number of personnel and strictly controlled to only those personnel with a business-justified reason.

## 1.5 Version Control

Refer to the GitHub repository at [https://github.com/Nutriadmin/policies/](https://github.com/Nutriadmin/policies/) for the full version history of these policies.
