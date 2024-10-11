Fusion ERP

Software Requirements Specification![](Aspose.Words.9d1f405d-75f7-4065-b965-602c621147db.001.png)

for

GAD-1-HR Module

Prepared by (**Web Team**):

Tushar Solanki(21bcs224) Akshay Pahuja(21bcs017) Samyak Jain(21bcs184) Arpit Yadav(21bcs035) Arpit Kumar(21bcs033)

**Table of Contents**

**Introduction**

Introduction about Fusion Purpose of the module Scope of the module

**Use case/Actor Description Functional Requirements**

Use Case Diagram

Use Case Description

Other Functional Requirements Other constraints

- User Interfaces
- Software (Tech) Stack Used
- Business rules (if any)

**Non Functional Requirement**

**Module dependencies with other fusion modules**

UI level

DB level Dependencies Module level dependencies

**Introduction![ref1]**

In this section, we present a comprehensive overview of the contents of this Software Requirements Specification (SRS) document. It encompasses the scope, providing a detailed description of what is covered, and an overview that outlines the key elements included. The purpose of this document is outlined, emphasizing its role in specifying the requirements for the software under consideration.

Additionally, we furnish a list of abbreviations and definitions to ensure clarity and understanding throughout the document. This section serves as a guide for readers, offering a roadmap to navigate the subsequent details and specifications outlined in the SRS document.

**Purpose**

This document serves to provide a detailed description of the requirements for the "HR-1" module within the "Fusion" software. Its main purpose is to outline the system's objectives, constraints, and specifications, serving as a proposal for customer approval and a reference guide for the development team as they embark on creating the initial version of the system. By offering clear insights, it aims to establish a shared understanding among stakeholders regarding the envisioned functionalities of the "HR-1" module in the broader context of the "Fusion" software.

**Product Scope**

The HR-1 module consists of many activities. This software product will have a limited scope as some of the activities are taken care of by other software. This software will take care of the following activities:

- CPDA (Cumulative Professional Development Allowance)
- LTC (Leave Travel Concession)
- Appraisal

**Definitions, Acronyms, and Abbreviations**

Table 1 - Definitions



|**Term**|**Definition**|
| - | - |



|User|Someone who interacts with the application.|
| - | - |
|LTC|Leave Travel Concession|
|CPDA|Cumulative Professional Development Allowance|
|Appraisal|A formal assessment of the performance of an employee over a particular period.|
|Faculty|The teaching or research staff of university departments|
|Staff|All the people employed by a particular organization.|
|Director|A person who is in charge of an organization.|
|Dealing Asstt.|Deals with the receipts.|
|HOD|Head of Department|
|AR|Assistant Registrar|
|DR|Deputy Registrar|
|Stakeholder|Any person who has interaction with the system who is not a developer.|
|Registrar|An official is responsible for keeping a register or official records.|
|SRS|Software Requirements Specification|
|Admin|Assigns reviewers to applications.|

**References and Acknowledgments**

1. IEEE Software Engineering Standards Committee, “IEEE Std 830-1998, IEEE Recommended Practice for Software Requirements Specifications”, October 20, 1998.
1. “Fusion” - Open Source Software, https://github.com/FusionIIIT/Fusion

**User/Actor Description![ref1]**

Three types of users interact with the system: Users of the module, Approval Authorities, and Administrators. Each of these three types of users has a different use of the system so each of them has its own requirements.

**Faculty/Staff :**

Faculty/Staff members interact with the system to initiate various requests such as Appraisal, CPDA (Continuing Professional Development Activity), and LTC (Leave Travel Concession).

**Role**: They are applicants in different submission processes, seeking Appraisal assessment, professional development activities, or leave travel concessions.

**General Functionalities:**

- Faculty/Staff must log in to access respective functionalities.
- Click on the relevant option (Appraisal,CPDA,or LTC) to access the request form.
- Fill in details on the request form and submit the form.
- Redirected to the requests page with a pending status for the respective request.

**HR Admin :**

The HR Admin is a system user with elevated privileges responsible for assigning applications to reviewers.

**Role**: The Admin manages the application review process, assigning reviewers to assess applications.

**General Functionalities:**

