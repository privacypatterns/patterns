    {%hyde

    title: "Morphed Representation"
    type: pattern
    excerpt: "Change the representation of the data when it is passing through an anonymity providing node so that outgoing data cannot be linked with incoming data."
    categories:
        - 
    status: stub
    address:

    %}

[TOC]


##Name
<!--Primary name the pattern is known by.-->

Morphed Representation

###[Also Known As]
<!-- All other names the pattern is known by.-->

Werewolf / Gate of Heaven / Dr. Jekyll and Mr. Hyde / Amoeboid Shape / Psuedo Identities / Identity Separation

##Summary
<!-- One short paragraph summarising the pattern.-->

Change the representation of the data when it is passing through an anonymity providing node so that outgoing data cannot be linked with incoming data.

##Context
<!-- The situations in which the pattern may apply.-->

Designing a mix based system to protect the privacy of the users with sender anonymity and sender and receiver unlinkability for the communicating parties. The mix based system can be a mix based filter in the Internet messaging domain that is used for email messaging or web browsing

##Problem
<!-- The problem a pattern addresses, including a list of forces describing why a problem might be difficult to solve.-->

Mix networks combine the data from a sender with the data coming from multiple other sources and send them together. The incoming data packets carry the data content. They also have metacharacteristics associated like the time of packet generation, ingress order of packets etc. The mix network obfuscates these metacharacteristics by adding random delays to the ingress packets, or by batching a number of ingress packets before releasing the packets. However, if themix concepts do not obfuscate the data content, the incoming and outgoing data packets have the same representation and they can be correlated trivially. 

##Solution
<!-- A concise description of how the pattern addresses the problem.-->

Change the representation of the incoming data packet such that the outgoing packets look different from incoming packets. The incoming packets are encrypted using a key shared between the sending node and themix node. At themix node, decrypt the packet and then re-encrypt itwith the key shared between themix node and the subsequent node. Use symmetric keys for encryption to avoid the expensive primary key operations. The nodes set up a key share with all its neighbors

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

<!--##General Comments-->
<!-- Separate discussion on the pattern.-->



##Categories
<!-- Placeholder for future agreed upon categories as per collaboration's evaluation.-->
Hide
Mix

<!--##Tags-->
<!-- User definable descriptors for additional correlation.-->




