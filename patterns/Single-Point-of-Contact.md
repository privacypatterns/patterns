    {%hyde

    title: "Single Point of Contact"
    type: pattern
    excerpt: "The Single Point of Contact is a security authority who protects the privacy and security of sensitive medical data stored in a cloud by validating the authority of requests and ensuring secure communication channels."
    categories:
        - 
    status: stub
    address:

    %}

[TOC]


##Name
<!--Primary name the pattern is known by.-->

Single Point of Contact

###[Also Known As]
<!-- All other names the pattern is known by.-->

Personal Agent

##Summary
<!-- One short paragraph summarising the pattern.-->

The Single Point of Contact is a security authority who protects the privacy and security of sensitive medical data stored in a cloud by validating the authority of requests and ensuring secure communication channels.

##Context
<!-- The situations in which the pattern may apply.-->

e-Health Services that store their data in a cloud.

##Problem
<!-- The problem a pattern addresses, including a list of forces describing why a problem might be difficult to solve.-->

Conventional security mechanisms are restricted to concrete protocols and platforms which do not allow for effective cloud-based ubiquitous service privacy management

##Solution
<!-- A concise description of how the pattern addresses the problem.-->

Single Point of Contact 'adopts a claim-based approach for both authentication and authorisation' similar to a super-peer design, also acting as a (Resource) Security Token Service, an Identity and Attribute Provider, and a Relying Party. It features a tried and proven expressive e-consent language, and can communicate with other SPoCs in a Circle of Trust

<!--###[Structure]-->
<!--A detailed specification of the structural aspects of the pattern. A class diagram if applicable.-->



<!--###[Implementation]-->
<!--Guidelines for implementing the pattern; code fragments; suggested PETS; policy fragments.-->



##Consequences
<!--The advantages (benefits) and disadvantages (liabilities) of applying the pattern.-->

The SPoC ensures that the privacy of sensitive medical data is protected, and that it is distributed securely and only to the people who are allowed to access the data. However, it requires a reliable credential-based authentication system to be able to validate requests.

<!--###[Constraints]-->
<!-- limitations as a consequence of applying the pattern.-->



<!--##Examples-->
<!--Motivational example to see how the pattern is applied.-->



<!--###[Known Uses]-->
<!-- Pointers to various applications of the pattern.-->



<!--##See Also-->
<!-- Any pointers to relevant information, not contained in the subfields below.-->



<!--###[Related Patterns]-->
<!-- Supporting and conflicting patterns-->



###[Sources]
<!-- References to the original source of the pattern.-->

C. Bier and E. Krempel, “Common Privacy Patterns in Video Surveillance and Smart Energy,” in ICCCT-2012, 2012, pp. 610–615.

L. Fan et al., “SPoC: Protecting Patient Privacy for e-Health Services in the Cloud,” 2012.

<!--##General Comments-->
<!-- Separate discussion on the pattern.-->



##Categories
<!-- Placeholder for future agreed upon categories as per collaboration's evaluation.-->
Control
Choose

<!--##Tags-->
<!-- User definable descriptors for additional correlation.-->




