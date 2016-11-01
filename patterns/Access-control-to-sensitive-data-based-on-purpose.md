    {%hyde

    title: "Access control to sensitive data based on purpose"
    type: pattern
    excerpt: "How Data Subjects can ensure that only the required personal information is transferred to the data processor. This pattern is described in detail."
    categories:
        - 
    status: stub
    address:

    %}

[TOC]


##Name
<!--Primary name the pattern is known by.-->

Access control to sensitive data based on purpose

###[Also Known As]
<!-- All other names the pattern is known by.-->

Purpose-based Access Control / Limited Access to Personal Data / Access Control

##Summary
<!-- One short paragraph summarising the pattern.-->

How Data Subjects can ensure that only the required personal information is transferred to the data processor. This pattern is described in detail.

<!--##Context-->
<!-- The situations in which the pattern may apply.-->



##Problem
<!-- The problem a pattern addresses, including a list of forces describing why a problem might be difficult to solve.-->

According to the data protection Directive and Data Protection Legislation the personal data that is collected should be used solely for the purpose for which it was collected, and should not be further processed for any other purposes. Therefore, when personal data is transferred to a third party to carry out any agreed processing (obtaining consent is described in Explicit Consent pattern), only that part of the personal data which is should be conveyed to the third party.

##Solution
<!-- A concise description of how the pattern addresses the problem.-->

It is the responsibility of the DC to protect the personal data of the DS. Consequently the DP needs to ensure that whenever personal data is transferred to carry out an agreed processing, only that part of the personal data should be transferred, which is necessary to carry out the agreed function. The DP does not need to be granted the permission to access all the data, but needs access to PD1 only. After the DC delegates permission to access PD1 to the DP, the DC needs to assure a form of access control so that DP can only access the first part of personal data (PD1). Consequently the DP now cannot get access to all of the Data Subject’s data; instead he is provided the access to a part of the data that he needs to carry out agreed processing. It is the responsibility of the DC to ensure this is carried out, and this responsibility in turn has to be fulfilled by the DP.

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

J. Porekar, A. Jerman-Blažič, and T. Klobučar, “Towards organizational privacy patterns,” Proceedings - The 2nd International Conference on the Digital Society, ICDS 2008, 2008.

E. S. Chung, J. I. Hong, J. Lin, M. K. Prabaker, J. a. Landay, and A. L. Liu, “Development and Evaluation of Emerging Design Patterns for Ubiquitous Computing,” DIS ’04 Proceedings of the 5th conference on Designing interactive systems: processes, practices, methods, and techniques, pp. 233–242, 2004.

C. Bier and E. Krempel, “Common Privacy Patterns in Video Surveillance and Smart Energy,” in ICCCT-2012, 2012, pp. 610–615.

H. Baraki et al., Towards Interdisciplinary Design Patterns for Ubiquitous Computing Applications. Kassel, Germany, 2014.

J. H. Hoepman, “Privacy design strategies,” IFIP SEC 2014, 2014.

<!--##General Comments-->
<!-- Separate discussion on the pattern.-->



##Categories
<!-- Placeholder for future agreed upon categories as per collaboration's evaluation.-->
Hide
Restrict

<!--##Tags-->
<!-- User definable descriptors for additional correlation.-->




