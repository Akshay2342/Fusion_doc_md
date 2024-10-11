**Software Requirements Specification![](Aspose.Words.f51d0a49-c17a-48e6-a784-acad866b268e.001.png)**

**for**

**GAD-1**

**Prepared by**



|Dhruv Ghevariya|21BCS077|
| - | - |
|Omkar Wadekar|21BCS151|
|Naman Bhagat|21BCS140|
|Kishan Patel|21BCS117|
|Avdhesh Kumar|21BCS045|
|Priyansh Prajapati|21BCS166|

**1.Introduction**

1. Introduction about the Fusion

FusionIIIT stands as a testament to the seamless integration and automation of diverse functions within PDPM Indian Institute of Information Technology, Design and Manufacturing, Jabalpur. Crafted with precision using Python 3.8 and powered by the Django Web framework, this initiative is a student-driven endeavour designed to elevate the institute's operational landscape. Encompassing everything from efficient administration management to academic prowess and miscellaneous departmental tasks, FusionIIIT is a holistic solution that harmonizes the intricacies of campus life. Imagine it as a digital wizard that takes care of everything, from organizing the administrative stuff to making academics smoother. It is not just limited to the usual tasks; FusionIIIT jumps into various departments and sections, making sure every corner of campus life runs smoothly.

In the admin side, it handles the complicated paperwork and processes. For academics, it brings a digital touch, making learning and managing courses easier. But it does not stop there; FusionIIIT is like a friendly companion for all the different parts of the campus, making sure everything works well.

In simpler terms, FusionIIIT is not just a tool – it is a helpful friend, making life at PDPM IIITDM Jabalpur more organized and enjoyable for everyone.

2. Purpose of the module

GAD-1 Module is software designed to manage different administrative procedures related to the faculties of PDPM IIITDM Jabalpur.

The software is designed to provide automated features to the faculties and Administration Staff, to handle different faculties’ activities.

The different activities that come under this module are CPDA, LTC, and Appraisal.

3. Scope of the module

The HR-1 module consists of many activities. This software product will have a limited scope as some of the activities are taken care of by other software. This software will take care of the following activities:

- CPDA (Cumulative Professional Development Allowance)
- LTC (Leave Travel Concession)
- Appraisal



|**Term**|**Definition**|
| - | - |
|User|Someone who interacts with the application.|
|LTC|Leave Travel Concession|
|CPDA|Cumulative Professional Development Allowance|
|Appraisal|A formal assessment of the performance of an employee over a particular period.|
|Faculty|The teaching or research staff of university departments|
|Staff|All the people employed by a particular organization.|
|Director|A person who oversees an organization.|
|Dealing Asstt.|Deals with the receipts.|
|HOD|Head of Department|
|AR|Assistant Registrar|
|DR|Deputy Registrar|
|Stakeholder|Any person who interacts with the system who is not a developer.|
|Registrar|An official is responsible for keeping a register or official records.|
|SRS|Software Requirements Specification|
|Admin|Assigns reviewers to applications.|



- Faculty/Staff can apply for LTC, CPDA, and Appraisal through the web interface.
- The superiors can view the applications, approve and give reviews/remarks on them.
- Faculty/Staff can see the status of the application on their profile.

**2.User/Actor Description(characteristics)**

Three types of users interact with the system: Users of the module, approval Authorities, and administrators. Each of these three types of users has a different use of the system so each of them has its own requirements.

1. Users

The users which include the Faculty and Staff Members can only use the web application to submit their application. This means that the user has to be able to select the form, fill in the details, and then submit it.

2. Authorities

The authorities will use the web portal to verify the details of the applicant (user) and then decide whether to approve or reject that application.

3. Administrator

The administrators are managing the overall system so that there is no incorrect information within it. The administrator can manage the information for each application as well as the details of users and the approval authorities.

**3.Functional Requirements**

1. Use case Diagram

![](Aspose.Words.f51d0a49-c17a-48e6-a784-acad866b268e.002.jpeg)

2. **Use case description**
1. **Use Case #1**



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
2. **Use Case #2**



