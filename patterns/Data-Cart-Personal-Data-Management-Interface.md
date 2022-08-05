{%hyde _metadata blocks must begin with this_

title: "Data Cart Personal Data Management Interface"
type: pattern
excerpt: "Help data processing employees in the privacy-compliant handling of personal data by providing them with a privacy enhancing personal data management interface."

categories: 
  - enforce
  - demonstrate

status: draft _values allowed: stub, draft, published_ 

address: @jatoko

%}

[TOC]

<!--### [Also Known As]-->
<!-- All other names the pattern is known by.-->



## Summary
<!-- One short paragraph summarising the pattern.-->

A privacy enhancing personal data management interface that helps [data processing employees](a "An employee who processes personal data under the authority of their employer.") gather and manage personal data in a privacy-compliant manner.

## Context
<!-- The situations in which the pattern may apply.-->

This pattern applies to data processing employees working in organizations that elicit personal data as a part of an overarching business process, and must share the personal data with other entities or departments as part of this business process. Elicitation is usually done in structured surveys through forms, or by requesting the personal data from other departments within the organization. The pattern has been evaluated with data processing employees from public institutions who mainly process employee personal data.

<table>
<thead>
  <tr>
    <th>Attribute</th>
    <th>Description</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Target stakeholders</td>
    <td>Data processing employees</td>
  </tr>
  <tr>
    <td>Category of controller</td>
    <td>Public institutions</td>
  </tr>
  <tr>
    <td>Processing purposes</td>
    <td>Academic services, consulting and coaching, event management, monitoring activities, patent registration and exploitation, project management</td>
  </tr>
  <tr>
    <td>Categories of personal data</td>
    <td>Contact, education, finances, personal identifiers, pictures, professional activity</td>
  </tr>
  <tr>
    <td>Data subjects</td>
    <td>Employees, other members of the institution, (external parties)</td>
  </tr>
  <tr>
    <td>Categories of recipients</td>
    <td>Employees, service providers, authorities, public institutions</td>
  </tr>
  <tr>
    <td>Data sources</td>
    <td>Data subjects, supervisors, HR Department</td>
  </tr>
</tbody>
</table>

## Problem
<!-- The problem a pattern addresses, including a list of forces describing why a problem might be difficult to solve.-->

Data processing employees are frequently required to process personal data for (time-critical) job tasks, which necessitates extensive communication with an organization's employees, departments, and partners. In an organization, particularly heterogeneous business processes prevent effective data inquiries, either because the data received are incomplete and incorrect, or because the correct contact person in other departments is unknown. In many of these cases, data processing employees perceive data protection as a burden because they are uncertain whether they act in compliance with data protection, or whether certain measures are necessary, and how they should put them into practice. In practice, data processing employees thus act with uncertainty and make efforts to protect themselves from misconduct that they do not know are necessary or even correct. As a result, employers, as [data controllers](a "'the natural or legal person, public authority, agency or other body which [...] determines the purposes and means of the processing of personal data' (Art. 4 (7) GDPR)") thus liable for the actions of their employees, may subsequently fail to comply with their accountability obligations.

## Solution
<!-- A concise description of how the pattern addresses the problem.-->

Provide a privacy enhancing personal data management interface to personal data that:

1. streamlines data collection processes in organizations and aligns them with data protection requirements;
2. standardizes access to personal data for data processing employees;
3. simplifies access to privacy policies for data processing employees; 
4. and supports both controllers and data processing employees in demonstrating transparency and compliance by documenting processing activities.

### [Structure]
<!--A detailed specification of the structural aspects of the pattern. A class diagram if applicable.-->

The pattern is a harmonized combination of process flow and interaction concept:

#### [Process flow]

1. The first process step requires data processing employees to model a data processing activity to be performed. They must choose a processing activity from the organization's [records of processing activities](a "Art. 30 GDPR") that must be maintained by all data controllers with regular processing activities. Each entry comprises a purpose, categories of personal data, categories of data subjects, categories of recipients, legal basis, and, if applicable, further information on technical and organizational measures. 

2. In the second process step, data processing employees define tuples of required categories of personal data and data subjects. They may also add additional details, such as specific recipients, the version of personal data they require, or a personal message to the data source (e.g., data subject, department). Once finished, the modeled processing activity is to be submitted as a new data processing request.

3. The submitted processing request is validated by verifying for lawfulness of processing against the processing policies extracted from the record of processing activities and by checking the availability and timeliness of the personal data requested.

4. The next process step comprises obtaining missing personal data and permissions. Depending on the processing activity, this may require initiating requests to the respective data subjects or departments to provide the missing data and approvals.

5. After all tasks have been completed, data processing employees get access to a privacy enhancing personal data management interface. It provides access to metadata of the data processing request, including status information and details about the tuples requested. In addition, it provides access to contextual privacy policies and reminders extracted from the organizations' directory of processing records. Furthermore, the interface provides the ability to request additional combinations of personal data and data subjects, and to request access to the personal data (e.g., exports).

