 {%hyde

    title: "Pub-Sub Pattern"
    type: pattern
    excerpt: "Mediate information through impartial actor."
    categories: 
        - control
        - seperate
    sim: Onion Routing
    com: Pseudonymous Messaging
    com: Single Point of Contact
    status: draft
    %}

[TOC]

<!--### [Also Known As]-->
<!-- All other names the pattern is known by.-->

## Summary
<!-- One short paragraph summarising the pattern.-->
A publishing party sends information to an intermediate message broker, who relays this information to all participants that indicate their willingness to receive this information

## Context
<!-- The situations in which the pattern may apply.-->
Often service providers want to be able to contact users, also when users are not actively engaging with the product.
Likewise, users may wish to recieve information from service providers. For this reason many service providers collect personal information in the form of emails or phone numbers.

## Problem
<!-- The problem a pattern addresses, including a list of forces describing why a problem might be difficult to solve.-->
Revoking access to personal data is made difficult for data-informants, as their data is stored elsewhere; out-of-view and control of the data-informants.

## Solution
<!-- A concise description of how the pattern addresses the problem.-->
Users should not share personal information with service providers. Instead service providers may publish updates on a certain _channel_ that users can subscribe and unsubscribe to as they desire.

<!--goals-->
Personal data is not shared with service providers and either party can chose to disengage from the information transactions at any point.

### [Structure]
<!--A detailed specification of the structural aspects of the pattern. A class diagram if applicable.-->
The pattern introduces an additional actor in the information transaction, i.e. a message broker who relays information.
The message broker will relay information to actors that have indicated that they wish to receive these updates. 

### [Implementation]
<!--Guidelines for implementing the pattern; code fragments; suggested PETS; policy fragments.-->
The message broker may be implemented as an independent third party, a decentralized network, or even by the user himself.

## Consequences
<!--The advantages (benefits) and disadvantages (liabilities) of applying the pattern.-->
- Users avoid sharing sensitive information with service providers.
- Users can easily unsubscribe from information.
- Service providers can avoid legal complications related to the processing of personal data, when data is not collected.

### [Constraints]
<!-- limitations as a consequence of applying the pattern.-->
- May require end-to-end-encryption or trust in message brokers.
- This pattern may necessitate special client software.
- Encreased setup time as the channel must first be established.


## Examples
<!--Motivational example to see how the pattern is applied.-->
It is possible for the user to emulate a pub-sub pattern by creating a pseudonymous email address with forwarding to the user's real email address for each service he/she uses. The user can unsubscribe from updates from certain
service providers by deactivating the forwarding of emails from the corresponding pseudonymous email address. Something similar exists for credit cards, where a virtual credit card can be used to hide information about the real physical credit card.

### [Known Uses]
<!-- Pointers to various applications of the pattern.-->
Push notifications are a notification that appears on the home screen of the user's mobile device. Push notifications on the web, i.e. The Web Push API allows users to grant or revoke permission for a specific service provider to send them push messages. This is enforced by each browser's Push Message Provider.

<!--## See Also-->
<!-- Any pointers to relevant information, not contained in the subfields below.-->



### [Related Patterns]
<!-- Supporting and conflicting patterns-->
This pattern is _similar to_ [Onion Routing](patterns/Onion-routing.md) as data is moved through additional layers in an attempt to hide the final destination.

This pattern _compliments_ [Pseudonymous Messaging](patterns/Pseudonymous-messaging.md) and [Single Point of Contact](patterns/Single-Point-of-Contact.md) as these patterns can work together to solve the problem of data asymmetry between users and data processors. 


<!--### [Sources]-->
<!-- References to the original source of the pattern.-->



<!--## General Comments-->
<!-- Separate discussion on the pattern.-->



<!--## Tags-->
<!-- User definable descriptors for additional correlation.-->