- Log in to access administrative functions.
- Assign reviewers to applications by filling out a form.
- Open and manage a list of application requests.
- Faculty/Staff can view submission status and remarks on their profiles.
- Manages and updates Employee records.

**Director/Registrar :**

The Director/Registrar is a pivotal role in the system responsible for approving or rejecting LTC (Leave Travel Concession) and CPDA (Continuing Professional Development Activity) requests.

**Role**: They hold the authority to review and make decisions on LTC and CPDA requests, ensuring compliance and appropriateness.

**General Functionalities**:

- The Director/Registrar must log in to access their respective functionalities.
- Click on the relevant option (LTC or CPDA) to view the list of requests.
- Open a specific request and click on the APPROVE or REJECT button accordingly.
- Faculty/Staff can see the approved status on their profile after approval or the not approved status with remarks if rejected.

**Note** : Director manages requests from faculty and Registrar manages requests from Staff.

**HOD :**

- View the list of CPDA, LTC or Appraisal requests.
- Approves(forwards) or rejects the requests.
- Be redirected to the relevant request page.
- Faculty/Staff can see the submitted status and remarks on their profile after appraisal approval.
- For CPDA requests, forward the approved application to the Estt. Section.

**Accountant :**

- The Accountant manages audits, updates and reconciles financial transactions, ensuring accuracy and compliance.
- Conduct financial audits and implement corrective actions.
- Record, reconcile, and update financial transactions related to LTC and CPDA.

**Functional Requirements![ref1]**

**Use Case Diagram :**

![](Aspose.Words.9d1f405d-75f7-4065-b965-602c621147db.003.jpeg)

**Use Case Description :**

**Use Case #1**



|Use Case ID|UC#1|
| - | - |
|Use Case Name|LTC form submission|
|Description|This use case describes the interaction between Faculty/Staff with the system to apply for LTC.|
|Actor|Faculty/Staff|
|Precondition|The Faculty/Staff must be logged in to the system.|
|Main Flow|<p>1. Faculty/Staff clicks on the LTC option on the panel on the right side.</p><p>2. LTC request form opens where Faculty/Staff fills the details.</p><p>3. Faculty/Staff clicks on the submit button.</p>|
|Postcondition|Faculty/Staff is redirected to the requests page having pending status on LTC request.|
|Alternate Flow||
|Postcondition||
|Sub Flow||
|Postcondition||
**Use Case #2**



|Use Case ID|UC#2|
| - | - |
|Use Case Name|LTC approval|
|Description|This use case describes the interaction between the Registrar/Director with the system to approve or reject an LTC request.|
|Actor|Registrar/Director|
|Precondition|The Registrar/Director must be logged in the system.|
|Main Flow|<p>1. The Registrar/Director clicks on the LTC option on the panel on the right side.</p><p>2. The Registrar/Director clicks on the LTC requests tab on the left side panel.</p><p>3. A list of requests opens up and the registrar/director opens a request.</p><p>4. The Registrar/Director clicks on the APPROVE button.</p>|
|Postcondition|<p>The Registrar/Director is redirected to the LTC request page.</p><p>Faculty/Staff can see the approved status on his profile.</p>|
|Alternate Flow|The Registrar/Director clicks on the REJECT button.|
|Postcondition|<p>The Registrar/Director is redirected to the LTC request page.</p><p>Faculty/Staff can see not approved status with remarks on his profile.</p>|
|Sub Flow||
|Postcondition||
**Use Case #3**



|Use Case ID|UC#3|
| - | - |
|Use Case Name|CPDA form submission|
|Description|This use case describes the interaction between Faculty/Staff with the system to apply for CPDA.|
|Actor|Faculty/Staff|
|Precondition|The Faculty/Staff must be logged in to the system.|
|Main Flow|<p>1. Faculty/Staff clicks on the CPDA option on the panel on the right side.</p><p>2. CPDA request form opens where Faculty/Staff fills the details.</p><p>3. Faculty/Staff clicks on the submit button.</p>|
|Postcondition|Faculty/Staff is redirected to the requests page having pending status on CPDA request.|
|Alternate Flow||
|Postcondition||
|Sub Flow||
|Postcondition||
**Use Case #4**



