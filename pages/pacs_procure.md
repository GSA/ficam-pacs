---
layout: default
title: Procure an Approved PACS
permalink: /procure/
---
## Where Can I Find Information about GSA-Approved Products?

The General Services Administration (GSA) is responsible for ensuring that products comply with FIPS 201-2 requirements. Products are evaluated based on specific topologies (parameters) and the results are available on GSA's www.idmanagement.gov website: [FIPS 201 Evaluation Program](https://www.idmanagement.gov/fips201/){:target="_blank"} and [Approved Products List](https://www.idmanagement.gov/approved-products-list/){:target="_blank"}.  

## What Is a GSA APL-Listed PACS?

The current GSA APL practice approves three components of a complete, end-to-end PACS:

1. PACS infrastructure
2. Validation system
3. PIV reader  

Complete systems consist of components from all three categories and are integrated through software development kits (SDKs) or application programming interfaces (APIs).

A GSA APL-listed PACS is engineered by the manufacturer to achieve the goals and objectives outlined in HSPD-12.  The main objectives are:

* Detect a cloned, forged, or altered card and deny access
* Detect an invalid card and deny access
* Detect a valid card presented by a person other than the card owner and deny access
* Support non-proprietary card formats (FASC-N and UUID) by federal and specially accredited NFIs.

The tools required to achieve these objectives include PKI and related certificate validation services with interfaces to the Federal PKI and certificate authorities.  Only a small percentage of the approximately 150 PACS manufacturers have achieved compliance.

## Why Does My Agency Need This?

A legacy or other non-compliant PACS often relies on proprietary credential data models produced locally.  Non-FICAM-compliant systems typically use common card identifiers, such as 26-bit Wiegand.  The cards are susceptible to cloning, alteration, or duplication.  In addition, these cards are ordered from system providers and the encoding is proprietary.  The data encoded in the card is therefore recorded by several outside organizations.  With no encryption to prevent cloning, duplication, or alteration, a non-compliant PACS offers a relatively simple attack vector to an adversary trying to access a controlled area.

A FICAM-compliant system can mitigate attacks and ensure that only authentic and validated cards can be used.

## How Do I Know Whether This is a Compliant System?<!--How do I know whether a specific PACS is a compliant system?-->

A GSA-listed PACS is significantly different from a legacy or other non-compliant PACS. System hardware, firmware, and software (the PACS infrastructure) and readers support a certificate validation service.  The reader must support bidirectional communication between the card and the certificate validation service.  The certificate validation service interfaces with the Federal PKI and must validate a card before access can be authorized.

To ensure that all the cryptographic processes are executed as intended, the GSA FIPS 201 Evaluation Program has established end-to-end system testing procedures.  Only PACS that have passed the evaluation tests are included in the GSA [Approved Products List](https://www.idmanagement.gov/approved-products-list/){:target="_blank"}. The APL tests the following system components:
* PACS infrastructure
* PACS certificate validation service
* PACS readers

Each component is tested in a configuration specified by the PACS manufacturer, and each component has an APL approval number.

## What Other Considerations Do I Need To Be Aware of in Implementing a GSA APL-Listed PACS?

* Include in the scope of work (SOW) the location of each system component to be installed.<!--SOW = Statement of Work-->
* Secure the location for all system components.
* Coordinate with other organizations and service providers to make certain there is appropriate power for all system components.
* Ensure that network communication is available and secured according to local policies.

## How Do I Buy a Compliant PACS?

GSA has developed useful tools for both a procuring agency and an organization that is submitting a proposal or responding to a solicitation.

GSA publishes lists of [approved products and services](https://www.idmanagement.gov/buy/){:target="_blank"} and helpful links for purchasing these items using GSA schedules.

Another useful resource is the [PACS Ordering Guide](https://www.gsa.gov/cdnstatic/Guide_to_PACS_-_REVISED_060717.pdf){:target="_blank"}, a vendor-agnostic generic template that procurement and contract officers can use to write solicitations. The Guide explains various functions and FICAM compliance requirements.  It includes simple spreadsheets for use when responding to a proposal or writing one. Use the Guide to be confident that your proposed solution represents a compliant PACS.

## How Can I Identify Qualified FIPS 201 Service Providers?

FIPS 201 service providers must be certified under a federally recognized certification program such as the [Certified System Engineer ICAM PACS Training and Certification Program](https://www.securetechalliance.org/activities-certified-system-engineer-icam-pacs-training-and-certification-program/){:target="_blank"}<!--Replaced original broken link with current program name and website URL.-->.  

The GSA FIPS 201 Evaluation Program maintains a list of approved products and qualified service providers.  Additional details can be found at [GSA Buy Products and Services](https://www.idmanagement.gov/buy/){:target="_blank"}.<!--Corrected reference and GSA website name.-->
