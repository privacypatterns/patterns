    {%hyde

    title: "Distributed Usage Control"
    type: pattern
    excerpt: "An infrastructure that supports (1) application and protocol-independent data flow tracking across different operating system instances, (2) sticking policies to data upon sending it to another system, and (3) policy enforcement at the receiving site."
    categories:
        - 
    status: stub
    address:

    %}

[TOC]


##Name
<!--Primary name the pattern is known by.-->

Distributed Usage Control

<!--###[Also Known As]-->
<!-- All other names the pattern is known by.-->



##Summary
<!-- One short paragraph summarising the pattern.-->

An infrastructure that supports (1) application and protocol-independent data flow tracking across different operating system instances, (2) sticking policies to data upon sending it to another system, and (3) policy enforcement at the receiving site.

##Context
<!-- The situations in which the pattern may apply.-->

Usage control has been proposed and discussed with the goal to overcome one shortcoming of traditional access control models: the loss of control after access to data has been granted. Distributed usage control is concerned with the usage of data in distributed system environments

##Problem
<!-- The problem a pattern addresses, including a list of forces describing why a problem might be difficult to solve.-->

Policies express what may or may not happen to usage controlled data. They must be enforced at and across all systems storing, processing, and distributing data. For this reason, an infrastructure is needed that allows for (1) inter-system data flow tracking and (2) the enforcement of both globally and locally enforceable usage control policies.

##Solution
<!-- A concise description of how the pattern addresses the problem.-->

The infrastructure is distributed in that its components must be deployed on [all] system[s]. The task of the Policy Information Point is to hold the information flow state of the system on which it is deployed. The Policy Management Point manages all usage control policies for data entering, leaving, and residing in the respective system. [These two components communicate together between systems].

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

F. Kelbert and A. Pretschner, “Towards a policy enforcement infrastructure for distributed usage control,” Proceedings of the 17th ACM SACMAT (Symposium on Access Control Models And Technologies), p. 119, 2012.

<!--##General Comments-->
<!-- Separate discussion on the pattern.-->



##Categories
<!-- Placeholder for future agreed upon categories as per collaboration's evaluation.-->
Enforce
Uphold

<!--##Tags-->
<!-- User definable descriptors for additional correlation.-->




