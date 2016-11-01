    {%hyde

    title: "Who’s Listening"
    type: pattern
    excerpt: " "
    categories:
        - 
    status: stub
    address:

    %}

[TOC]


##Name
<!--Primary name the pattern is known by.-->

Who’s Listening

<!--###[Also Known As]-->
<!-- All other names the pattern is known by.-->



<!--##Summary-->
<!-- One short paragraph summarising the pattern.-->

 

##Context
<!-- The situations in which the pattern may apply.-->

The users are providing information in an information space.

##Problem
<!-- The problem a pattern addresses, including a list of forces describing why a problem might be difficult to solve.-->

Users are providing information for other users by means of shared objects. But making an object accessible does not ensure that the object was seen by other users.

##Solution
<!-- A concise description of how the pattern addresses the problem.-->

Inform the author of a shared object when another user reads this object.

<!--###[Structure]-->
<!--A detailed specification of the structural aspects of the pattern. A class diagram if applicable.-->



<!--###[Implementation]-->
<!--Guidelines for implementing the pattern; code fragments; suggested PETS; policy fragments.-->



##Consequences
<!--The advantages (benefits) and disadvantages (liabilities) of applying the pattern.-->

This pattern will only work, if the users trust the system that provides the information and log in personally. In web based systems that don’t require personal login, it is not possible to detect, who is visiting the site (even cookies do not reveal information about the users’ identities). This is problematic for this pattern, but it ensures that the users can control their privacy. If information like addresses of the visiting users were sent by the browser on each visit to a web site, then spammers could easily misuse the mech- anism by creating a web site that collects all the addresses of the visitors.

<!--###[Constraints]-->
<!-- limitations as a consequence of applying the pattern.-->



##Examples
<!--Motivational example to see how the pattern is applied.-->

Electronic Mail; The BSCWshared workspace system(Bentley, Horstmann, and Trevor 1997); Whitepaper download at serviceware.com; MSN Messenger

<!--###[Known Uses]-->
<!-- Pointers to various applications of the pattern.-->



<!--##See Also-->
<!-- Any pointers to relevant information, not contained in the subfields below.-->



###[Related Patterns]
<!-- Supporting and conflicting patterns-->

Activity Counter; Elephant’s Brain; Magic Document (Volter 2003)

###[Sources]
<!-- References to the original source of the pattern.-->

T. Shümmer, “The Public Privacy – Patterns for Filtering Personal Information in Collaborative Systems,” in Proceedings of CHI workshop on Human-Computer-Human-Interaction Patterns, 2004.

<!--##General Comments-->
<!-- Separate discussion on the pattern.-->



<!--##Categories-->
<!-- Placeholder for future agreed upon categories as per collaboration's evaluation.-->

<!--##Tags-->
<!-- User definable descriptors for additional correlation.-->




