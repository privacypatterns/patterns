    {%hyde

    title: "Keeping Personal Data on Personal Devices"
    type: pattern
    excerpt: "Subjects keep control on their personal data that are stored on a personal device."
    categories:
        - 
    status: draft
    address:

    %}

[TOC]


##Name
<!--Primary name the pattern is known by.-->

Keeping Personal Data on Personal Devices

###[Also Known As]
<!-- All other names the pattern is known by.-->

Personal Data Store / Data Confinement

##Summary
<!-- One short paragraph summarising the pattern.-->

Subjects keep control on their personal data that are stored on a personal device.

##Context
<!-- The situations in which the pattern may apply.-->

The pattern is applicable to any data produced by the data subject (or originally under his control) as opposed to data about him produced by third parties.

##Problem
<!-- The problem a pattern addresses, including a list of forces describing why a problem might be difficult to solve.-->

Data subjects lose control over their data when they are stored on a server operated by a third party.

##Solution
<!-- A concise description of how the pattern addresses the problem.-->

A solution consists in combining a central server and secure personal tokens. Personal tokens, which can take the form of USB keys, embed a database system, a local web server and a certificate for their authentication by the central server. Data subjects can decide on the status of their data and, depending on their level of sensitivity, choose to record them exclusively on their personal token or to have them replicated on the central server. Replication on the central server is useful to enhance sustainability and to allow designated third parties (e.g. health professionals) to get access to the data.

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

E. S. Chung, J. I. Hong, J. Lin, M. K. Prabaker, J. a. Landay, and A. L. Liu, “Development and Evaluation of Emerging Design Patterns for Ubiquitous Computing,” DIS ’04 Proceedings of the 5th conference on Designing interactive systems: processes, practices, methods, and techniques, pp. 233–242, 2004.

C. Bier and E. Krempel, “Common Privacy Patterns in Video Surveillance and Smart Energy,” in ICCCT-2012, 2012, pp. 610–615.

H. Baraki et al., Towards Interdisciplinary Design Patterns for Ubiquitous Computing Applications. Kassel, Germany, 2014.

“privacypatterns.eu - collecting patterns for better privacy.” [Online]. Available: https://privacypatterns.eu/. [Accessed: 20-Oct-2015].

A. Kung, “PEARs: Privacy Enhancing ARchitectures,” Lecture Notes in Computer Science (including subseries Lecture Notes in Artificial Intelligence and Lecture Notes in Bioinformatics), vol. 8450 LNCS, pp. 18–29, 2014.

G. Iachello and J. Hong, “End-User Privacy in Human-Computer Interaction,” Foundations and Trends® in Human-Computer Interaction, vol. 1, no. 1, pp. 1–137, 2007.

<!--##General Comments-->
<!-- Separate discussion on the pattern.-->



<!--##Categories-->
<!-- Placeholder for future agreed upon categories as per collaboration's evaluation.-->

<!--##Tags-->
<!-- User definable descriptors for additional correlation.-->




