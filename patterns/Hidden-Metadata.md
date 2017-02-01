    {%hyde

    title: "Hidden Metadata"
    type: pattern
    excerpt: "Hide the meta information associated with data content that reveal information about sensitive data content"
    categories:
        - 
    status: draft
    address:

    %}

[TOC]


##Name
<!--Primary name the pattern is known by.-->

Hidden Metadata

###[Also Known As]
<!-- All other names the pattern is known by.-->

HeaderManipulation / Anonymization Proxy / Anonymization Gateway / Blurred Identity / Pseudonym Hopping / Blurred Personal Data / Strip Invisible Metadata

##Summary
<!-- One short paragraph summarising the pattern.-->

Hide the meta information associated with data content that reveal information about sensitive data content

##Context
<!-- The situations in which the pattern may apply.-->

You are designing a system to protect the privacy of the users. This system will maintain sender anonymity in a messaging scenario. Although this is an important application area, the context is not limited to messaging only. The context also entails other scenarios like anonymity in a location tracking systemor anonymity preserv- ing data sharing in a data publishing system.

##Problem
<!-- The problem a pattern addresses, including a list of forces describing why a problem might be difficult to solve.-->

Any metadata associated with the data traffic in the network reveals information about the originator of that data packet. The packet headers are used for information routing in forward and reverse direction. The information in the packet headers like IP addresses reveal private information about sender’s identity and their location.

##Solution
<!-- A concise description of how the pattern addresses the problem.-->

Obfuscate the metadata associated with the data. For the web browsing domain, create a middleman between the request sender and the recipient that strips off identity-revealing metadata from the packet headers. For email messaging, use a remailer that strips identifying header information from outbound email messages. Strip off the pseudonym associated with an agent when he enters the mix zone. Assign a different pseudonym to the agent when he comes out of the mix zone. For privacy preserving data sharing, scramble the sorting order of the data in the table. Remove any other meta-information in the data that can compromise the privacy.

<!--###[Structure]-->
<!--A detailed specification of the structural aspects of the pattern. A class diagram if applicable.-->



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



<!--###[Related Patterns]-->
<!-- Supporting and conflicting patterns-->



###[Sources]
<!-- References to the original source of the pattern.-->

M. Hafiz, “A collection of privacy design patterns,” Proceedings of the 2006 conference on Pattern languages of programs - PLoP ’06, p. 1, 2006.

E. S. Chung, J. I. Hong, J. Lin, M. K. Prabaker, J. a. Landay, and A. L. Liu, “Development and Evaluation of Emerging Design Patterns for Ubiquitous Computing,” DIS ’04 Proceedings of the 5th conference on Designing interactive systems: processes, practices, methods, and techniques, pp. 233–242, 2004.

C. Bier and E. Krempel, “Common Privacy Patterns in Video Surveillance and Smart Energy,” in ICCCT-2012, 2012, pp. 610–615.

S. Romanosky, A. Acquisti, J. Hong, L. F. Cranor, and B. Friedman, “Privacy patterns for online interactions,” Proceedings of the 2006 conference on Pattern languages of programs - PLoP ’06, p. 1, 2006.

H. Baraki et al., Towards Interdisciplinary Design Patterns for Ubiquitous Computing Applications. Kassel, Germany, 2014.

<!--##General Comments-->
<!-- Separate discussion on the pattern.-->



<!--##Categories-->
<!-- Placeholder for future agreed upon categories as per collaboration's evaluation.-->

<!--##Tags-->
<!-- User definable descriptors for additional correlation.-->