|Use Case ID|UC#2|
| - | - |
|Use Case Name|LTC approval|
|Description|This use case describes the interaction between the Registrar/Director with the system to approve or reject an LTC request.|
|Actor|Registrar/Director|



|Precondition|The Registrar/Director must be logged in the system.|
| - | :- |
|Main Flow|<p>1. The Registrar/Director clicks on the LTC option on the panel on the right side.</p><p>2. The Registrar/Director clicks on the LTC requests tab on the left side panel.</p><p>3. A list of requests opens up and the registrar/director opens a request.</p><p>4. The Registrar/Director clicks on the APPROVE button.</p>|
|Postcondition|<p>The Registrar/Director is redirected to the LTC request page.</p><p>Faculty/Staff can see the approved status on his profile.</p>|
|Alternate Flow|The Registrar/Director clicks on the REJECT button.|
|Postcondition|<p>The Registrar/Director is redirected to the LTC request page.</p><p>Faculty/Staff can see not approved status with remarks on his profile.</p>|
|Sub Flow||
|Postcondition||
3. **Use Case #3**



|Use Case ID|UC#3|
| - | - |
|Use Case Name|CPDA form submission|
|Description|This use case describes the interaction between Faculty/Staff with the system to apply for CPDA.|
|Actor|Faculty/Staff|
|Precondition|The Faculty/Staff must be logged in to the system.|



|Main Flow|<p>1. Faculty/Staff clicks on the CPDA option on the panel on the right side.</p><p>2. CPDA request form opens where Faculty/Staff fills the details.</p><p>3. Faculty/Staff clicks on the submit button.</p>|
| - | :- |
|Postcondition|Faculty/Staff is redirected to the requests page having pending status on CPDA request.|
|Alternate Flow||
|Postcondition||
|Sub Flow||
|Postcondition||
4. **Use Case #4**



|Use Case ID|UC#4|
| - | - |
|Use Case Name|CPDA HOD\_Recommendation|
|Description|This use case describes the interaction between the HOD with the system to forward a CPDA request,|
|Actor|HOD|
|Precondition|The HOD must be logged in the system.|
|Main Flow|<p>1. The HOD clicks on the CPDA option on the panel on the right side.</p><p>2. The HOD clicks on the CPDA requests tab on the left side panel.</p><p>3. A list of requests opens up and HOD opens a request.</p><p>4. The HOD clicks on the APPROVE button.</p>|
|Postcondition|<p>The HOD is redirected to the CPDA request page.</p><p>The application is forwarded to Estt. Section.</p>|



|Alternate Flow|The HOD clicks on the REJECT button.|
| - | - |
|Postcondition|<p>The HOD is redirected to the CPDA request page.</p><p>Faculty/Staff can see not approved status with remarks on their profile.</p>|
|Sub Flow||
|Postcondition||
5. **Use Case #5**



|Use Case ID|UC#5|
| - | - |
|Use Case Name|CPDA Estt. Section|
|Description|This use case describes the interaction between the AR/DR and Dealing Asstt. with the system to forward a CPDA request,|
|Actor|AR/DR, Dealing Asstt.|
|Precondition|The AR/DR, Dealing Asstt. must be logged in the system.|
|Main Flow|<p>1. The AR/DR, Dealing Asstt. clicks on the CPDA option on the panel on the right side.</p><p>2. The AR/DR, Dealing Asstt. clicks on the CPDA requests tab on the left side panel.</p><p>3. A list of requests open up and AR/DR, Dealing Asstt. opens a request.</p><p>4. The AR/DR, Dealing Asstt. clicks on the APPROVE button.</p>|
|Postcondition|<p>The AR/DR, Dealing Asstt. is redirected to the CPDA request page.</p><p>The application is forwarded to Internal Audit.</p>|
|Alternate Flow|The AR/DR, Dealing Asstt. clicks on the REJECT button.|
|Postcondition|The AR/DR, Dealing Asstt. is redirected to the CPDA request page.|



