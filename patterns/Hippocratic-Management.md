    {%hyde

    title: "Hippocratic Management"
    type: pattern
    excerpt: "Enforce the collecting and processing of data in a predefined confinement area (which could be a user controlled location, or an engineer defined distributed location). The rationale for the enforcement principle is to prevent accidental or malicious leaking of personal data."
    categories:
        - 
    status: draft
    address:

    %}

[TOC]


##Name
<!--Primary name the pattern is known by.-->

Hippocratic Management

<!--###[Also Known As]-->
<!-- All other names the pattern is known by.-->



##Summary
<!-- One short paragraph summarising the pattern.-->

Enforce the collecting and processing of data in a predefined confinement area (which could be a user controlled location, or an engineer defined distributed location). The rationale for the enforcement principle is to prevent accidental or malicious leaking of personal data.

##Context
<!-- The situations in which the pattern may apply.-->

Implementation of a data management capability should follow the principles for data protection (purpose specification, consent, limited collection-use-disclosure-retention, accuracy, safety, openness, and compliance)

##Problem
<!-- The problem a pattern addresses, including a list of forces describing why a problem might be difficult to solve.-->

For instance careless management of a web server that collects customer data would increase the risk that employees access such data without authorisation.

##Solution
<!-- A concise description of how the pattern addresses the problem.-->

The resulting architecture associates data with metadata describing protection policies, e.g. who can have access to data, or retention parameters. Data can only be accessed through a well-defined interface (e.g. based on a query language). Finally the data management takes proactive moves for enforcing policies (e.g. data is deleted after the retention limit).

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




