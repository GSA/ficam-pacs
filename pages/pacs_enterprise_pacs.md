---
layout: default
title: Understand Enterprise PACS
permalink: /enterprisepacs/
---

New title: Understand Enterprise PACS (Original title:  Understanding Enterprise PACS and Security Functions)

### The Current State of PACS in Government

Individual PACS are often part of a local “security” network (not the enterprise network), along with cameras, intrusion detection sensors, and other security devices.  In some cases, the PACS is not connected to any network.  As a result, different brands of PACSs or even multiple PACSs that are the same brand, are individually administered with little thought given to unifying security policies enterprise-wide.

This lack of coordination increases risk to the enterprise and operational costs. 

Traditionally, physical security has focused on one site at a time, without regard to overall use.  Government employees and contractors often must travel to or work in different buildings as part of their employment.  Common practice is to enroll the individual’s PIV card in each standalone PACS and provide access authorizations (also called entitlements or privileges) at enrollment.  One problem is that subsequent changes to access authorizations are made manually.  But the biggest problem is that privileges may not be terminated when a PIV card or other credential is no longer valid.

For a variety of reasons, some agencies have undertaken efforts to network their PACSs into a coherent, centrally managed system.  

### What Is an Enterprise PACS?

“Enterprise PACS” refers to the concept of connecting the PACS to the owners’ enterprise network leveraging the FICAM infrastructure to support strong authentication using the PIV card.  An enterprise PACS provides one access control environment that can be shared and managed centrally.  For more information see Chapter 10, page 313, of “The Federal Identity Credential and Access Management (FICAM) Roadmap and Guidance,” Version 2.0 (the FICAM Roadmap), which details the notional architecture and components of an enterprise PACS environment (Figure 1).

### Current Government Directives for an Enterprise PACS

**INSERT IMAGE HERE:** **Is this Figure 1. Architecture and Components of an Enterprise PACS Environment?** <!--"Enterprise PACS Management System" shown next to figure. Caption was separated from figure.-->

Authoritative sources are connected to an in-place PACS over what is called the External Interface/Cardholder Provisioning System or a Centralized Enterprise PACS Management System.  An Enterprise PACS management system can help reduce human error, reduce costs, and provide a unified view of all identities and their privileges.

### Prerequisites for an Enterprise PACS

In order to unify PACSs, each system must either be part of the organization’s enterprise network or have a network connection.  The security department that manages the PACS must work with the organization’s IT department to obtain an Authority To Operate (ATO).  The ATO process can be costly and tedious and involves each PACS vendor, who may need to update or patch its software to fix security flaws.  The more PACSs involved, the more funding required.

One way to mitigate cost is to deploy an enterprise PACS management system on the enterprise network, obtain the ATO for that system, and then connect each individual PACS to the management system with a point-to-point link, such as a point-to-point VPN.  This strategy is subject to a department’s or agency’s FISMA policy interpretation for security boundary control.

Another variant is to deploy the enterprise PACS management system in a Federal Risk and Authorization Management Program (FEDRAMP) HIGH secure cloud and interconnect each PACS and authoritative source to that environment.  This solution is also subject to the FISMA controls implemented at the agency.

### Vital Security Functions Performed by an Enterprise PACS Management System

The purpose of any access control system is to make sure the right person has the right access at the right time for the right reason.  Ultimately, some person or system needs to provision the “right” access levels.  Provisioning means specifying for each identity both the credential used (PIV card in government) and the privileges granted to access specific resources, such as a particular facility, door, or portal.  Correct provisioning can sometimes mean ensuring that a complex set of rules is enforced.  As such, this provisioning process is a vital security function.

Three security functions are fundamental to an enterprise PACS:

* **Authentication.** Authentication of the PIV card and the controls on it.
* **Authorization.** Just because someone has an authentic high assurance credential (such as a PIV card or Common Access Card (CAC)) does not mean that person should be able to access every resource.  Authorizing access only to the resources each person needs to perform a job is paramount to controlling risk.  In a large enterprise with thousands of employees and contractors needing access to thousands of physical access points, attempting to manage authorization manually is costly and error-prone.  Some form of policy-based automated authorization process is needed.
* **Audit.** Compliance to policy must be measured and monitored and violations or defects mitigated.  It is almost impossible to audit authentication and authorizations for every individual without an enterprise PACS management system.

Figure 2, from Chapter 4, page 102, of the FICAM Roadmap, illustrates these concepts.

**INSERT IMAGE HERE:** **Figure 2. FICAM Architecture and Flow for Electronically Automated Provisioning and Access Authorization with Audit Capabilitie** 

Authoritative sources (Active Directory, PIV card database, personnel security system, other identity management systems (IDMS)) are connected to the enterprise PACS management system and automatically add new identities and remove terminated identities.  Most IDMS sources include an application programing interface (API) that allows external systems to access identity information.  The enterprise PACS management system should use that API to provide a near real-time interface, so that new identities are added within minutes.  Any changes to identity attribute data are similarly synchronized between the specific authoritative source and the enterprise PACS management system. This timely synchronization ensures that policy decisions regarding access can be implemented immediately.

Requested changes to access are submitted electronically (for example, through a self-service portal). The enterprise PACS management system registers the new or modified access privileges in the affected PACS as directed by your agency’s business rules.  Such rules could include enforced compliance with prerequisites such as achievement of a certain training level or an electronically auditable approval process.

Another key component is the audit trail.  It is vital to record who approved an access request, what conditions were met, and other policy or process data.  A record of access privilege changes over time is also important, for lifecycle audits.  An additional required audit is the attestation audit.  For high security access points or exclusion zones, many organizations require ongoing periodic audits by an access “owner” to maintain ongoing access.  The final audit determines whether access was granted manually through a back-door process, such as a privileged PACS admin user logging directly into a specific PACS and provisioning cards or granting access outside of policy.  The ability to detect, report, and even automatically remand such errant access is part of the audit function.  The enterprise PACS management system should address all these requirements.

The enterprise PACS management system should be able to support these functions not only for federal employees, long-term contractors and visitors from other agencies (PIV cardholders), but also for shorter-term contractors (non-PIV cardholders).  Agencies may consider issuing a _Commercial Identity Verification (CIV)_ card for the latter or validate and enroll a non-agency PIV card for the former and perform these authentication, authorization and audit functions.  The CIV card, which the agency may issue, shall support the GSA APL-approved PACS that can authenticate the card at the time of use.

### Implementation Guidance for an Enterprise PACS Management System

According to 41 USC &sect; 3307, preference for commercial items is U.S. law.  Federal Acquisition Regulation, subpart 44.4, reiterates that contractors must supply commercial off-the-shelf (COTS) products to the maximum extent possible.  With these requirements in mind, your agency should first investigate whether a COTS software product exists that can serve as an enterprise PACS management system.  In-house software development should be a last resort.

Because an enterprise PACS management system interfaces with so many other systems that are owned or managed by different departments (such as human resources, IT, facilities security), it is imperative for all stakeholders to understand all requirements and implement properly. (The ideal governance for this process is a FICAM program management office.)  All stakeholders can benefit from the implementation of an enterprise PACS management system and should be motivated to provide guidance to the implementation group within your agency.  