||Faculty/Staff can see not approved status with remarks on their profile.|
| :- | :- |
|Sub Flow||
|Postcondition||
6. **Use Case #6**



|Use Case ID|UC#6|
| - | - |
|Use Case Name|CPDA Internal Audit|
|Description|This use case describes the interaction between the AR/DR and Dealing Asstt. with the system to forward a CPDA request|
|Actor|AR/DR, Dealing Asstt.|
|Precondition|The AR/DR, Dealing Asstt. must be logged in the system.|
|Main Flow|<p>1. The AR/DR, Dealing Asstt. clicks on the CPDA option on the panel on the right side.</p><p>2. The AR/DR, Dealing Asstt. clicks on the CPDA requests tab on the left side panel.</p><p>3. A list of requests opens up and AR/DR, Dealing Asstt. opens a request.</p><p>4. The AR/DR, Dealing Asstt. clicks on the APPROVE button.</p>|
|Postcondition|<p>The AR/DR, Dealing Asstt. is redirected to the CPDA request page.</p><p>The application is forwarded to the Director.</p>|
|Alternate Flow|The AR/DR, Dealing Asstt. clicks on the REJECT button.|
|Postcondition|<p>The AR/DR, Dealing Asstt. is redirected to the CPDA request page.</p><p>Faculty/Staff can see not approved status with remarks on their profile.</p>|



|Sub Flow||
| - | :- |
|Postcondition||
7. **Use Case #7**



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
8. **Use Case #8**



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
9. **Use Case #9**



|Use Case ID|UC#9|
| - | - |
|Use Case Name|Review and Remarks|
|Description|This use case describes the interaction between the Director, HOD with the system to review and give remarks on an appraisal|



||request|
| :- | - |
|Actor|Director, HOD|
|Precondition|The Director, HOD must be logged in the system.|
|Main Flow|<p>1. The HOD, Director clicks on the Appraisal option on the panel on the right side.</p><p>2. The HOD, Director clicks on the Appraisal requests tab on the left side panel.</p><p>3. A list of requests opens up and the HOD, Director opens a request.</p><p>4. The HOD, Director clicks on the APPROVE button.</p>|
|Postcondition|<p>The Director, HOD is redirected to the Appraisal request page.</p><p>Faculty/Staff can see the submitted status on their profile along with the remarks provided.</p>|
|Alternate Flow||
|Postcondition||
|Sub Flow||
|Postcondition||
10. **Use Case #10**



|Use Case ID|UC#10|
| - | - |
|Use Case Name|Assign Reviewer|
|Description|This use case describes the interaction of the Admin with the system to assign applications to authorities to review and give remarks on an application.|
|Actor|Admin|
|Precondition|The Admin must be logged in the system.|



|Main Flow|<p>1. The Admin clicks on the CPDA/LTC/Appraisal option on the panel on the right side.</p><p>2. A list of requests opens up and the admin opens a request.</p><p>3. The Admin can assign the role of reviewing the application to other users by filling up a form.</p><p>4. The Admin clicks on the ASSIGN button.</p>|
| - | :- |
|Postcondition|The Admin is redirected to the requests page. Faculty/Staff can see the submitted status on their profile along with the remarks provided.|
|Alternate Flow||
|Postcondition||
|Sub Flow||
|Postcondition||
11. **Use Case #11**



|Use Case ID|UC#11|
| - | - |
|Use Case Name|LTC Estt. Section|
|Description|This use case describes the interaction between the AR/DR and Dealing Asstt. with the system to forward a LTC request,|
|Actor|AR/DR, Dealing Asstt.|
|Precondition|The AR/DR, Dealing Asstt. must be logged in the system.|
|Main Flow|<p>5. The AR/DR, Dealing Asstt. clicks on the LTC option on the panel on the right side.</p><p>6. The AR/DR, Dealing Asstt. clicks on the LTC requests tab on the left side panel.</p><p>7. A list of requests open up and AR/DR, Dealing Asstt. opens a request.</p><p>8. The AR/DR, Dealing Asstt. clicks on the APPROVE button.</p>|
|Postcondition|The AR/DR, Dealing Asstt. is redirected to the LTC request page.|



