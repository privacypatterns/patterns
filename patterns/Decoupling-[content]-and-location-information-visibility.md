    {%hyde

    title: "Decoupling [content] and location information visibility"
    type: pattern
    excerpt: "Allow users to select the default level of privacy that a system will apply to their uploaded media."
    categories:
        - 
    status: draft
    address:

    %}

[TOC]


##Name
<!--Primary name the pattern is known by.-->

Decoupling [content] and location information visibility

<!--###[Also Known As]-->
<!-- All other names the pattern is known by.-->



##Summary
<!-- One short paragraph summarising the pattern.-->

Allow users to select the default level of privacy that a system will apply to their uploaded media.

##Context
<!-- The situations in which the pattern may apply.-->

Automatic media sharing policies

##Problem
<!-- The problem a pattern addresses, including a list of forces describing why a problem might be difficult to solve.-->

Automating public media disclosure presents the possibility for unintentional personal data leakage

##Solution
<!-- A concise description of how the pattern addresses the problem.-->

Provide a means to control the default level of privacy attributed to an automated media share, with granular settings to maintain usability

<!--###[Structure]-->
<!--A detailed specification of the structural aspects of the pattern. A class diagram if applicable.-->



<!--###[Implementation]-->
<!--Guidelines for implementing the pattern; code fragments; suggested PETS; policy fragments.-->



##Consequences
<!--The advantages (benefits) and disadvantages (liabilities) of applying the pattern.-->

If the system default is not the setting users usually use, allowing them to pick their own default setting will make it less likely that users make mistakes when uploading media. Users will still need to pay attention when they want to upload media with privacy settings that don't match their own defaults, and any changes the system makes to the privacy settings may invite mistakes by users who are caught unaware.

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




