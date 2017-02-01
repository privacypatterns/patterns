    {%hyde

    title: "[Decoupling] discoverability and the convenience of disclosure"
    type: pattern
    excerpt: "Make newly uploaded media private by default and require extra user action to make it public."
    categories:
        - 
    status: draft
    address:

    %}

[TOC]


##Name
<!--Primary name the pattern is known by.-->

[Decoupling] discoverability and the convenience of disclosure

<!--###[Also Known As]-->
<!-- All other names the pattern is known by.-->



##Summary
<!-- One short paragraph summarising the pattern.-->

Make newly uploaded media private by default and require extra user action to make it public.

##Context
<!-- The situations in which the pattern may apply.-->

Automatic media sharing and indexing

##Problem
<!-- The problem a pattern addresses, including a list of forces describing why a problem might be difficult to solve.-->

Published media is often immediately indexed and shown in searches, when this media is unintentionally public then privacy concerns are present

##Solution
<!-- A concise description of how the pattern addresses the problem.-->

Do not automatically enable discoverability of media, unless users have given consent to do so, instead giving users a chance to change their minds

<!--###[Structure]-->
<!--A detailed specification of the structural aspects of the pattern. A class diagram if applicable.-->



<!--###[Implementation]-->
<!--Guidelines for implementing the pattern; code fragments; suggested PETS; policy fragments.-->



##Consequences
<!--The advantages (benefits) and disadvantages (liabilities) of applying the pattern.-->

Making media automatically discoverable without user consent violates the informed concent property in European data law, so having the default be set to private will prevent legal liabilities for the company. It also means users will be less likely to accidentally share personal information with entities they didn't want to.

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

S. Ahern, D. Eckles, N. Good, S. King, M. Naaman, and R. Nair, “Over-Exposed ? Privacy Patterns and Considerations in Online and Mobile Photo Sharing,” CHI ’07, pp. 357–366, 2007.

<!--##General Comments-->
<!-- Separate discussion on the pattern.-->



<!--##Categories-->
<!-- Placeholder for future agreed upon categories as per collaboration's evaluation.-->

<!--##Tags-->
<!-- User definable descriptors for additional correlation.-->




