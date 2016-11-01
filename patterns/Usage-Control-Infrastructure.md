    {%hyde

    title: "Usage Control Infrastructure"
    type: pattern
    excerpt: "A usage control infrastructure retains control over data even after someone else has been granted access to it."
    categories:
        - 
    status: draft
    address:

    %}

[TOC]


##Name
<!--Primary name the pattern is known by.-->

Usage Control Infrastructure

<!--###[Also Known As]-->
<!-- All other names the pattern is known by.-->



##Summary
<!-- One short paragraph summarising the pattern.-->

A usage control infrastructure retains control over data even after someone else has been granted access to it.

##Context
<!-- The situations in which the pattern may apply.-->

A system where multiple parties work with the same data.

##Problem
<!-- The problem a pattern addresses, including a list of forces describing why a problem might be difficult to solve.-->

In order to enforce policies, 'an infrastructure is needed that allows for (1) inter-system data flow tracking and (2) the enforcement of both globally and locally enforceable usage control policies. Examples for policies are “do not process my data with application X” and “not more than two instances of document Y may be opened simultaneously”. While the compliance with the former can be enforced locally, this is not the case for the latter, since the document may be opened on different systems at the same time'.

##Solution
<!-- A concise description of how the pattern addresses the problem.-->

An 'infrastructure that supports (1) application-and protocol-independent data flow tracking across different operating system instances, (2) sticking policies to data upon sending it to another system, and (3) policy enforcement at the receiving site'

<!--###[Structure]-->
<!--A detailed specification of the structural aspects of the pattern. A class diagram if applicable.-->



<!--###[Implementation]-->
<!--Guidelines for implementing the pattern; code fragments; suggested PETS; policy fragments.-->



##Consequences
<!--The advantages (benefits) and disadvantages (liabilities) of applying the pattern.-->

A usage control infrastructure enables an organisation to enforce their data policies even after another party has been granted access to data. The downside is that this party will need to use the infrastructure every time they want access to the data. An 'offline mode' might not be available, depending on the policies set for the data.

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

F. Kelbert and A. Pretschner, “Towards a policy enforcement infrastructure for distributed usage control,” Proceedings of the 17th ACM SACMAT (Symposium on Access Control Models And Technologies), p. 119, 2012.

<!--##General Comments-->
<!-- Separate discussion on the pattern.-->



<!--##Categories-->
<!-- Placeholder for future agreed upon categories as per collaboration's evaluation.-->

<!--##Tags-->
<!-- User definable descriptors for additional correlation.-->




