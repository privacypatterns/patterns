    {%hyde

    title: "Data Abstraction"
    type: pattern
    excerpt: "Reduce ('abstract') collected raw data to a form in which it only contains the information that is necessary for processing, and it is ready to be processed."
    categories:
        - 
    status: stub
    address:

    %}

[TOC]


##Name
<!--Primary name the pattern is known by.-->

Data Abstraction

<!--###[Also Known As]-->
<!-- All other names the pattern is known by.-->



##Summary
<!-- One short paragraph summarising the pattern.-->

Reduce ('abstract') collected raw data to a form in which it only contains the information that is necessary for processing, and it is ready to be processed.

##Context
<!-- The situations in which the pattern may apply.-->

Data processing and data storage are the core features of nearly every system. Data processing can happen at different levels of abstraction. Data storage varies in the representational form

##Problem
<!-- The problem a pattern addresses, including a list of forces describing why a problem might be difficult to solve.-->

Undesired second-use of data is a great threat for privacy. While there are methods like access control to regulate who has access to data, it is not possible to define fine grained who is allowed to access which data, if data is stored and processed in a raw format. One of the most important gaps is the one between analog and digital processing. Analog data cannot always be split into data concerning different persons and different situations.It is also hard to assign low-level digital data (e.g., video streams) to well defined purposes and purpose-based processing tasks

##Solution
<!-- A concise description of how the pattern addresses the problem.-->

Data abstraction is one way to obtain structured data ready for sophisticated privacy annotations. Data abstraction is the reduction of data to the information needed and the preparation of data for the subsequent combination with other data. Data abstraction helps to prevent many privacy problems while at the same time obtain or even improve data usability. While raw data streams are hard to control by privacy measures, deduced objects, relationships and their properties can be supplemented by privacy properties. It is also possible to reveal only the data needed for a specific task, e.g. energy consumption in a 15 minute intervall or the location of a suspicious person observed. The workflow of the pattern is shown in Figure 4. Raw data is collected from real world, especially physical, data objects by digital or analog sensors. The collected data is either anolog like a voltage graph or low- level digital, e.g., a digitial image in an video stream. For further abstraction, analog data has to be preprocessed by an analog-to-digital converter. After the digital data is eventually collected, matching algorihms abstract the data to their final  representation which is used in the system. If data from different sources is necessary for a single purpose, data fusion takes place between data abstraction and data usage. Data fusion increases data quality and further decreases the amount of unnecesary information.

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
Abstract
Generalise

<!--##Tags-->
<!-- User definable descriptors for additional correlation.-->




