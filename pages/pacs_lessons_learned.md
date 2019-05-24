---
layout: default
title: Lessons Learned
permalink: /lessonslearned/
---

{% include alert-info.html content="\"PACS\" and \"E-PACS\" are used interchangeably in this section." %}

Federal agencies have shared these PACS lessons learned:

## Planning
- Identify all stakeholders upfront, to include an Executive Sponsor.
- Designate staff to fill key roles, such as architects, engineers, and operators.
- Engage CIO/CISO representatives early. _Remember: A PACS is an IT System._
- As an IT system, a PACS must complete Certification and Accreditation and obtain an Authority to Operate before connecting to the network.
- Create, maintain, and share an integrated master schedule that presents project phases, tasks, resources, and dependencies.
- Build the cost of software licensing and system sustainment into your project budget.
- Work with facility engineers to identify constraints specific to your workplace, such as mandatory construction requirements. These constraints may limit solution offerings.
- Legacy system hardware, such as credential readers, may not support FICAM compliant modes of operation. (FICAM Mode implies using PKI-based authentication mechanisms and online identity validation.) Review your system hardware capabilities after identifying desired authentication mechanisms to determine if upgrades are necessary. 
- Utilize legacy credentials and non-FICAM compliant modes of operation *only* in a migration strategy, not as the end state.
- Retire and phase out secondary, legacy credentials.
- Use your agency Identity Management System as the canonical source for all user records in the PACS.
- Some PACS allow user access levels to be assigned at the time of credential registration. Plan the method of assignment before provisioning/registration.
- Avoid acts of “omission” that create non-compliance. For example, procuring products listed on the Approved Products List (APL) but not correctly enabling FICAM Mode.
- Understand that PKI is the foundation for high assurance PACS implementations.


## Procurements
- Do not procure non-compliant PACS technologies, such as proximity cards.
- Use consistent terms and recommended procurement language within requirements documents, specifications, SOWs, RFIs, RFPs, and RFQs. 
- Leverage agency subject matter experts to review SOWs, RFPs, and RFQs before releasing them for contractors' bids.
- Resolve SOW and PACS compliance issues as soon as they are recognized.
- Work closely with agency legal team members to define a SOW that contains unambiguous responsibilities for the integrator and appropriate cures for non-performance.
- Have your integrator provide copies of all relevant FIPS 201-2 compliance and functionality testing documentation.
- Specify personnel roles, responsibilities, and training requirements within the SOW (for example, all engineers must be CSEIP certified.)
- Ensure qualified professionals and/or subject matter experts review the design documents before releasing them for bid or formal contractor response. Consider hiring an SME capability to augment agency staff as a "buyer’s agent" during these activities.
- Consider looking for evidence of qualified and/or registered personnel certifying the proposed solution (submittals) prior to approval or notice to proceed.


## Operations
- Ensure the PACS is configured and maintained to operate in FICAM Mode. 
- Work with your IT Department to ensure your PACS can perform online certificate validation. If your PACS is limited to offline certificate validation, manually load CRLs and certificate trust lists into the PACS daily.
- Provision only assured identities from an agency authoritative source into your PACS.
- For any PIV credential that becomes invalid (expired, certificates placed on CRL, etc.), the PACS administrator may wish to disable the credential in the PACS immediately, rather than waiting for it to happen automatically through the routine credential validation process.  Consider disabling identity and credential records rather than removing them to retain audit data that might be needed at a later time (for example, employee misconduct investigations).
- To protect privacy, remove all PII from PACS endpoints.
- Audit expected system functionality on a regular basis.  Minimally, verify that access points are challenging the correct number and type of authentication factors. Consider using test credentials which have expired or been revoked to further ensure correct operation.


## Training
- Create and maintain a training plan that formally documents training requirements.
- Provide role-specific training to agency stakeholders, such as HR, IT, or Security.

The next section, [Standards, Policies, and Guidance]({{site.baseurl}}/standards/) lists relevant public law, policies, regulations, standards, guidance, and publications relevant to PACS/E-PACS.
