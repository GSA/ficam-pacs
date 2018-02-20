---
layout: default
title: Deploy a PACS
permalink: /deploy/
---
Before deploying a PACS, be sure you have read the prerequisites for an Enterprise PACS.

### What Information Security Standards and Guidelines Apply to the PACS?

PACS are now considered part of federal IT infrastructure and are subject to numerous federal information security policies.

[FIPS Publication 200, _Minimum Security Requirements for Federal Information and Information Systems_](https://csrc.nist.gov/publications/detail/fips/200/final){:target="_blank"} is a mandatory federal standard developed by NIST in response to the Federal Information Security Modernization Act of 2014.<!--Corrected "Management" (FISMA of 2002 acronym) to "Modernization" (FISMA of 2014 changed acronym)-->  To comply with the federal standard: 
* Use [FIPS Publication 199, _Standards for Security Categorization of Federal Information and Information Systems_](https://csrc.nist.gov/csrc/media/publications/fips/199/final/documents/fips-pub-199-final.pdf){:target="_blank"} to determine the security category applicable to your information system.
* Determine the information system impact level in accordance with FIPS 200.
* Apply the appropriately tailored set of baseline security controls as described in [NIST SP 800-53, Revision 4](http://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-53r4.pdf){:target="_blank"}.  

FIPS Publication 199<!--Moved title to 1st FIPS PUB 199 reference above-->establishes security categories for information and information systems.  The security categories are based on the potential impact on an organization of events that jeopardize the information and information systems needed by the organization to accomplish its assigned mission, protect its assets, fulfill its legal responsibilities, maintain its day-to-day functions, and protect individuals.  Security categories are to be used in conjunction with vulnerability and threat information to assess the risk to an organization.
NIST Special Publication 800-53 rev 4, “Recommended Security Controls for Federal Information Systems and Organizations,” defines controls that facilitate compliance with all applicable Federal legal requirements.  Compliance requires organizations to perform due diligence with regard to information security and risk management.  The controls establish security due diligence for the organization.
The guidance provided in Special Publication 800-53 allows you to tailor the relevant security controls to more closely align with your mission, business requirements, and operational environment.
NIST Special Publication 800-171, "Protecting Controlled Unclassified Information in Nonfederal Information Systems and Organizations," recommends requirements for protecting the confidentiality of controlled unclassified information (CUI) in two situations: 
When the CUI is included in a nonfederal information system operated by contractors to Federal agencies or other organizations on behalf of those agencies
When the authorizing law, regulation, or government-wide policy prescribes no specific requirements for protecting the confidentiality of CUI in that particular category.  
The requirements apply only to components of nonfederal information systems that process, store, or transmit CUI or that provide security protection for such components.  
Federal agencies should adhere to the CUI requirements in appropriate contractual vehicles including Federal Acquisition Regulations (FAR) or other agreements established between their agency and nonfederal organizations.  Federal agencies using Federal information systems to process, store, or transmit CUI must also comply with FIPS 200, FIPS 199, NIST SP 800-53, and NIST SP 800-60, “Guide for Mapping Types of Information and Information Systems to Security Categories.”

