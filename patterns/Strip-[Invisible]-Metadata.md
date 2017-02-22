    {%hyde

    title: "Strip [Invisible] Metadata"
    type: pattern
    excerpt: "Metadata that is not needed and poses a potential threat to privacy should be hidden."
    categories:
        - 
    status: draft
    address:

    %}

[TOC]


##Name
<!--Primary name the pattern is known by.-->

Strip [Invisible] Metadata

<!--###[Also Known As]-->
<!-- All other names the pattern is known by.-->



##Summary
<!-- One short paragraph summarising the pattern.-->

Metadata that is not needed and poses a potential threat to privacy should be hidden.

##Context
<!-- The situations in which the pattern may apply.-->

This pattern is applicable in a system in which metadata is shared, published or sent. When a service requires a user to import data from external sources (eg. pictures, tweets, documents) different types of metadata may be transmitted. Users may not be aware of the metadata as it can be automatically generated or not directly visible. Services might be inadvertently responsible for exposing private metadata, or going against users' expectations.

##Problem
<!-- The problem a pattern addresses, including a list of forces describing why a problem might be difficult to solve.-->

There are multiple types of metadata. There is user-generated metadata data like exif-data. Exif is a format for storing metadata in pictures. There is also metadata which exists to ensure the functionality of some services like headers in email or http, or timestamps in files. Often the user is not aware of this additional data that is attached to the content. Much of this data is automatically generated, or not directly visible to users during their interactions. This can create situations where, even though users share information explicitly with services, they may be surprised to find this data being revealed. In certain cases where the data is legally protected, the service could be held responsible for any leakage of sensitive information. How should services that need users to share data and upload files treat additional metadata attached with files? In case of uploading documents and images, which parts of the metadata can be treated as explicitly shared information.

##Solution
<!-- A concise description of how the pattern addresses the problem.-->

Erase metadata which is not needed for the functionality. Stripping all metadata that is not directly visible during upload time, or during the use of the service can help protect services from leaks and liabilities. Even in cases where the information is not legally protected, the service can protect themselves from surprising their users and thus alienating them. Additionally when users share data with services, they can be presented with a preview of the data obtained by the service, including any metadata [[Preview Shared Data]]. This allows users to be more aware of information that they are sharing with the services, and in many cases with other entities on the Internet.To summarize: user metadata that can not be made visible to users clearly should be stripped to avoid overstepping the users' expectations.

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

C. Bier and E. Krempel, “Common Privacy Patterns in Video Surveillance and Smart Energy,” in ICCCT-2012, 2012, pp. 610–615.

“privacypatterns.eu - collecting patterns for better privacy.” [Online]. Available: https://privacypatterns.eu/. [Accessed: 20-Oct-2015].

<!--##General Comments-->
<!-- Separate discussion on the pattern.-->



<!--##Categories-->
<!-- Placeholder for future agreed upon categories as per collaboration's evaluation.-->

<!--##Tags-->
<!-- User definable descriptors for additional correlation.-->




