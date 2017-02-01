    {%hyde

    title: "Layered Encryption"
    type: pattern
    excerpt: " This pattern provides unlinkability between senders and receivers by encapsulating the data in different layers of encryption, limiting the knowledge of each node along the delivery path."
    categories:
        - 
    status: draft
    address:

    %}

[TOC]


##Name
<!--Primary name the pattern is known by.-->

Layered Encryption

###[Also Known As]
<!-- All other names the pattern is known by.-->

Onion Routing

##Summary
<!-- One short paragraph summarising the pattern.-->

 This pattern provides unlinkability between senders and receivers by encapsulating the data in different layers of encryption, limiting the knowledge of each node along the delivery path.

##Context
<!-- The situations in which the pattern may apply.-->

A system in which data is routed between different nodes.

##Problem
<!-- The problem a pattern addresses, including a list of forces describing why a problem might be difficult to solve.-->

When delivering data, the receiver has to be known. If the system provides the functionality that the receiver of data should be able to answer, than the receiver should also know the address of the sender. When forwarding information over multiple stations then, in a naive implementation, each station on the delivery path knows the sender and the final destination.

##Solution
<!-- A concise description of how the pattern addresses the problem.-->

The solution is to encrypt the data in layers such that every station on the way can remove one layer of encryption and thus get to know the immediate next station. This way, every party on the path from the sender to the receiver only gets to know the immediate successor and predecessor on the delivery path.

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

C. Bier and E. Krempel, “Common Privacy Patterns in Video Surveillance and Smart Energy,” in ICCCT-2012, 2012, pp. 610–615.

“privacypatterns.eu - collecting patterns for better privacy.” [Online]. Available: https://privacypatterns.eu/. [Accessed: 20-Oct-2015].

<!--##General Comments-->
<!-- Separate discussion on the pattern.-->



<!--##Categories-->
<!-- Placeholder for future agreed upon categories as per collaboration's evaluation.-->

<!--##Tags-->
<!-- User definable descriptors for additional correlation.-->




