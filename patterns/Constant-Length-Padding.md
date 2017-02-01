    {%hyde

    title: "Constant Length Padding"
    type: pattern
    excerpt: "Suggests making the size of data packets the same in a mix network."
    categories:
        - 
    status: draft
    address:

    %}

[TOC]


##Name
<!--Primary name the pattern is known by.-->

Constant Length Padding

<!--###[Also Known As]-->
<!-- All other names the pattern is known by.-->



##Summary
<!-- One short paragraph summarising the pattern.-->

Suggests making the size of data packets the same in a mix network.

##Context
<!-- The situations in which the pattern may apply.-->

In a mix network, incoming packets may be modified to each have the same length when dispatched to prevent association

##Problem
<!-- The problem a pattern addresses, including a list of forces describing why a problem might be difficult to solve.-->

A mix network uses Layered Encryption to protect packet headers and data. However, meta-information about packet content can be leaked from packet size. [An] adversary [should] be [unable] to exploit the size variation in data traffic

##Solution
<!-- A concise description of how the pattern addresses the problem.-->

Make the length of all packets the same. If needed, add padding to data packets. Mixmaster, Mixminion, Babel and Tarzan [break] data into uniform-sized packets, and [pad] the packets to a uniform size. In practice, cyphertext is usually somewhat longer than cleartext. Chaum suggests breaking data into fixed size blocks and pad them.

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




