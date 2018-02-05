    {%hyde

    title: "Dynamic Privacy Policy Display"
    type: pattern
    excerpt: "Provide standardized contextual policy information on the nature and risks of disclosure through tooltips."
    categories:
        - inform
        - notify
    status: pattern
    address:

    %}

[TOC]

<!--### [Also Known As]-->
<!-- All other names the pattern is known by.-->



## Context
<!-- The situations in which the pattern may apply.-->
<!-- Aspects which constrain the solution, but are not modified by it. They affect the impact of different forces.-->

Controllers are mandated by various laws and regulations to ensure that users, their data subjects, are adequately informed before requesting consent. Failing this, the consent loses legitimacy and the controller may face repercussions. However, the main mechanism for supplying this information resides with privacy policies, which must also conform to legislative norms. The language this necessitates is long and complex, which jeopardizes the chances of users understanding it. This information can be summarized, and otherwise reworded to make the content more accessible to users, though typically the length of such summaries are still quite long.

## Problem
<!-- The problem a pattern addresses, including a list of forces describing why a problem might be difficult to solve.-->

Not all contexts are suitable for extensive privacy policy information, yet users often still need to be able to obtain additional data without breaking those contexts.

#### Forces and Concerns
<!-- Implications in this problem which affect the appropriateness of a solution, and are affected by this pattern.-->
<!-- Forces should be highly visible for easy reference, where less obvious a dedicated section is recommended.-->
- Controllers need to comply with the laws mandating informed consent, but users do not read privacy policies
- Users do not want to spend time and effort reading through privacy policies
- Controllers want users to actually use their service (or product), but users will not do so if the cost of doing so entails disproportionate effort
- Users want to be able to get to using the service quickly

## Solution
<!-- A concise description of how the pattern addresses the problem.-->

Provide the user with additional relevant policy information on hover or tap, by way of 'tooltips', to best inform them given contextual limitations.

This information may highlight the nature and potential consequences of the disclosure, and should be displayed consistently.

<!--### [Structure]-->
<!--A detailed specification of the structural aspects of the pattern. A class diagram if applicable.-->



### [Implementation]
<!--Guidelines for implementing the pattern; code fragments; suggested PETS; policy fragments.-->

_The information should be provided to the user where it is needed. Therefore the tooltip should appear on demand (i.e., need of information). This could be for example in a login dialog as soon as the user navigates the mouse into the concerning part of the interface. The tooltip should then be made visible to the user and contain all necessary information for making an informed decision._

## Consequences
<!--The advantages (benefits) and disadvantages (liabilities) of applying the pattern.-->

_By displaying the relevant [information pertaining to] privacy policies whenever they apply to what the user is currently doing or about to do, the user's awareness of what will happen with the information they're about to share is increased._

However, users may also happen to not trigger the tooltip, especially when using a mobile device. As such it is important that they are aware of its existence, and its importance, given the current context.

<!--### [Constraints]-->
<!-- limitations as a consequence of applying the pattern.-->



<!--## Examples-->
<!--Motivational example to see how the pattern is applied.-->



<!--### [Known Uses]-->
<!-- Pointers to various applications of the pattern.-->



<!--## See Also-->
<!-- Any pointers to relevant information, not contained in the subfields below.-->



<!--### [Related Patterns]-->
<!-- Supporting and conflicting patterns-->
<!-- These relationships are still under review -->
### [Sources]
<!-- References to the original source of the pattern.-->

S. Fischer-Hübner, C. Köffel, J.-S. Pettersson, P. Wolkerstorfer, C. Graf, L. E. Holtz, U. König, H. Hedbom, and B. Kellermann, “HCI Pattern Collection - Version 2,” 2010.

C. Graf, P. Wolkerstorfer, A. Geven, and M. Tscheligi, “A Pattern Collection for Privacy Enhancing Technology,” The Second International Conferences of Pervasive Patterns and Applications (Patterns 2010), vol. 2, no. 1, pp. 72–77, 2010.

<!--## General Comments-->
<!-- Separate discussion on the pattern.-->



<!--## Tags-->
<!-- User definable descriptors for additional correlation.-->




