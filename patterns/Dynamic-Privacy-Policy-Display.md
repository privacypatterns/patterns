    {%hyde

    title: "Dynamic Privacy Policy Display"
    type: pattern
    excerpt: "Display a tooltip to the user when his attention is required for privacy matters, e.g., person data are requested by a website."
    categories:
        - 
    status: stub
    address:

    %}

[TOC]


##Name
<!--Primary name the pattern is known by.-->

Dynamic Privacy Policy Display

<!--###[Also Known As]-->
<!-- All other names the pattern is known by.-->



##Summary
<!-- One short paragraph summarising the pattern.-->

Display a tooltip to the user when his attention is required for privacy matters, e.g., person data are requested by a website.

##Context
<!-- The situations in which the pattern may apply.-->

Dynamic privacy policy displays can be applied to small interfaces (e.g., login) or when the credential selection contains information that needs the user's attention.

##Problem
<!-- The problem a pattern addresses, including a list of forces describing why a problem might be difficult to solve.-->

Users need to be well informed about possible consequences when releasing personal data upon certain actions such as login, registration, payments, etc. Art. 25 requires that data subjects are at least informed about what personal data are processed, by whom (i.e., the identity of the controller), and for what purposes.

##Solution
<!-- A concise description of how the pattern addresses the problem.-->

The multi-layered presentation approach by the Article 29 Working Party can be implemented by dynamical information “tooltips” informing the user about the nature of the data disclosed and possible consequences. The dynamic information need to be adapted to the context of the website it is used in. It should only include relevant security and privacy information and have a unique standard layout making it easy to recognize.

###[Structure]
<!--A detailed specification of the structural aspects of the pattern. A class diagram if applicable.-->

Because of peripheral viewing, the user is able to recognize visual change (i.e., motion) even when on the border of the field of view. The user will recognize each visual change and might automatically connect it to danger. Hence, he will immediately notice the visual change and direct the attention to it. Using this approach, it is increasingly unlikely that the user might oversee the privacy indications.

###[Implementation]
<!--Guidelines for implementing the pattern; code fragments; suggested PETS; policy fragments.-->

The information should be provided to the user where it is needed. Therefore the tooltip should appear on demand (i.e., need of information). This could be for example in a login dialog as soon as the user navigates the mouse into the concerning part of the interface. The tooltip should then be made visible to the user and contain all necessary information for making an informed decision.

##Consequences
<!--The advantages (benefits) and disadvantages (liabilities) of applying the pattern.-->

By displaying the relevant (sections of) privacy policies whenever they apply to what the user is currently doing or about to do, the user's awareness of what will happen with the information they're about to share is increased.

<!--###[Constraints]-->
<!-- limitations as a consequence of applying the pattern.-->



<!--##Examples-->
<!--Motivational example to see how the pattern is applied.-->



<!--###[Known Uses]-->
<!-- Pointers to various applications of the pattern.-->



<!--##See Also-->
<!-- Any pointers to relevant information, not contained in the subfields below.-->



###[Related Patterns]
<!-- Supporting and conflicting patterns-->

Privacy Policy DisplayPrivacy Policy Display

###[Sources]
<!-- References to the original source of the pattern.-->

C. Graf, P. Wolkerstorfer, A. Geven, and M. Tscheligi, “A Pattern Collection for Privacy Enhancing Technology,” The Second International Conferences of Pervasive Patterns and Applications (Patterns 2010), vol. 2, no. 1, pp. 72–77, 2010.

<!--##General Comments-->
<!-- Separate discussion on the pattern.-->



<!--##Categories-->
<!-- Placeholder for future agreed upon categories as per collaboration's evaluation.-->

<!--##Tags-->
<!-- User definable descriptors for additional correlation.-->




