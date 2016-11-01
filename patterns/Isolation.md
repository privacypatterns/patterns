    {%hyde

    title: "Isolation"
    type: pattern
    excerpt: "Provides isolation between independent applications which run on the same platform"
    categories:
        - 
    status: stub
    address:

    %}

[TOC]


##Name
<!--Primary name the pattern is known by.-->

Isolation

<!--###[Also Known As]-->
<!-- All other names the pattern is known by.-->



##Summary
<!-- One short paragraph summarising the pattern.-->

Provides isolation between independent applications which run on the same platform

##Context
<!-- The situations in which the pattern may apply.-->

In a system which runs multiples processes, these processes need to be isolated from one another in order to prevent overlapping resource access and risking personal data exposure

##Problem
<!-- The problem a pattern addresses, including a list of forces describing why a problem might be difficult to solve.-->

Some processes are able to accidentally or maliciously access resources from another application, thereby acquiring the ability to access personal data

##Solution
<!-- A concise description of how the pattern addresses the problem.-->

The rationale is to prevent the risk for other applications to accidentally or maliciously access computing resources and data associated with another application. The isolation pattern is based on the concepts of partitions which are created by a virtualisation layer.

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

A. Kung, “PEARs: Privacy Enhancing ARchitectures,” Lecture Notes in Computer Science (including subseries Lecture Notes in Artificial Intelligence and Lecture Notes in Bioinformatics), vol. 8450 LNCS, pp. 18–29, 2014.

<!--##General Comments-->
<!-- Separate discussion on the pattern.-->



<!--##Categories-->
<!-- Placeholder for future agreed upon categories as per collaboration's evaluation.-->

<!--##Tags-->
<!-- User definable descriptors for additional correlation.-->




