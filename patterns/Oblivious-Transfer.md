    {%hyde

    title: "Oblivious Transfer"
    type: pattern
    excerpt: "A transaction between an initiator and a respondent without revealing the initiator’s private information to the respondent."
    categories:
        - 
    status: stub
    address:

    %}

[TOC]


##Name
<!--Primary name the pattern is known by.-->

Oblivious Transfer

<!--###[Also Known As]-->
<!-- All other names the pattern is known by.-->



##Summary
<!-- One short paragraph summarising the pattern.-->

A transaction between an initiator and a respondent without revealing the initiator’s private information to the respondent.

##Context
<!-- The situations in which the pattern may apply.-->

Protocols exist wherein a sender or initiator can provide multiple pieces of information, and up to one unknown piece is selected by a receiver. The sender does not know which piece was taken, nor does the receiver know which pieces were not

##Problem
<!-- The problem a pattern addresses, including a list of forces describing why a problem might be difficult to solve.-->

Messaging is amenable to anonymity because if a message sender or a recipient hides its identity and does not reveal any traits in the message, he or she can remain hidden. For transactions that require users to share identifying attributes between them, it is much harder to remain private

##Solution
<!-- A concise description of how the pattern addresses the problem.-->

Adopt an oblivious transfer protocol, in which a sender transfers one of potentially many pieces of information to a receiver, but remains oblivious as to what piece (if any) has been transferred. Alternatives include 1-out-of-2 oblivious transfer, private information retrieval, private matching and private set intersection schemes, and other practical applications other than privacy.

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

M. Hafiz, “A Pattern Language for Developing Privacy Enhancing Technologies,” Software - Practice and Experience, vol. 43, 2013.

<!--##General Comments-->
<!-- Separate discussion on the pattern.-->



##Categories
<!-- Placeholder for future agreed upon categories as per collaboration's evaluation.-->
Hide
Dissociate

<!--##Tags-->
<!-- User definable descriptors for additional correlation.-->