|Use Case ID|UC#4|
| - | - |
|Use Case Name|HOD\_Recommendation|
|Description|This use case describes the interaction between the HOD with the system to forward a CPDA request,|
|Actor|HOD|
|Precondition|The HOD must be logged in the system.|
|Main Flow|<p>1. The HOD clicks on the CPDA option on the panel on the right side.</p><p>2. The HOD clicks on the CPDA requests tab on the left side panel.</p><p>3. A list of requests opens up and HOD opens a request.</p><p>4. The HOD clicks on the APPROVE button.</p>|
|Postcondition|<p>The HOD is redirected to the CPDA request page.</p><p>The application is forwarded to Estt. Section.</p>|
|Alternate Flow|The HOD clicks on the REJECT button.|
|Postcondition|<p>The HOD is redirected to the CPDA request page.</p><p>Faculty/Staff can see not approved status with remarks on their profile.</p>|
|Sub Flow||
|Postcondition||

**Use Case #5**



|Use Case ID|UC#5|
| - | - |
|Use Case Name|Estt. Section|
|Description|This use case describes the interaction between the AR/DR and Dealing Asstt. with the system to forward a CPDA request,|
|Actor|AR/DR, Dealing Asstt.|
|Precondition|The AR/DR, Dealing Asstt. must be logged in the system.|
|Main Flow|<p>1. The AR/DR, Dealing Asstt. clicks on the CPDA option on the panel on the right side.</p><p>2. The AR/DR, Dealing Asstt. clicks on the CPDA requests tab on the left side panel.</p><p>3. A list of requests open up and AR/DR, Dealing Asstt. opens a request.</p><p>4. The AR/DR, Dealing Asstt. clicks on the APPROVE button.</p>|
|Postcondition|<p>The AR/DR, Dealing Asstt. is redirected to the CPDA request page.</p><p>The application is forwarded to Internal Audit.</p>|
|Alternate Flow|The AR/DR, Dealing Asstt. clicks on the REJECT button.|
|Postcondition|<p>The AR/DR, Dealing Asstt. is redirected to the CPDA request page.</p><p>Faculty/Staff can see not approved status with remarks on their profile.</p>|
|Sub Flow||
|Postcondition||

**Use Case #8****
|Use Case ID|UC#6|
| - | - |
|Use Case Name|Internal Audit|
|Description|This use case describes the interaction between the AR/DR and Dealing Asstt. with the system to forward a CPDA request|
|Actor|AR/DR, Dealing Asstt.|
|Precondition|The AR/DR, Dealing Asstt. must be logged in the system.|
|Main Flow|<p>1. The AR/DR, Dealing Asstt. clicks on the CPDA option on the panel on the right side.</p><p>2. The AR/DR, Dealing Asstt. clicks on the CPDA requests tab on the left side panel.</p><p>3. A list of requests opens up and AR/DR, Dealing Asstt. opens a request.</p><p>4. The AR/DR, Dealing Asstt. clicks on the APPROVE button.</p>|
|Postcondition|<p>The AR/DR, Dealing Asstt. is redirected to the CPDA request page.</p><p>The application is forwarded to the Director.</p>|
|Alternate Flow|The AR/DR, Dealing Asstt. clicks on the REJECT button.|
|Postcondition|<p>The AR/DR, Dealing Asstt. is redirected to the CPDA request page.</p><p>Faculty/Staff can see not approved status with remarks on their profile.</p>|
|Sub Flow||
|Postcondition||


|Use Case ID|UC#7|
| - | - |
|Use Case Name|CPDA form approval|
|Description|This use case describes the interaction between the Director with the system to approve a CPDA request|
|Actor|Director|
|Precondition|The Director must be logged in to the system.|
|Main Flow|<p>1. The Director clicks on the CPDA option on the panel on the right side.</p><p>2. The Director clicks on the CPDA requests tab on the left side panel.</p><p>3. A list of requests opens up and the Director opens a request.</p><p>4. The Director clicks on the APPROVE button.</p>|
|Postcondition|<p>The Director is redirected to the CPDA request page.</p><p>Faculty/Staff can see the approved status on their profile.</p>|
|Alternate Flow|<p>5\. The AR/DR clicks on the REJECT</p><p>button.</p>|
|Postcondition|<p>The AR/DR is redirected to the CPDA request page.</p><p>Faculty/Staff can see not approved status with remarks on their profile.</p>|
|Sub Flow||
|Postcondition||


