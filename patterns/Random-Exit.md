    {%hyde

    title: "Random Exit"
    type: pattern
    excerpt: "Suggests adding a variation to packet routing mechanism by allowing mix networks to forward packet to a recipient instead of forwarding to the next hop."
    categories:
        - 
    status: draft
    address:

    %}

[TOC]


##Name
<!--Primary name the pattern is known by.-->

Random Exit

<!--###[Also Known As]-->
<!-- All other names the pattern is known by.-->



##Summary
<!-- One short paragraph summarising the pattern.-->

Suggests adding a variation to packet routing mechanism by allowing mix networks to forward packet to a recipient instead of forwarding to the next hop.

##Context
<!-- The situations in which the pattern may apply.-->

In a mix network, incoming packets may be routed out prematurely to prevent association if there are compromised exit nodes

##Problem
<!-- The problem a pattern addresses, including a list of forces describing why a problem might be difficult to solve.-->

The exit node of an anonymity network forwards a packet to its final recipient. Exit nodes often come under abuse. Having a few exit nodes reduces the number of points an adversary needs to monitor.

##Solution
<!-- A concise description of how the pattern addresses the problem.-->

Allow traffic to exit an anonymity network not only at the endpoints [of] a circuit, but also in the middle of a circuit. Tor initiators can direct traffic to exit partway down the circuit, by using in-band signaling within the circuit. This frustrates traffic shape and volume attacks based on observing the end of the circuit.

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



<!--##Categories-->
<!-- Placeholder for future agreed upon categories as per collaboration's evaluation.-->

<!--##Tags-->
<!-- User definable descriptors for additional correlation.-->




