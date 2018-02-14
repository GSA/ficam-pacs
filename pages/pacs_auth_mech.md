---
layout: default
title: Select Authentication Mechanism
permalink: /authmech/
---

## Selecting the Appropriate Authentication Mechanism 

In order to determine how many factors of authentication are required, a risk analysis should be conducted for each access point (door). The diagram below outlines the multi-step process for selecting which mechanism to use for authentication.  At a minimum, the process includes four steps:

**INSERT IMAGE**; Caption = Authentication Mechanism Selection Process

1. **Asset Risk Assessment.** The first step is to evaluate the likelihood and effect of losing or compromising each asset within a security area. If the likelihood is high or the impact is substantial, then categorize the risk to that asset as HIGH.  Other assets may have LOW or MODERATE risk.

2. **Security Area Categorization.**  Next, assign to the security area the same risk level as the highest risk asset within the area.  For example, say there are three assets within a designated security area:  a LOW-risk asset, a MODERATE-risk asset, and a HIGH-risk asset.  The security area must be classified as a HIGH-risk security area.  As an alternative, split the security area into separate security areas, or a set of embedded security areas, each with a different risk categorization. 

NIST SP800-116 adopts the security area categorizations described in Field Manual 3-19.30, _Physical Security. Headquarters, Department of the Army, United States of America_ (8 January 2001). <!--FM 3-19-30 is no longer listed as in effect by the Army. See http://usacac.army.mil/sites/default/files/misc/doctrine/CDG/fms.html for active listing of FMs.-->The manual defines three security area categories: Exclusion, Limited, and Controlled. (See Table 1.)  The categories distinguish how immediately accessible the security assets (or security interests) are within the security area. 

Table 1.  Security Area Categories<br>

| **Category** | **Description**                      |
| :----------- | :-------------------------------     |
| Controlled  |  An area close to or surrounding a limited or exclusion area.  Entry to a controlled area is restricted to personnel who need access.  Movement of authorized personnel within this area is not necessarily controlled, since entry to the area does not provide immediate access to any security assets or interests.  A controlled area provides administrative control, or safety, or acts as a buffer zone for embedded limited or exclusion areas. |  
| Limited   | An area close to a security asset or interest.  Uncontrolled movement within a limited area may permit access to the asset.  Escorts and other internal restrictions can prevent access. |  
| Exclusion   | An area in which uncontrolled movement would permit direct access to a security asset or interest. |<br>  

You can also define your own categorizations to reflect your particular security needs and/or physical security policies and practices.

3. **Authentication Factor Selection.** The guidelines that govern the types and number of factors required to authenticate people and their credentials for specific security area classifications are straightforward.  Authentication is based on verifying one, two, or three of the following factors:

* Something you have (e.g., a PIV card)
* Something you know (e.g., a PIN)
* Something you are (e.g., a fingerprint or iris scan)

NIST SP800-116 recommends the minimum number of authentication factors required to access controlled, limited, and exclusion areas. (See Table 2.)



