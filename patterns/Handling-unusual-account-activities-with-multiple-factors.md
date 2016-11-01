    {%hyde

    title: "Handling unusual account activities with multiple factors"
    type: pattern
    excerpt: "For Internet services, prevent suspicious access to the account, and/or make the account owner aware of unusual activities."
    categories:
        - 
    status: stub
    address:

    %}

[TOC]


##Name
<!--Primary name the pattern is known by.-->

Handling unusual account activities with multiple factors

<!--###[Also Known As]-->
<!-- All other names the pattern is known by.-->



##Summary
<!-- One short paragraph summarising the pattern.-->

For Internet services, prevent suspicious access to the account, and/or make the account owner aware of unusual activities.

##Context
<!-- The situations in which the pattern may apply.-->

Many Internet services are using password-based authentication which is really convenient (compared to strong authentication) but has apparent drawbacks: The password itself does not change, can be cracked, cannot be ensured to be exclusive, can only change access control through resets, and is susceptible to shoulder surfing.

##Problem
<!-- The problem a pattern addresses, including a list of forces describing why a problem might be difficult to solve.-->

How can a service that uses username-password authentication and involves a lot of privacy identify unusual sign-ins, confirm the identify of the user, and inform the account owner of such unusual activities?

##Solution
<!-- A concise description of how the pattern addresses the problem.-->

The service should be able to identify unusual sign-ins through new country/browser/operating system accesses, and in the local application context assess environment variables and hardware parameters. Then the service may use multi-factor authentication to confirm the identity of the user beyond the use of a password, with tokens (SW/HW/dis/connected), secret personal data, or one-time passwords through alternative mediums. Finally, subjects should be notified and given tools to respond to unusual activity.

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

N. Doty, M. Gupta, and J. Zych, “PrivacyPatterns.org.” [Online]. Available: http://privacypatterns.org/. [Accessed: 26-Feb-2015].

J. Polakis et al., “All Your Face Are Belong to Us: Breaking Facebook’s Social Authentication,” Proceedings of the Annual Computer Security Applications Conference (ACSAC), no. i, pp. 399–408, 2012.

<!--##General Comments-->
<!-- Separate discussion on the pattern.-->



##Categories
<!-- Placeholder for future agreed upon categories as per collaboration's evaluation.-->
Inform
Notify

<!--##Tags-->
<!-- User definable descriptors for additional correlation.-->




