    {%hyde

    title: "Masquerade"
    type: pattern
    excerpt: ""
    categories:
        - 
    status: stub
    address:

    %}

[TOC]


##Name
<!--Primary name the pattern is known by.-->

Masquerade

###[Also Known As]
<!-- All other names the pattern is known by.-->

Anonymous Interaction

<!--##Summary-->
<!-- One short paragraph summarising the pattern.-->



##Context
<!-- The situations in which the pattern may apply.-->

You are working in a monitored environment (e.g. an environment with Gaze Over the Shoulder in place), where personal information such as mail addresses or the work status are visible for other users of the environment.

##Problem
<!-- The problem a pattern addresses, including a list of forces describing why a problem might be difficult to solve.-->

User monitoring is required for providing awareness information to remote users or associating work results with a specific user. On the other hand users often do not act as confident if they know that they are monitored as they would act in an anonymous environment. Especially open- ness and the courage for taking risks may be much lower.

##Solution
<!-- A concise description of how the pattern addresses the problem.-->

Let the user control how much interaction information he provides to the system. This means that the user should be able to filter the information, which is revealed from his personal information. Remember to consider Reciprocity

<!--###[Structure]-->
<!--A detailed specification of the structural aspects of the pattern. A class diagram if applicable.-->



<!--###[Implementation]-->
<!--Guidelines for implementing the pattern; code fragments; suggested PETS; policy fragments.-->



##Consequences
<!--The advantages (benefits) and disadvantages (liabilities) of applying the pattern.-->

Anonymous interaction with the system may lower the inhibition threshold for destructive or forbidden behavior. The users do not have to fear that destructive activities are associated with their identity. Thus, you should provide only limited functionality for anonymous users (e.g. only read access or only moderated postings to a discussion board).

<!--###[Constraints]-->
<!-- limitations as a consequence of applying the pattern.-->



##Examples
<!--Motivational example to see how the pattern is applied.-->

Video systems: NYNEXPortholes (Lee, Girgensohn, and Schlueter 1997); TUKAN (Schummer and Haake 2001); Anonymous access

<!--###[Known Uses]-->
<!-- Pointers to various applications of the pattern.-->



<!--##See Also-->
<!-- Any pointers to relevant information, not contained in the subfields below.-->



###[Related Patterns]
<!-- Supporting and conflicting patterns-->

Don’t Disturb; Gaze Over the Shoulder; Reciprocity

###[Sources]
<!-- References to the original source of the pattern.-->

T. Shümmer, “The Public Privacy – Patterns for Filtering Personal Information in Collaborative Systems,” in Proceedings of CHI workshop on Human-Computer-Human-Interaction Patterns, 2004.

<!--##General Comments-->
<!-- Separate discussion on the pattern.-->



##Categories
<!-- Placeholder for future agreed upon categories as per collaboration's evaluation.-->
Control
Choose

<!--##Tags-->
<!-- User definable descriptors for additional correlation.-->




