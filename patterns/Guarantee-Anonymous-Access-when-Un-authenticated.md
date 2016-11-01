    {%hyde

    title: "Guarantee Anonymous Access when Un-authenticated"
    type: pattern
    excerpt: "By filtering the identities of anonymous access attempts, clients who access the server anonymously will be unable to be identified."
    categories:
        - 
    status: stub
    address:

    %}

[TOC]


##Name
<!--Primary name the pattern is known by.-->

Guarantee Anonymous Access when Un-authenticated

<!--###[Also Known As]-->
<!-- All other names the pattern is known by.-->



##Summary
<!-- One short paragraph summarising the pattern.-->

By filtering the identities of anonymous access attempts, clients who access the server anonymously will be unable to be identified.

##Context
<!-- The situations in which the pattern may apply.-->

“Client” has the goal “Adhoc form request” that requires the resource “adhoc form” owned by “Server”. This goal contributes to the resource “connection information” “Server” has the goal “Record connections” that requires the resource “connection information”

##Problem
<!-- The problem a pattern addresses, including a list of forces describing why a problem might be difficult to solve.-->

Clients need to make anonymous connections to the Server for ad-hoc requests. Connections are recorded, for statistical purposes, but the identity of the Client s must not be recorded.

##Solution
<!-- A concise description of how the pattern addresses the problem.-->

To guarantee the ‘privacy’ property:Add the task ‘Identity Filter ’ to the Server. The Client trusts the task IF to remove his identity for anonymous access to the Server.

<!--###[Structure]-->
<!--A detailed specification of the structural aspects of the pattern. A class diagram if applicable.-->



<!--###[Implementation]-->
<!--Guidelines for implementing the pattern; code fragments; suggested PETS; policy fragments.-->



##Consequences
<!--The advantages (benefits) and disadvantages (liabilities) of applying the pattern.-->

If a client abuses their anonymous session to violate server rules or even laws, their activities can not be linked back to their identity.

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

Y. Asnar et al., “Initial Set of Security and Privacy Patterns at Organizational Level,” no. December 2006, 2007.

<!--##General Comments-->
<!-- Separate discussion on the pattern.-->



<!--##Categories-->
<!-- Placeholder for future agreed upon categories as per collaboration's evaluation.-->

<!--##Tags-->
<!-- User definable descriptors for additional correlation.-->