6. To access raw personal data, data processing employees must choose a specific purpose for which they require the data. Based on this, they should be provided with an export of the personal data, which contains only the data authorized for the purpose and recipients. The export should be adequately protected by default, as data processing employees may not have the necessary knowledge to do this themselves.

7. All actions, including requests for data and data exports, are logged to document all personal data processing activities. After completing a processing activity, requests can be archived and serve as evidence for later audits and traceability. In addition, the activity log may be used to create a usage history for data processing employees.

![Data Cart process flow](media/images/data_cart_process_flow.png)

#### [UI concept]

1. Data processing employees should be offered a personal data management tool that provides for centralized access to personal data and enforces consistency of the full data management process.

2. To model a data processing request, data processing employees should be provided with a preloaded list of processing activities for which they are authorized. Upon selection, employees should be provided with a summary of the processing record. In addition, the planned processing must be given a name and a description. These steps require employees to become aware of the legal basis before processing begins. At the same time, the interaction concept provides for contextual support, such as providing templates and contextual information. Templates may be based on previous requests.

3. To define tuples of personal data and data subjects, data processing employees should be provided with predefined lists. For personal data, these lists may be derived from the selected processing record entry and should be offered as a pre-selection. The interface should further support the iterative adding of multiple different combinations.

4. When submitting the request for validation, the results should be provided for review in an overview. It should include status information on whether the processing activity can start immediately after submission of the processing request, or whether additional actions are required, such as collecting personal data or obtaining consent. Detailed status information should be accessible as needed. At this point, further information may be added to the request.

5. The privacy enhancing data management interface should provide detailed information on the status of pending requests. In addition, it should provide frequently needed or important information on data protection tailored to its users' needs. This includes information on allowed processing operations, whether processing has been approved, to whom data may be disclosed, deletion periods, data sensitivity, and how data must be safeguarded. In general, the interface should aim to provide such notices at a glance, with details accessible when necessary. Additional visualizations and a help section for questions should accompany detail views.

![Data Cart UI concept](media/images/data_cart_ui_concept.png)

<!--### [Implementation]-->
<!--Guidelines for implementing the pattern; code fragments; suggested PETS; policy fragments.-->



## Consequences
<!--The advantages (benefits) and disadvantages (liabilities) of applying the pattern.-->

The pattern help address the following [GDPR principles](a "'Principles relating to processing of personal data' (Art. 5 GDPR)"):

*Lawfulness* and *purpose limitation* are addressed by reducing human error due to employee's ignorance, since information about the legal basis and purpose become an integral part of any request for personal data;

*Data minimization* and *accuracy* are achieved through (1) centrally controlled access to personal data, (2) provision of meta-information about personal data, and (3) triggering of updates for personal data; 

*Storage limitation* and *integrity and confidentiality* are supported by incorporating the principle of *privacy by default* (e.g., encryption of exports) and notices on the correct handling of personal data;

*Fairness and transparency* and *accountability* are supported by the implicit documenting of requests for personal data. *Accountability* is further addressed by making data processing employees aware of personal data processing obligations through clear and uniform privacy notices.

### [Constraints]
<!-- limitations as a consequence of applying the pattern.-->
Applying the pattern is constraint by potential integration barriers, especially if tools incorporating this pattern are introduced as a supplement to existing processes or current workflows. Further problems may arise from a lack of digitalization in organizations, which could cause a significant overhead in both the integration and operation. Further issues may result from the consequences enforcing a specific way of managing personal data that might require additional change management efforts.


## Examples
<!--Motivational example to see how the pattern is applied.-->

Select processing activitiy             |  Add tuples of personal data and data subjects | Personal data management interface
:-------------------------:|:-------------------------:|:-------------------------:
<img src="/media/images/data_cart_screen_01.png" alt="Data Cart Screen 01" width="100"/>  |  <img src="/media/images/data_cart_screen_02.png" alt="Data Cart Screen 01" width="100"/> | <img src="/media/images/data_cart_screen_01.png" alt="Data Cart Screen 03" width="100"/>

<!--### [Known Uses]-->
<!-- Pointers to various applications of the pattern.-->



## See Also
<!-- Any pointers to relevant information, not contained in the subfields below.-->

This pattern generally supports design strategies *minimize*, *inform*, and *control*.


<!--### [Related Patterns]-->
<!-- Supporting and conflicting patterns-->



### [Sources]
<!-- References to the original source of the pattern.-->

Original work:

J. Tolsdorf, F. Dehling, und L. Lo Iacono, "Data Cart – designing a tool for the GDPR-compliant handling of personal data by employees", Behaviour & Information Technology (BIT), p. 1–36, May 2022, doi: [10.1080/0144929X.2022.2069596](https://doi.org/10.1080/0144929X.2022.2069596)

Prototype and study material (German only): 

J. Tolsdorf, "Data Cart Study Material for Study 4 Usability Study", GRO.data, V1, 2022, doi: [10.25625/PMQC0P](https://doi.org/10.25625/PMQC0P)

<!-- ## General Comments -->
<!-- Separate discussion on the pattern.-->



<!--## Tags-->
<!-- User definable descriptors for additional correlation.-->