|Use Case ID|UC#8|
| - | - |
|Use Case Name|Appraisal|
|Description|This use case describes the interaction between Faculty/Staff with the system to apply for Appraisal.|
|Actor|Faculty/Staff|
|Precondition|The faculty/staff must be logged in to the system.|
|Main Flow|<p>1. Faculty/Staff clicks on the Appraisal option on the panel on the right side.</p><p>2. The appraisal request form opens where Faculty/Staff fills in the details.</p><p>3. Faculty/Staff clicks on the submit button.</p>|
|Postcondition|Faculty/Staff is redirected to the requests page having pending status on Appraisal request.|
|Alternate Flow||
|Postcondition||
|Sub Flow||
|Postcondition||


**Use Case #9**



|Use Case ID|UC#9|
| - | - |
|Use Case Name|Review and Remarks|
|Description|This use case describes the interaction between the Director, HOD with the system to review and give remarks on an appraisal request|
|Actor|Director, HOD|
|Precondition|The Director, HOD must be logged in the system.|
|Main Flow|<p>1. The HOD, Director clicks on the Appraisal option on the panel on the right side.</p><p>2. The HOD, Director clicks on the Appraisal requests tab on the left side panel.</p><p>3. A list of requests opens up and the HOD, Director opens a request.</p><p>4. The HOD, Director clicks on the APPROVE button.</p>|
|Postcondition|<p>The Director, HOD is redirected to the Appraisal request page.</p><p>Faculty/Staff can see the submitted status on their profile along with the remarks provided.</p>|
|Alternate Flow||
|Postcondition||
|Sub Flow||
|Postcondition||

**Use Case #10****



|Use Case ID|UC#10|
| - | - |
|Use Case Name|Assign Reviewer|
|Description|This use case describes the interaction of the Admin with the system to assign applications to authorities to review and give remarks on an application.|
|Actor|Admin|
|Precondition|The Admin must be logged in the system.|
|Main Flow|<p>1. The Admin clicks on the CPDA/LTC/Appraisal option on the panel on the right side.</p><p>2. A list of requests opens up and the admin opens a request.</p><p>3. The Admin can assign the role of reviewing the application to other users by filling up a form.</p><p>4. The Admin clicks on the ASSIGN button.</p>|
|Postcondition|The Admin is redirected to the requests page. Faculty/Staff can see the submitted status on their profile along with the remarks provided.|
|Alternate Flow||
|Postcondition||
|Sub Flow||
|Postcondition||


**Other Functional Requirements:**

1. **Notification:**

Automate HR event alerts for employees, enhancing communication and engagement.

2. **Superuser/Admin Access:**

Grant elevated access to HR personnel for efficient system management.

3. **Form Editing:**

Enable employees to digitally edit HR forms, streamlining updates for data accuracy.

4. **Form Downloading:**

Enable employees to download the forms approved by the competent authority.

**Other Constraints: User Interfaces:**

The user interface should comply with the color scheming and dashboard design of the FUSIONIIT. Users should be able to navigate from one functionality to another. Inter module navigation should be smooth. All the functionalities should be easy to use and no specific training should be required for the usage of the module.

**Software (Tech) Stack Used: Frontend:**

**HTML**: The application's user interface is developed using HTML for structuring Web content

**CSS**: Styling in our application

**Backend:**

**Django**: Python web framework employed for building the application's back-end logic, facilitating efficient development and integration.

**Database:**

**PostgreSQL**: The relational database management system (RDBMS) used for storing and managing application data with a focus on scalability and performance.

**Version Control:** Git **Deployment:** Docker

**Business rules:**

1. Users must authenticate using a valid username and password to access the

system.

2. Different user roles (e.g., admin, faculty, student) have distinct access permissions,

and access is restricted based on these roles.

