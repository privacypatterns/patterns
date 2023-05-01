    {%hyde

    title: "Polling Pattern"
    type: pattern
    excerpt: "Actively request information at intervals."
    categories: 
        - minimize
        - seperate
    use: User-data-confinement-pattern
    ref: Minimal-Information-Asymmetry
    status: draft
    %}

[TOC]

<!--### [Also Known As]-->
<!-- All other names the pattern is known by.-->

## Summary
<!-- One short paragraph summarising the pattern.-->
A data-observer requests information from a data-informant at regular intervals.
The parties can deny access to the information or stop requesting information at any time.

## Context
<!-- The situations in which the pattern may apply.-->
Data-observants, such as service providers, often collect personal data in order to take actions on behalf of data-informants, such as users, as part of their services.
E.g. payment-information or names and email-adresses. 

## Problem
<!-- The problem a pattern addresses, including a list of forces describing why a problem might be difficult to solve.-->
Revoking access to personal data is made difficult for data-informants, as their data is stored elsewhere; out-of-view and control of the data-informants.

## Solution
<!-- A concise description of how the pattern addresses the problem.-->
Let actions that require the use of personal data be carried out directly by the data-informants. 
Then queury the status by requesting information at regular intervals.

<!--goals-->
Personal data is not shared with the service provider and either party in the data-transaction can deny access to information, or stop requesting information.

<!--### [Structure]-->
<!--A detailed specification of the structural aspects of the pattern. A class diagram if applicable.-->

<!--### [Implementation]-->
<!--Guidelines for implementing the pattern; code fragments; suggested PETS; policy fragments.-->

## Consequences
<!--The advantages (benefits) and disadvantages (liabilities) of applying the pattern.-->
- Users are to a higher degree in control of their data. 
- There may be more possibilities for running processes on the client-side.
- Service providers can avoid legal complications related to the processing of personal data, when data is not collected.

### [Constraints]
<!-- limitations as a consequence of applying the pattern.-->
- This pattern can be computationally inefficient, as the parties do not know in advance when there is new information,
and thus potentially initiates communication in vain.
- In cases where the user needs to query for information, the use of this pattern may necessitate special software that can do this automatically.


## Examples
<!--Motivational example to see how the pattern is applied.-->
Recurring payments on the web, often relies on the user exposing credit card information to a private company in the form of a payment provider.
Using a polling-pattern users would instead make payments to a service provider on a specified account or with specified transaction meta-data.
The service provider would then allow access to the service for as long as it receives payments.
One possible implementation would be setting up a Cron job that regularily checks if a payment has been made, and revokes access to the service if no payment is found.

### [Known Uses]
<!-- Pointers to various applications of the pattern.-->
Contrary to a newsletter, RSS uses a polling-pattern where instead of giving up a personal email-adress, users queury for updates on specific end-points made available by the service providers.

<!--## See Also-->
<!-- Any pointers to relevant information, not contained in the subfields below.-->



### [Related Patterns]
<!-- Supporting and conflicting patterns-->
This pattern _refines_ [Minimal Information Asymmetry](patterns/Minimal-Information-Asymmetry.md) as it provides a more specific solution to exposing less personal data to service providers.

This pattern _uses_ [User Data Confinement](patterns/User-data-confinement-pattern.md) as it is necessary to move processing from server- to client-side when implementing a polling-pattern.


<!--### [Sources]-->
<!-- References to the original source of the pattern.-->



<!--## General Comments-->
<!-- Separate discussion on the pattern.-->



<!--## Tags-->
<!-- User definable descriptors for additional correlation.-->
