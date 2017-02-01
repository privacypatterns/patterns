    {%hyde

    title: "K-anonymity"
    type: pattern
    excerpt: "Make unique identification of people in an anonymized dataset impossible by having potentially identifying attribute combinations always link to at least k entries."
    categories:
        - 
    status: draft
    address:

    %}

[TOC]


##Name
<!--Primary name the pattern is known by.-->

K-anonymity

<!--###[Also Known As]-->
<!-- All other names the pattern is known by.-->



##Summary
<!-- One short paragraph summarising the pattern.-->

Make unique identification of people in an anonymized dataset impossible by having potentially identifying attribute combinations always link to at least k entries.

##Context
<!-- The situations in which the pattern may apply.-->

Data sets that have been anonymized before being transferred to another organization, or sold on the commercial market.

##Problem
<!-- The problem a pattern addresses, including a list of forces describing why a problem might be difficult to solve.-->

Even when data has been anonymized, people can often be uniquely identified through inference of the data that remains in the data set with other (anonymized) datasets.

##Solution
<!-- A concise description of how the pattern addresses the problem.-->

If RT is a dataset and QI_RT is a quasi-identifier (a set of attributes in RT that could potentially identify an individual in RT), then if a certain combination of values for the attributes in QI_RT exists in RT, that combination of values must occur in at least k entries. Only if an anonymized dataset satisfies this property may it be released.

<!--###[Structure]-->
<!--A detailed specification of the structural aspects of the pattern. A class diagram if applicable.-->



<!--###[Implementation]-->
<!--Guidelines for implementing the pattern; code fragments; suggested PETS; policy fragments.-->



##Consequences
<!--The advantages (benefits) and disadvantages (liabilities) of applying the pattern.-->

The primary problem of k-anonymity is determining quasi-identifiers, those combinations of attributes that could potentially identify individuals. Predicting every possible inference attack with a dataset is virtually impossible, as it may always be possible to identify individuals by inferring the dataset with another dataset in a way that was not predicted. If quasi-identifiers are correctly picked, k-anonymity does protect against direct matching, and at least prevents anonymity violation by inference attacks of that kind.

<!--###[Constraints]-->
<!-- limitations as a consequence of applying the pattern.-->



##Examples
<!--Motivational example to see how the pattern is applied.-->

Datafly (Sweeney 1997), mu-Argus (Hundepool, Willenborg 1996), k-Similar (Sweeney 1998)

<!--###[Known Uses]-->
<!-- Pointers to various applications of the pattern.-->



<!--##See Also-->
<!-- Any pointers to relevant information, not contained in the subfields below.-->



<!--###[Related Patterns]-->
<!-- Supporting and conflicting patterns-->



###[Sources]
<!-- References to the original source of the pattern.-->

L. Sweeney, “k-ANONYMITY: A MODEL FOR PROTECTING PRIVACY,” International Journal of Uncertainty, Fuzziness and Knowledge-Based Systems, vol. 10, no. 5, pp. 557–570, 2002.

J. H. Hoepman, “Privacy design strategies,” IFIP SEC 2014, 2014.

<!--##General Comments-->
<!-- Separate discussion on the pattern.-->



<!--##Categories-->
<!-- Placeholder for future agreed upon categories as per collaboration's evaluation.-->

<!--##Tags-->
<!-- User definable descriptors for additional correlation.-->




