---
layout: default
title: Types of Physical Access Control Systems
permalink: /pacs/
---

This page will give you a basic understanding of Physical Access Control Systems (PACSs) and Enterprise Physical Access Control Systems (E-PACSs). 

- [What Is a Physical Access Control System?](#what-is-a-physical-access-control-system)
- [What Is an Enterprise Physical Access Control System?](#what-is-an-enterprise-pacs)
- [Would an Enterprise Physical Access Control System Work for Our Agency?](#would-an-enterprise-pacs-work-for-our-agency)
- [What Are the Characteristics of a Federal Identity, Credential, and Access Management (FICAM)-Compliant PACS/E-PACS?](#characteristics-of-a-ficam-compliant-pacse-pacs)


## What Is a Physical Access Control System?

An agency's standalone PACS grants access to employees and contractors who work at or visit one site by authenticating their PIV credentials. Each site must manage its PACS locally, because the PACS is not connected to the agency’s enterprise network. 

The following table defines common PACS components: 

| **Component** | **Description** |
|----------------|----------|
| **Access point** | Entrance point, such as a credential reader, where an employee or contractor interacts with the PACS. The access point also includes barriers, such as turnstiles, gates, and locking doors. |
| **PIV credential** | Federal employees and contractors use [Personal Identity Verification (PIV) credentials](https://piv.idmanagement.gov/elements/){:target="_blank"}, also known as PIV cards, to *physically access* federal facilities and *logically access* federal information systems. |
| **Credential reader and keypad** | The reader provides power to and reads data from a PIV credential. The reader also sends this data to a control panel to authenticate the PIV credential and request access authorization. Employees and contractors may need to enter a PIN into the keypad and add a biometric, depending on the facility's security classification and risk levels. | 
| **Biometric reader** | Captures biometric data (for example, fingerprint or iris scan) and verifies it against the PIV credential's biometric data. |
| **Control panel** | Receives the credential data sent by the reader and verifies its presence in the credential-holder data repository. It then makes an access decision and transmits authorization data to the access control server and access point.  |
| **Access control server** | Grants authorization to the employee or contractor requesting access (for example, presenting a PIV credential to a reader). It also registers and enrolls employees and contractors; enrolls and validates credentials; and logs system events. |
| **Credential-<br>holder data repository** | Contains employee and contractor data and physical access privileges. Control panels use this authoritative data to validate credential data. |

{% include alert-info.html content="All agency-purchased PACS and E-PACS components must be FIPS 201-compliant and selected from <a href=\"https://www.idmanagement.gov/approved-products-list-pacs-products/\" target=\"_blank\">GSA's Approved Products List (APL) for PACS Products</a>. The products in this list have undergone vulnerability and interoperability testing through the FIPS 201 Evaluation Program." %}


### Some PACS' Operational Challenges

Agencies that use standalone PACSs have encountered operational challenges: 
* Sites must independently control physical access.
* Agencies see delays with credential transfers or terminations.
* Employees and contractors must re-enroll their credentials for all federal work sites that they visit.
* Departments inconsistently apply enterprise-wide security policies.
* Agencies experience reduced situational awareness (for example, logs cannot be correlated across the enterprise)
* Agencies with many standalone PACSs see increased human error, such as data entry errors.

{% include alert-success.html content="Can agencies centrally control physical access for most, or all, of their sites?  Yes - the answer is to implement an Enterprise Physical Access Control System." %}

## What Is an Enterprise PACS?

An Enterprise PACS extends the concept of a PACS to act as a unified, enterprise-wide system that controls physical access at most (or all) sites that belong to an agency. E-PACSs address the operational challenges of standalone PACSs and improve system management, scalability, monitoring, and performance. 

E-PACSs rely on the same components as standalone PACSs. However, an essential architectural distinction is that an E-PACS connects to an agency's enterprise-network, whereas a PACS typically does not.

{% include alert-info.html content="Some agencies need standalone PACSs for their unique sites and missions, but most agencies could benefit from transitioning to an E-PACS." %}

## Would an Enterprise PACS Work for Our Agency?

Here are some key E-PACS advantages to consider:

* One enterprise-wide system controls physical access for many (or all) agency sites
* One employee and contractor enrollment system that connects multiple enrollment locations
* One credential registration and provisioning point
* One enterprise-wide system for administrators to modify or terminate access privileges
* One enterprise-wide system that regularly polls for [Certificate Revocation List](https://piv.idmanagement.gov/pivcertchains/#revocation){:target="_blank"} (CRL) updates and maintains revocation data
* Reduced costs for system management, such as patching, server system administration, and software updates
* Reduced costs for reporting , such as Federal Information Security Modernization Act [FISMA] reporting
* Reduced costs for:
    * Server hardware
    * System security assessment and accreditation


## Characteristics of a FICAM-Compliant PACS/E-PACS
In February 2011, the Office of Management and Budget (OMB) issued memorandum [M-11-11](https://obamawhitehouse.archives.gov/sites/default/files/omb/memoranda/2011/m11-11.pdf){:target="_blank"} to lead Executive Departments and Agencies on the continued implementation of [HSPD-12](http://www.dhs.gov/homeland-security-presidential-directive-12){:target="_blank"}. M-11-11 also defined a partnership between DHS and GSA to provide agencies with guidance on the implementation of physical access requirements for Federal buildings per the DHS [Interagency Security Committee](https://www.dhs.gov/isc-policies-standards-best-practices){:target="_blank"} Standards and NIST guidelines (for example, [SP 800-116](https://csrc.nist.gov/publications/detail/sp/800-116/rev-1/final){:target="_blank"}, _A Recommendation for the Use of PIV Credentials in Physical Access Control Systems (PACS)_). 


Characteristics of NIST SP 800-116 compliant systems include, but are not limited to:
- Use high-assurance credentials for electronic authentication of employees and contractors
- Use non-deprecated authentication mechanisms, as defined by [FIPS 201-2](https://csrc.nist.gov/publications/detail/fips/201/2/final){:target="_blank"}
- Validate the status and authenticity of credentials
- Interoperate with PIV credentials issued by other agencies
- Use components listed on the GSA FIPS 201 Approved Products List (APL)
	
The next section, *[Aligning Facility Security Level (FSL) and Authentication]({{site.baseurl}}/alignfslandauth/)*, explains the processes needed to prepare for a PACS/E-PACS deployment and offers more detail related to the FIPS 201-approved PIV authentication mechanisms.
