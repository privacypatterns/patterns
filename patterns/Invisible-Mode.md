    {%hyde

    title: "Invisible Mode"
    type: pattern
    excerpt: "Invisible mode is a simple and useful interaction for hiding from all others."
    categories:
        - 
    status: draft
    address:

    %}

[TOC]


##Name
<!--Primary name the pattern is known by.-->

Invisible Mode

<!--###[Also Known As]-->
<!-- All other names the pattern is known by.-->



##Summary
<!-- One short paragraph summarising the pattern.-->

Invisible mode is a simple and useful interaction for hiding from all others.

##Context
<!-- The situations in which the pattern may apply.-->

A user system that keeps track of, and displays the login status of its users.

##Problem
<!-- The problem a pattern addresses, including a list of forces describing why a problem might be difficult to solve.-->

When a user is authenticated they are typically identified by the system, either partially through a pseudonym, or by association. The system then typically alerts other users to the presence of this user, and maintains a status reflecting their availability. This is not always a desired behaviour, as it can be used for trend analysis or to correlate with other potentially external data, thereby revealing identity, or aspects about an identity which the user would not want revealed

##Solution
<!-- A concise description of how the pattern addresses the problem.-->

Makes an invisible mode available to the user so that the flow of data to others will be stopped. An instant messenger would indicate, for example, that the user is off-line

<!--###[Structure]-->
<!--A detailed specification of the structural aspects of the pattern. A class diagram if applicable.-->



<!--###[Implementation]-->
<!--Guidelines for implementing the pattern; code fragments; suggested PETS; policy fragments.-->



##Consequences
<!--The advantages (benefits) and disadvantages (liabilities) of applying the pattern.-->

Invisible mode can be both useful and a problem for victims of bullying, e-stalking or other issues with other users in the same system. Although it enables the victim to remain invisible to the perpetrator they have problems with, the invisible mode can also be used against the victim by the perpetrator by suggesting they are offline even though they are actually logged in and able to perceive the victim.

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

H. Baraki et al., Towards Interdisciplinary Design Patterns for Ubiquitous Computing Applications. Kassel, Germany, 2014.

G. Iachello and J. Hong, “End-User Privacy in Human-Computer Interaction,” Foundations and Trends® in Human-Computer Interaction, vol. 1, no. 1, pp. 1–137, 2007.

<!--##General Comments-->
<!-- Separate discussion on the pattern.-->



<!--##Categories-->
<!-- Placeholder for future agreed upon categories as per collaboration's evaluation.-->

<!--##Tags-->
<!-- User definable descriptors for additional correlation.-->