||The application is forwarded to Internal Audit.|
| :- | :- |
|Alternate Flow|The AR/DR, Dealing Asstt. clicks on the REJECT button.|
|Postcondition|<p>The AR/DR, Dealing Asstt. is redirected to the LTC request page.</p><p>Faculty/Staff can see not approved status with remarks on their profile.</p>|
|Sub Flow||
|Postcondition||
12. **Use Case #12**



|Use Case ID|UC#13|
| - | - |
|Use Case Name|LTC Internal Audit|
|Description|This use case describes the interaction between the AR/DR and Dealing Asstt. with the system to forward a LTC request|
|Actor|AR/DR, Dealing Asstt.|
|Precondition|The AR/DR, Dealing Asstt. must be logged in the system.|
|Main Flow|<p>5. The AR/DR, Dealing Asstt. clicks on the LTC option on the panel on the right side.</p><p>6. The AR/DR, Dealing Asstt. clicks on the LTC requests tab on the left side panel.</p><p>7. A list of requests opens up and AR/DR, Dealing Asstt. opens a request.</p><p>8. The AR/DR, Dealing Asstt. clicks on the APPROVE button.</p>|
|Postcondition|<p>The AR/DR, Dealing Asstt. is redirected to the LTC request page.</p><p>The application is forwarded to the Director.</p>|
|Alternate Flow|The AR/DR, Dealing Asstt. clicks on the REJECT button.|



|Postcondition|<p>The AR/DR, Dealing Asstt. is redirected to the LTC request page.</p><p>Faculty/Staff can see not approved status with remarks on their profile.</p>|
| - | :- |
|Sub Flow||
|Postcondition||
13. **Use Case #13**



|Use Case ID|UC#14|
| - | - |
|Use Case Name|LTC HOD\_Recommendation|
|Description|This use case describes the interaction between the HOD with the system to forward a LTC request,|
|Actor|HOD|
|Precondition|The HOD must be logged in the system.|
|Main Flow|<p>5. The HOD clicks on the LTC option on the panel on the right side.</p><p>6. The HOD clicks on the LTC requests tab on the left side panel.</p><p>7. A list of requests opens up and HOD opens a request.</p><p>8. The HOD clicks on the APPROVE button.</p>|
|Postcondition|<p>The HOD is redirected to the LTC request page.</p><p>The application is forwarded to Estt. Section.</p>|
|Alternate Flow|The HOD clicks on the REJECT button.|
|Postcondition|<p>The HOD is redirected to the LTC request page.</p><p>Faculty/Staff can see not approved status with remarks on their profile.</p>|
|Sub Flow||
|Postcondition||
3. **Other Functional Requirements**
1. **Integration with External Systems:**

The system should integrate with other existing systems within the institution for seamless data exchange and consistency.

2. **Data Backup and Recovery:**

Regular automated data backups should be performed to ensure data integrity and facilitate recovery in case of system failures.

3. **Security Measures:**

Implement security measures, such as encryption, to safeguard sensitive information stored in the system.

Regular security audits and vulnerability assessments should be conducted.

4. **Other Constraints**
1. **User Interfaces**
- Login Page:

  The system should have a secure login page for Faculty/Staff, Registrar/Director, HOD, AR/DR, Dealing Asstt., Director, and Admin.

  Usernames and passwords must be securely stored and validated.

- Dashboard:

  Each user role should have a personalized dashboard displaying relevant information and options based on their role (e.g., LTC requests, CPDA requests, Appraisal requests).

- Navigation Panel:

  A clear and intuitive navigation panel should be available to easily access different modules such as LTC, CPDA, Appraisal, and Admin functions.

- Request Forms:

  Request forms for LTC, CPDA, and Appraisal should be user-friendly with clear instructions and validation checks for mandatory fields.

  Input fields should be labeled appropriately, and the form should provide feedback on successful submission.

- Status Display:

  Users should be able to view the status of their requests on their profile or a dedicated page.

  Status labels (e.g., pending, approved, not approved) should be easily understandable.

