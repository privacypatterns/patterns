    {%hyde

    title: "Batched Routing"
    type: pattern
    excerpt: "Collect the input data packets, and when the collection reaches a limit, output all the datapackets together in a batch."
    categories:
        - 
    status: stub
    address:

    %}

[TOC]


##Name
<!--Primary name the pattern is known by.-->

Batched Routing

<!--###[Also Known As]-->
<!-- All other names the pattern is known by.-->



##Summary
<!-- One short paragraph summarising the pattern.-->

Collect the input data packets, and when the collection reaches a limit, output all the datapackets together in a batch.

##Context
<!-- The situations in which the pattern may apply.-->

In a mix network, incoming packets may be dispatched in batches to prevent association through k-anonymity

##Problem
<!-- The problem a pattern addresses, including a list of forces describing why a problem might be difficult to solve.-->

An anonymity set in a mix network is created by mixing a sender’s incoming packets with packets from other sources, and morphing data representation. However, there remains a strong causal relationship between between incoming and outgoing messages. Unless this relationship is hidden, an adversary can correlate input with output messages.

##Solution
<!-- A concise description of how the pattern addresses the problem.-->

In a mix network, different batching strategies can be adopted. A threshold mix collects n messages and flushes everything. A timed mix flushes the entire queue every t seconds. A mix can [also] combine the batching strategies. Crowds proxies forward web requests, and the final proxy in the path forwards a request to a server. It batches all the GETs and passes them together. Some location-based systems use [the] temporal cloaking mechanism

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
Mix

<!--##Tags-->
<!-- User definable descriptors for additional correlation.-->




