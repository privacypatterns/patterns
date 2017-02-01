    {%hyde

    title: "Chaining"
    type: pattern
    excerpt: "Anonymity solutions should be applied in layers to have defense in depth. Even if one anonymity solution fails, another mechanism will maintain the anonymity cover."
    categories:
        - 
    status: draft
    address:

    %}

[TOC]


##Name
<!--Primary name the pattern is known by.-->

Chaining

<!--###[Also Known As]-->
<!-- All other names the pattern is known by.-->



##Summary
<!-- One short paragraph summarising the pattern.-->

Anonymity solutions should be applied in layers to have defense in depth. Even if one anonymity solution fails, another mechanism will maintain the anonymity cover.

##Context
<!-- The situations in which the pattern may apply.-->

In a mix network, multiple strategies, namely mutliple pseudonyms and mixes, may be used in conjunction on packets to prevent association even if there is a weakness in the chain

##Problem
<!-- The problem a pattern addresses, including a list of forces describing why a problem might be difficult to solve.-->

A single anonymity solution may not guarantee strong privacy. For example, an attacker may observe the incoming and outgoing traffic of a single mix node, or even perturb the traffic (e.g., blending attack) to compromise anonymity. Users should also not trust a single mix network, because it may be owned by an active adversary

##Solution
<!-- A concise description of how the pattern addresses the problem.-->

Adopt multiple instances of an anonymity mechanism in layers. Chain multiple mix nodes instead of one and route traffic through multiple nodes. Adopt multiple pseudonym covers to protect users. Adversaries can simply observe incoming and outgoing traffic of a single-point anonymizer, and correlate the encrypted incoming traffic to an anonymizer with the unencrypted traffic going to a receiver by timing analysis. Chaining makes this type of analysis difficult by introducing multiple intermediaries. Furthermore, it protects user anonymity even if a single mix in the entire chain is honest.

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




