    {%hyde

    title: "Privacy Proxy"
    type: pattern
    excerpt: "Pass all data requests through a privacy proxy that takes care of privacy concerns before the data is submitted (such as access control, anonymization, abstraction etc)."
    categories:
        - 
    status: stub
    address:

    %}

[TOC]


##Name
<!--Primary name the pattern is known by.-->

Privacy Proxy

###[Also Known As]
<!-- All other names the pattern is known by.-->

Privacy Gateway / Privacy Manager

##Summary
<!-- One short paragraph summarising the pattern.-->

Pass all data requests through a privacy proxy that takes care of privacy concerns before the data is submitted (such as access control, anonymization, abstraction etc).

##Context
<!-- The situations in which the pattern may apply.-->

Modern information systems gather and process a lot of data. Commonly, data is shared between one or more servers, responsible for data storage, and the processing clients. Additionally, different systems need to communicate with each other, e.g., for accounting purposes.

##Problem
<!-- The problem a pattern addresses, including a list of forces describing why a problem might be difficult to solve.-->

While the transmission of data is a core concept in system design, it also involves multiple privacy issues. Therefore, data leaving the system has to be checked for the legitimacy of the data flow. The decision which data access is legitimate is highly system dependent and should be outsourced to an access control module. To enforce access control decisions done by the access decision module gets especially complicated when there are different types of receivers with diverse access rights. Additionally, the outgoing data has to be anonymized or otherwise preprocessed, according to the access rights. Using various communication protocols or multiple data storages worsens the problem.

##Solution
<!-- A concise description of how the pattern addresses the problem.-->

A single privacy proxy is encouraged to enforce access control decisions. The central privacy proxy is responsible to check every request for data. Therefore it has to communicate with any kind of clients desired. When heterogeneous communication protocols are used by different clients, the privacy proxy can be extended as needed with protocol translators. They are responsible for translating between different communications protocols, enabling a simpler design for the proxy. When complex database structures are used, the privacy proxy can be equipped with data collectors which are responsible to collect the data from different data sources. To keep the privacy proxy unified, access control decisions, anonymization and other measures should be outsourced to specialized components, seconding the privacy proxy (consider the related patterns).

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

C. Bier and E. Krempel, “Common Privacy Patterns in Video Surveillance and Smart Energy,” in ICCCT-2012, 2012, pp. 610–615.

<!--##General Comments-->
<!-- Separate discussion on the pattern.-->



##Categories
<!-- Placeholder for future agreed upon categories as per collaboration's evaluation.-->
Hide
Restrict

<!--##Tags-->
<!-- User definable descriptors for additional correlation.-->




