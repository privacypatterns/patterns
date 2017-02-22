    {%hyde

    title: "Attention Screen"
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

Attention Screen

###[Also Known As]
<!-- All other names the pattern is known by.-->

Message Filter

<!--##Summary-->
<!-- One short paragraph summarising the pattern.-->



##Context
<!-- The situations in which the pattern may apply.-->

Other users provide information to a shared environment and you are consuming this information. Other users may feel the need to get in contact with the local user. To do so, they send information to the local user that catches his attention.

##Problem
<!-- The problem a pattern addresses, including a list of forces describing why a problem might be difficult to solve.-->

Every request for attention needs to be processed by the user. Thus, it already takes some of his attention. But in situations, where the user needs to focus his attention on other things, this is disturbing.

##Solution
<!-- A concise description of how the pattern addresses the problem.-->

Enable the user to filter the information which reaches him. Use meta-information (e.g. sender details) or con- tent information (e.g. important keywords) to distinguish impor- tant information from not so relevant information. Collect the less important information at a place where the user can process it on demand and forward relevant information directly to the user.

<!--###[Structure]-->
<!--A detailed specification of the structural aspects of the pattern. A class diagram if applicable.-->



<!--###[Implementation]-->
<!--Guidelines for implementing the pattern; code fragments; suggested PETS; policy fragments.-->



##Consequences
<!--The advantages (benefits) and disadvantages (liabilities) of applying the pattern.-->

The definition of rules can get too complicated for naive users. Rules may classify important information wrong so that it may be ignored by the user. Thus, you should not be too rigid when fil- tering the information. If for instance only requests from users that are on the local user’s Buddy List are reaching the local user, he will not be able to establish new contacts anymore. This would be crucial in a community system because members are required to be open for other members.

<!--###[Constraints]-->
<!-- limitations as a consequence of applying the pattern.-->



##Examples
<!--Motivational example to see how the pattern is applied.-->

Siemens S55; Mozilla Junk Mail Filter; TeamSpace (Fuchs, Poltrock, and Wetzel 2001); Instant Messaging Systems; WebWasher

<!--###[Known Uses]-->
<!-- Pointers to various applications of the pattern.-->



<!--##See Also-->
<!-- Any pointers to relevant information, not contained in the subfields below.-->



###[Related Patterns]
<!-- Supporting and conflicting patterns-->

Don’t Disturb; Buddy List; Train the Recommender; Birds of a Feather; Masquerade

###[Sources]
<!-- References to the original source of the pattern.-->

T. Shümmer, “The Public Privacy – Patterns for Filtering Personal Information in Collaborative Systems,” in Proceedings of CHI workshop on Human-Computer-Human-Interaction Patterns, 2004.

<!--##General Comments-->
<!-- Separate discussion on the pattern.-->



##Categories
<!-- Placeholder for future agreed upon categories as per collaboration's evaluation.-->
Minimise
Select

<!--##Tags-->
<!-- User definable descriptors for additional correlation.-->