- Approval/Rejection Actions:

  Buttons for actions like "APPROVE" and "REJECT" should be clearly visible and accessible to the relevant roles.

  Confirmation messages should be displayed after approval or rejection, and users should be redirected appropriately.

- Remarks Section:

  For roles that can provide remarks (e.g., Director, HOD), there should be a text area for entering comments during the approval or rejection process.

- Requests List:

  Lists of requests should be well-organized and easily filterable by status, date, or other relevant criteria.

  Clicking on a request should open a detailed view of the request.

- Assignment Form:

  The Admin interface should include a form for assigning applications to specific users for review.

  This form should be straightforward, with options to select the application type and the user to whom it is assigned.

- Error Handling:

  The system should provide clear error messages and guidance in case of invalid inputs or system errors.

- Security Measures:

  Ensure that the system implements secure authentication, authorization, and data encryption to protect user information.

- Responsiveness:

  The user interface should be responsive and accessible on different devices, including desktops, tablets, and mobile phones.

- User Help/Documentation:

  Provide a help section or documentation to guide users through the system functionalities and processes.

- Logout Functionality:

  Include a secure logout option to ensure user sessions are properly terminated.

- Accessibility:

  Ensure the user interface complies with accessibility standards to accommodate users with disabilities.

2. **Software (Tech) Stack Used**
- Flutter Framework
- Dart Programming Language
- Android Studio IDE/VS code (As Preferred)
- Git Version Control
4. **Non-Functional Requirements**
1. Performance:
- The system should be responsive and provide timely feedback to users during application submission, approval, and other interactions.
- Response time for critical operations, such as viewing and approving applications, should be within acceptable limits (e.g., 2 seconds).
2. Scalability:
- The system should be scalable to accommodate an increasing number of users and applications over time.
- It should handle concurrent user activities without significant degradation in performance.
3. Availability:
- The system should have a high level of availability, aiming for at least 99.9% uptime.
- Scheduled maintenance windows, if any, should be communicated to users in advance.
4. Reliability:
- The system should be reliable, minimizing the occurrence of system failures, crashes, or unexpected downtime.
  1. It should have mechanisms in place for quick recovery in case of failures.
5. Security:
   1. Data transmission and storage should be encrypted to ensure the confidentiality and integrity of sensitive information.
   1. Access controls should be robust, and user authentication should be secure.
6. Usability:
- The user interface should be intuitive, user-friendly, and accessible to individuals with disabilities.
- User interactions should follow industry standards and best practices.
7. Compatibility:
- The system should be compatible with commonly used web browsers (e.g., Chrome, Firefox, Safari) and devices (desktops, tablets, mobile phones).
- Accessibility standards (e.g., WCAG) should be followed to ensure compatibility with assistive technologies.
8. Compliance:
- The system should comply with relevant laws, regulations, and institutional policies.
- It should adhere to data protection and privacy standards applicable to the institution.
9. Auditability:
- The system should maintain logs and audit trails for all user actions and system events.
- Logs should be secure, tamper-evident, and accessible to authorized administrators.
10. Interoperability:
- The system should be interoperable with other systems and platforms used within the institution.
- Standard data exchange formats (e.g., JSON, XML) should be supported for integration.
11. Documentation:
- Comprehensive documentation should be provided for users, administrators, and developers.
- Documentation should include user guides, system architecture, and API documentation.
5. **Module dependencies with other fusion modules**
1. **UI Level**

The GAD-1 module will be seamlessly integrated into the Fusion interface, ensuring a cohesive user experience. Faculty/staff, approval authorities, and administrators will access their respective functionalities through a unified dashboard. The UI will be designed to allow users to navigate easily between LTC, CPDA, Appraisal, and Admin functions, providing a user-friendly and efficient interaction.

2. **DB Level Dependencies**

At the database level, the GAD-1 module shares relevant data with other Fusion modules. Specifically, data related to user profiles, application statuses, and approval/rejection remarks will be stored and accessed across modules. Careful consideration will be given to ownership and user roles associated with shared data to maintain data integrity and security.