3. The system must comply with data privacy regulations, ensuring that sensitive user information is securely stored and accessed only by authorized personnel.

   4. Uploaded files must follow a specific naming convention for consistency and easier

management.

**Non-Functional Requirements** :

**Performance**: The system should be scalable for concurrent users and for huge data volumes of different actors.

**Reliability:** The system should have availability and Fault-tolerant error handling.

**Security**: Data encryption for sensitive information and role-based access control should be there in the product to ensure security.

**Usability:** The product will have a consistent and intuitive user interface. **Scalability:** Database scalability for courses and users. **Maintainability:** Modular architecture for easy updates.

**Module dependencies with other fusion modules : UI Level:**

The HR module can be accessed from the dashboard (the very first page after login) by the faculty, staff, and competent authorities or from the sidebar.

**DB Level Dependencies: Module Level Dependencies:**

GAD4, OS3 and GAD5 modules are having interactions with our module. Especially on GAD4 (File tracking module) for forwarding the requests.

**Appendix A – LTC Form![ref2]**

**PDPM**

**Indian Institute of Information Technology, Design & Manufacturing Jabalpur![](Aspose.Words.9d1f405d-75f7-4065-b965-602c621147db.005.png)**

**(An Institute Established by MHRD, Govt. of India)**

**Dumna Airport Road, PO: Khamaria, Jabalpur 482 005 India**

**APPLICATION FOR GRANT OF L.T.C (TO BE SUBMITTED IN DUPLICATE)**

Block year: P.F. No………………………… Basic Pay

Rs………

…………

…

1. Name\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
1. Designation\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
1. Department/Section\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
1. (a) Whether leave is required for availing L.T.C.? Yes\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_ No:\_\_\_\_\_\_\_\_\_\_\_\_ (b) (i) If so, duration of leave applied for From\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_ To:\_\_\_\_\_\_\_\_\_\_\_\_\_ (ii) Date of departure of family, if not availing himself \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_ (c) Nature of leave\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

(d) Purpose\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

5. Whether L.T.C. is desired for going to home town or elsewhere? Home

Town/Elsewhere (The place of the visit be also mentioned) Place

6. Address during leave\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_ \_\_\_ \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_ \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
6. Mode: Rail/Road \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

   8\.

1) Details of family members for whom L.T.C. for this block has already been availed: a. \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
   2. \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
   2. \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
1) Details of family members who will avail L.T.C.
1) Self
1) Wife
1) Children

   |S. No.|Full Name|Age|
   | - | - | - |
   ||||
   ||||
   ||||
   ||||
   ||||
   ||||
4) Dependent parents, minor brothers, and sisters residing with the applicant:

|S. No.|Full Name|Age|Why fully dependent?|
| - | - | - | - |
|||||
|||||
|||||


|||||
| :- | :- | :- | :- |
|||||
|||||
9 Amount of advance required, if any:

(i) Certified that family members for whom the L.T.C. is claimed are residing with me and are wholly dependent upon me. \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_ \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_ (ii) Certified that the previous L.T.C. advance drawn by me on ……………………….. has been adjusted in the month of ………………………...............................................................................

10. Date: \_\_\_/\_\_\_/\_\_\_\_\_
10. Phone Number for contact \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_ Signature
12. Specific recommendation of the Head of Department/Section

Approved/ Not Approved

Director/ Registrar

**Appendix B – CPDA Form![ref2]**

![](Aspose.Words.9d1f405d-75f7-4065-b965-602c621147db.006.jpeg)

**Appendix C – Appraisal Form![ref2]**

![](Aspose.Words.9d1f405d-75f7-4065-b965-602c621147db.007.jpeg)

![](Aspose.Words.9d1f405d-75f7-4065-b965-602c621147db.008.jpeg)

![](Aspose.Words.9d1f405d-75f7-4065-b965-602c621147db.009.png)

![](Aspose.Words.9d1f405d-75f7-4065-b965-602c621147db.010.png)

![](Aspose.Words.9d1f405d-75f7-4065-b965-602c621147db.011.png)

[ref1]: Aspose.Words.9d1f405d-75f7-4065-b965-602c621147db.002.png
[ref2]: Aspose.Words.9d1f405d-75f7-4065-b965-602c621147db.004.png
