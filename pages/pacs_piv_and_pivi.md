---
layout: default
title: PIV and PIV-I Considerations
permalink: /pivandpivi/
---

PIV and PIV-Interoperable (PIV-I) credentials are based on smart card technology. Smart cards incorporate a small computer chip in a card (or other form factor).  The embedded chip provides the card with built-in tamper resistance, the ability to store large amounts of data securely, data processing capability, and the ability to interact intelligently with a smart card reader. Smart cards can be used online and across networks and deliver very high levels of security over the Internet.  They are also convenient and easy to use.
Smart card technology can provide an identity management system or physical access control system with strong information and privacy protection.  A smart card-based ID can guard personal information and individual privacy by implementing a personal firewall, releasing only required information and only when it is genuinely required.

The PIV and PIV-I credentials include a dual-interface chip that supports both contact (ISO/IEC 7816-compliant) and contactless (ISO/IEC 14443-compliant) operations.

### What Is the Difference between PIV and PIV-I?

The Federal Government has issued well over 5 million PIV cards to employees and contractors.  Federal agencies use the PIV card to authorize employee access to both physical and logical resources and to assign access privileges.  The success of the program is largely due to the development of goals, issuance policies, and technical specifications that all Federal agencies have agreed to follow.  A cross-certification policy establishes trust between agencies; employees from one agency can use their PIV credentials to access controlled resources when visiting other agencies.  A variety of suppliers offer products and systems that conform to the technical interoperability standards. 

Interest in a common identity credential is growing among Non-Federal Issuers. PIV-I cards are already being issued by federal contractors to employees who need access to federal buildings and IT networks.  The PIV-I credential is technically interoperable with the government PIV systems (e.g., readers) and is issued in a way that allows government agencies to trust the card.  PIV-I credentials comply with Federal Bridge guidance on identity-proofing, registration, and issuance.  PIV-I credentials are cross-certified with the Federal Public Key Infrastructure (PKI) Bridge to allow contractor personnel, visitors, and personnel waiting for clearance to access authorized resources.  Table 4 compares the PIV and PIV-I cards.

Agency policy may dictate a background check before granting access to a PIV-I cardholder.

**Table 4. Comparison of PIV and PIV-I Cards**

#### POLICY
| **Q: What are these?** |  **PIV** | **PIV-I** | 
| :-------- | :------------ | :----------- | 
| Breeder documents  | Follows FIPS 201 |  Follows FIPS 201  | 
| Background checks  | National Agency check with investigation | None required |
#### PROCESS
| **Q: What are these?** |  **PIV** | **PIV-I** | 
| :-------- | :------------ | :----------- | 
| Application, Adjudication, Enrollment, Issuance, Activation  | Follows FIPS 201: separation of roles, strong biometric binding | Follows Federal Bridge cross-certification certificate policies. Follows NIST SP 800-63-1 for Federal issuance. Based on FIPS 201: separation of roles, strong biometric binding. |  
#### TECHNOLOGY
| **Q: What are these?** |  **PIV** | **PIV-I** | 
| :-------- | :------------ | :----------- | 
| Card data mode  | Must follow SP 800-73 | Must follow SP 800-73  | 
| Current primary credential number   | FASC-Nb (requires federal agency code) | UUID (no federal agency code required) | 
| Object identifiers  | Federal Bridge | Federal Bridge  | 
#### TYPES OF FEDERATION AND LEVELS OF ASSURANCE
| **Q: What are these?** |  **PIV** | **PIV-I** | 
| :-------- | :------------ | :----------- | 
| Trustworthiness   | Trusted identity, credential, and suitability | Trusted basic identity and credential but not suitability | 
| Trust among organizations   | Federal Bridge | Clustered through Federal Bridge | 
#### ORIGIN
| **Q: What are these?** |  **PIV** | **PIV-I** | 
| :-------- | :------------ | :----------- | 
| Organization   | NIST Federal | CIO Council | 
| Defining documents   | FIPS 201, FIPS 201-2, NIST SP 800-73 and other related NIST publications | Personal Identity Verification Interoperability for NFIs(1)<br>FICAM PIV-I FAQ(2) | 
| Motivation | HSPD-12 | Interoperable credential for organizations doing business with the government and for first responders |
#### MARKETS
| **Q: What are these?** |  **PIV** | **PIV-I** | 
| :-------- | :------------ | :----------- | 
| Organizations that may issue and/or use the credential  | Federal agencies | Federal agencies<br>Federal contractors<br>Commercial organizations doing business with the Federal Government<br>State and local governments<br>Critical infrastructure providers<br>First responder organizations<br>Commercial organizations who are part of an industry initiative and require an interoperable, trusted credential | 
| Use  | Credential can be used in a wide range of both employment-related and consumer-based transactions.  Examples include physical access, logical access,e mass transit, and closed loop payments. | Same as for PIV





