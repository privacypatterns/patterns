    {%hyde

    title: "Obtaining Explicit Consent"
    type: pattern
    excerpt: "Describes how organizations can obtain the required explicit consent in case when dealing with sensitive information of the data subject. This pattern is described in detail."
    categories:
        - 
    status: draft
    address:

    %}

[TOC]


##Name
<!--Primary name the pattern is known by.-->

Obtaining Explicit Consent

###[Also Known As]
<!-- All other names the pattern is known by.-->

Explicit Consent / Obtaining Explicit consent via privacy agreement

##Summary
<!-- One short paragraph summarising the pattern.-->

Describes how organizations can obtain the required explicit consent in case when dealing with sensitive information of the data subject. This pattern is described in detail.

<!--##Context-->
<!-- The situations in which the pattern may apply.-->



##Problem
<!-- The problem a pattern addresses, including a list of forces describing why a problem might be difficult to solve.-->

If Organization (ORG) wants to deliver services that require exposure of Sensitive Data (SD) to a User it needs to acquire an explicit permission to use the Sensitive Data. In described case ORG in the Data Controller (DC) and User is the Data Subject (DS).

##Solution
<!-- A concise description of how the pattern addresses the problem.-->

Organization (ORG) and User (DS) need to agree upon what sensitive data is to be gathered for what purposes. This is represented by ORG by its privacy policy. Constructing and maintaining Privacy Policy is matter of another organizational privacy pattern. After the privacy policy has been presented to the DS he might want to negotiate it. Negotiation of privacy policies can either be carried out in person or it can be automatic to certain degree. Automatic privacy policy negotiation is a matter of another privacy organizational pattern. Once the ORG and DS have agreed on the negotiated privacy practices described in Privacy Policy the Privacy Agreement is created time stamped to assure the point in time in which it starts to be valid. Both parties need to sign the agreement. Signing it serves as means of explicit consent. Signing can be carried out in traditional fashion or using digital signatures.

###[Structure]
<!--A detailed specification of the structural aspects of the pattern. A class diagram if applicable.-->

Privacy Agreement is composed of: Agreed Privacy Policy; Signatures of both parties involved; Timestamp

<!--###[Implementation]-->
<!--Guidelines for implementing the pattern; code fragments; suggested PETS; policy fragments.-->



<!--##Consequences-->
<!--The advantages (benefits) and disadvantages (liabilities) of applying the pattern.-->



<!--###[Constraints]-->
<!-- limitations as a consequence of applying the pattern.-->



<!--##Examples-->
<!--Motivational example to see how the pattern is applied.-->



<!--###[Known Uses]-->
<!-- Pointers to various applications of the pattern.-->



<!--##See Also-->
<!-- Any pointers to relevant information, not contained in the subfields below.-->



###[Related Patterns]
<!-- Supporting and conflicting patterns-->

Constructing Privacy Policy; Maintaining Privacy Policy; Privacy Policy Negotiation; Maintaining agreements over longer periods of time

###[Sources]
<!-- References to the original source of the pattern.-->

J. Porekar, A. Jerman-Blažič, and T. Klobučar, “Towards organizational privacy patterns,” Proceedings - The 2nd International Conference on the Digital Society, ICDS 2008, 2008.

C. Bier and E. Krempel, “Common Privacy Patterns in Video Surveillance and Smart Energy,” in ICCCT-2012, 2012, pp. 610–615.

<!--##General Comments-->
<!-- Separate discussion on the pattern.-->



<!--##Categories-->
<!-- Placeholder for future agreed upon categories as per collaboration's evaluation.-->

<!--##Tags-->
<!-- User definable descriptors for additional correlation.-->




