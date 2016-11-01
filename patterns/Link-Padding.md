    {%hyde

    title: "Link Padding"
    type: pattern
    excerpt: "Suggests keeping a constant [amount of] traffic on each outbound link in a mix."
    categories:
        - 
    status: stub
    address:

    %}

[TOC]


##Name
<!--Primary name the pattern is known by.-->

Link Padding

<!--###[Also Known As]-->
<!-- All other names the pattern is known by.-->



##Summary
<!-- One short paragraph summarising the pattern.-->

Suggests keeping a constant [amount of] traffic on each outbound link in a mix.

##Context
<!-- The situations in which the pattern may apply.-->

In a mix network, maintaining traffic flow even when no payload packets are incoming inhibits association

##Problem
<!-- The problem a pattern addresses, including a list of forces describing why a problem might be difficult to solve.-->

A passive adversary may monitor the input and output of an anonymity preserving node and be able to find the input and output correlation by monitoring the traffic flow variation in outgoing nodes. Generating cover traffic does not stop traffic analysis, if the cover traffic is only added to some links.

##Solution
<!-- A concise description of how the pattern addresses the problem.-->

Keep traffic flowing on all outbound links. Pad the links with cover traffic, even when actual payload is absent. Link Padding hides information about payload traffic, because the statistics of the total output traffic becomes significantly different from that of the payload traffic. [Heavy load] clock skew reveals payload information. Link padding with variable inter-arrival time between packets provides better protection. Again, keeping a constant flow has high cost, especially when packet flow is low. Adaptive link padding techniques tackle this issue.

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
Obfuscate

<!--##Tags-->
<!-- User definable descriptors for additional correlation.-->