**5.3. Module Level Dependencies File Tracking Module:**

The HR module's entire form and request forwarding logic will rely on the API provided by the File Tracking System module in FusionIIIT. This API integration ensures seamless coordination, enabling effective tracking of various form and request statuses.

**Notification Module:**

To maintain a synchronized and timely response to requests, the Notification Module will play a vital role. The HR module will utilize the Notification Module's API to inform concerned actors about the submission and status updates of requests made by faculty/staff. This integration ensures that all relevant parties stay informed and can respond promptly.

**Dashboards Module:**

Access and interaction with CPDA, LTC, and appraisal forms/requests will be centralized through the Dashboards Module. All actors, including faculty/staff and administrators, will utilize this module to navigate and manage requests efficiently. This centralized approach enhances user experience and streamlines the overall workflow within the HR module.

**Appendix A – LTC Form![ref1]**

**PDPM**

**Indian Institute of Information Technology, Design & Manufacturing Jabalpur![](Aspose.Words.f51d0a49-c17a-48e6-a784-acad866b268e.004.png)**

**(An Institute Established by MHRD, Govt. of India)**

**Dumna Airport Road, PO: Khamaria, Jabalpur 482 005 India**

**APPLICATION FOR GRANT OF L.T.C (TO BE SUBMITTED IN DUPLICATE)**

Block year: P.F. No………………………… Basic Pay

Rs…… ……… ………

1. Name\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
1. Designation\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
1. Department/Section\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
1. (a) Whether leave is required for availing L.T.C.? Yes\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_ No:\_\_\_\_\_\_\_\_\_\_\_\_ (b) (i) If so, duration of leave applied for From\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_ To:\_\_\_\_\_\_\_\_\_\_\_\_\_ (ii) Date of departure of family, if not availing himself \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_ (c) Nature of leave\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

(d) Purpose\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

5. Whether L.T.C. is desired for going to home town or elsewhere? Home Town/Elsewhere (The place of the visit be also mentioned) Place
5. Address during leave\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_ \_ \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_ \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_ 7. Mode: Rail/Road \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_

   8\.

1) Details of family members for whom L.T.C. for this block has already been availed: a. \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
2. \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
2. \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
2) Details of family members who will avail L.T.C.
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


|S. No.|Full Name|Age|Why fully dependent?|
| - | - | - | - |
|||||
|||||
|||||
|||||
|||||
|||||
4) Dependent parents, minor brothers, and sisters residing with the applicant: 9 Amount of advance required, if any:

   (i) Certified that family members for whom the L.T.C. is claimed are residing with me and are wholly dependent upon me.![](Aspose.Words.f51d0a49-c17a-48e6-a784-acad866b268e.005.png)

   ii) Certified that the previous L.T.C. advance drawn by me on ……………………….. has been adjusted in the month of ………………………...............................................................................

10. Date: \_\_\_/\_\_\_/\_\_\_\_\_
10. Phone Number for contact \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_ Signature
12. Specific recommendation of the Head of Department/Section

Approved/ Not Approved

Director/ Registrar

**Appendix B – CPDA Form![ref1]**

![](Aspose.Words.f51d0a49-c17a-48e6-a784-acad866b268e.006.jpeg)

**Appendix C – Appraisal Form![](Aspose.Words.f51d0a49-c17a-48e6-a784-acad866b268e.007.png)**

![](Aspose.Words.f51d0a49-c17a-48e6-a784-acad866b268e.008.jpeg)

![](Aspose.Words.f51d0a49-c17a-48e6-a784-acad866b268e.009.jpeg)

![](Aspose.Words.f51d0a49-c17a-48e6-a784-acad866b268e.010.png)

![](Aspose.Words.f51d0a49-c17a-48e6-a784-acad866b268e.011.png)

![](Aspose.Words.f51d0a49-c17a-48e6-a784-acad866b268e.012.png)

[ref1]: Aspose.Words.f51d0a49-c17a-48e6-a784-acad866b268e.003.png
