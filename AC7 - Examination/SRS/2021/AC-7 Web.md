**Software Requirements Specification**

**AC-7 EXAMINATION (WEB)**

**Faculty Mentor: Dr.Munesh Sir**

**Team Details**

**Team Mentor** : B.Nishanth (21BCS059) C.Sai Ganesh (21BCS067)

Charishma (21BCS065)

Akshitha (21BCS110)

B.Harshan Nayak (21BCS058) B.Harsha Nandan (21BCS061)

**1. Introduction**

1. **Introduction about the Fusion**

FusionIIIT stands as a testament to the seamless integration and automation of diverse functions within PDPM Indian Institute of Information Technology, Design and Manufacturing, Jabalpur. Crafted with precision using Python 3.8 and powered by the Django Web framework, this initiative is a student-driven endeavor designed to elevate the institute's operational landscape. Encompassing everything from efficient administration management to academic prowess and miscellaneous departmental tasks, FusionIIIT is a holistic solution that harmonizes the intricacies of campus life.

Imagine it as a digital wizard that takes care of everything, from organizing the administrative stuff to making academics smoother. It's not just limited to the usual tasks; FusionIIIT jumps into various departments and sections, making sure every corner of campus life runs smoothly.

In the admin side, it handles the complicated paperwork and processes. For academics, it brings a digital touch, making learning and managing courses easier. But it doesn't stop there; FusionIIIT is like a friendly companion for all the different parts of the campus, making sure everything works well.

In simpler terms, FusionIIIT is not just a tool – it's a helpful friend, making life at PDPM IIITDM Jabalpur more organized and enjoyable for everyone.

2. **Purpose of the module**

The Examination Module functions as an all-encompassing platform meticulously crafted to enhance the seamless and effective administration of the result declaration process within an educational institution. Serving as a pivotal element in the academic ecosystem, this module presents a user-friendly interface tailored for faculty members to effortlessly input grades and marks. Simultaneously, it furnishes administrators with robust tools for in-depth analysis of results, ensuring a just and streamlined outcome for students.

3. **Scope of the module**

The Examination Module has been meticulously crafted to function as a resilient platform, facilitating the efficient and streamlined declaration of academic results with a focus on two key stakeholders: faculty and administrators. Faculty members benefit from a user-friendly interface within the module, allowing them to seamlessly submit grades and marks. Conversely, administrators utilize the module's analytical tools to garner insights into overarching performance trends. Through in-depth result analyses that compare data across courses and semesters, the Examination Module assumes a pivotal role in ensuring a transparent, fair, and efficient process for result declaration within academic institutions.

**2.User/Actor Description(characteristics):**

1. **ACAD-ADMIN:**

This ACAD-ADMIN is responsible for overseeing all aspects of the examination system. Their role includes verifying and analyzing the grades submitted by faculty members. They play a crucial part in the strategic implementation, management, and optimization of the system to ensure its smooth operation. In essence, they are tasked with supervising the overall functionality of the examination process and making sure that the system operates effectively and efficiently.

**Role: Verifies and analyzes grades submitted by faculty Specific Functionalities:**

1\. Submits grades for different courses enrolled.

2\.Authenticate course grades from respective Faculty & Moderate-Grade If anywhere required

3\.generate results after compiling the grades submitted by faculty

4\.Make Important Announcements to the students and notify them regarding results and grade

5\.verify the student result if any student has discrepency

2. **FACULTY IN CHARGE:**

Responsible for Submitting grades to acad-admin of every Individual

**Role:** Based on calculated marks, Faculty generates grades for every student and sends it to acad-admin.

**Specific Functionalities:**

1. Enter and submit grades for students based on their performance in exams,Assignments,and Other assessments.
1. Verify and ensure the accuracy of the entered grades before submission.
3. **Functional Requirements**
1. **Use Case Diagram**

![](Aspose.Words.14eed2ce-1472-4e9f-ae2d-8b1ae4f22b30.001.jpeg)

2. **Use case Description**

This section describes each use case Description in the use case diagram in all details.

**1)**



|**UC ID**|UC#1|
| - | - |
|**Use case Name**|**Submit grade**|
|**Description**|The ”submit grade” use case allows the Acad Admin of the college to submit grade of specific examination of every student through the Fusion portal .|
|**Actor**|Acad Admin|
|**Precondition**|The Acad Admin is logged in into the system|



<table><tr><th colspan="1" rowspan="2" valign="top"><b>Main Flow</b></th><th colspan="1" valign="top">1</th><th colspan="1" valign="top">Academic Administrator selects the "Submit Grade" option.</th></tr>
<tr><td colspan="1" valign="top">2</td><td colspan="1" valign="top">System displays a list of available examinations. Acad admin selects the examination for which grades are to be submitted.</td></tr>
<tr><td colspan="1"></td><td colspan="1" valign="top">3</td><td colspan="1" valign="top">System displays a list of enrolled students for the selected examination. Acad admin enters the grades for each student.</td></tr>
<tr><td colspan="1"></td><td colspan="1" valign="top">4</td><td colspan="1" valign="top">System validates the entered grades.[A1]</td></tr>
<tr><td colspan="1"></td><td colspan="1" valign="top">5</td><td colspan="1" valign="top">System saves the submitted grades.[A2]</td></tr>
<tr><td colspan="1"></td><td colspan="1" valign="top">6</td><td colspan="1" valign="top">System displays a confirmation message for successful grade submission.</td></tr>
</table>



<table><tr><th colspan="1" valign="top"><b>Post conditions</b></th><th colspan="3" valign="top">Grades for the selected examination have been successfully submitted by the Academic Administrator.</th></tr>
<tr><td colspan="1" rowspan="2" valign="top"><b>Alternate Flow</b></td><td colspan="1" rowspan="2" valign="top">A1</td><td colspan="1" valign="top">1</td><td colspan="1" valign="top">System shows an error message for invalid grades.</td></tr>
<tr><td colspan="1" valign="top">2</td><td colspan="1" valign="top">Acad admin corrects the grades.</td></tr>
<tr><td colspan="1"></td><td colspan="1" valign="top">A2</td><td colspan="1" valign="top">1</td><td colspan="1" valign="top">System displays an error message for a submission failure</td></tr>
<tr><td colspan="1"></td><td colspan="1"></td><td colspan="1" valign="top">2</td><td colspan="1" valign="top">Academic Administrator retries the grade submission.</td></tr>
<tr><td colspan="1" valign="top"><b>Sub Flow</b></td><td colspan="3" valign="top">NIL</td></tr>
<tr><td colspan="1" rowspan="2" valign="top"><b>Global Alternate Flow</b></td><td colspan="1" valign="top">GA1</td><td colspan="2" valign="top">Acad admin cancels the grade submission. No grades are submitted. System displays the main menu</td></tr>
<tr><td colspan="1" valign="top">GA2</td><td colspan="2" valign="top">IAcademic Administrator retries the grade submission.</td></tr>
</table>

**2)**



|**UC ID**|UC#2|
| - | - |
|**Use case Name**|**Moderate Grade**|
|**Description**|The ”Moderate Grade” use case allows the Acad Admin of the college To Moderate Grade and check all results through the Fusion portal .so that the Grades of students can be moderated|
|**Actor**|Acad Admin|



<table><tr><th colspan="1" valign="top"><b>Precondition</b></th><th colspan="2" valign="top">The Acad Admin is logged in into the system</th></tr>
<tr><td colspan="1" rowspan="2" valign="top"><b>Main Flow</b></td><td colspan="1" valign="top">1</td><td colspan="1" valign="top">The Acad Admin navigates to the "Moderate Grade" section.</td></tr>
<tr><td colspan="1" valign="top">2</td><td colspan="1" valign="top">The system displays the list of Grades of the students for a subject after selecting the Respective semester and Branch .</td></tr>
<tr><td colspan="1"></td><td colspan="1" valign="top">3</td><td colspan="1" valign="top">Academic Administrator reviews the submitted grades and identifies any adjustments needed.</td></tr>
<tr><td colspan="1"></td><td colspan="1" valign="top">4</td><td colspan="1" valign="top">System validates the moderated grades.[A1]</td></tr>
<tr><td colspan="1"></td><td colspan="1" valign="top">5</td><td colspan="1" valign="top">The system displays button to publish Results.</td></tr>
</table>



<table><tr><th colspan="1" valign="top"><b>Post conditions</b></th><th colspan="3" valign="top">Grades for the selected examination have been successfully moderated by the Academic Administrator.</th></tr>
<tr><td colspan="1" rowspan="2" valign="top"><b>Alternate Flow</b></td><td colspan="1" rowspan="2" valign="top">A1</td><td colspan="1" valign="top">1</td><td colspan="1" valign="top">System displays an error message for invalid moderated grades.</td></tr>
<tr><td colspan="1" valign="top">2</td><td colspan="1" valign="top">Academic Administrator corrects the grades.</td></tr>
<tr><td colspan="1" valign="top"><b>Sub Flow</b></td><td colspan="3" valign="top">NIL</td></tr>
<tr><td colspan="1" rowspan="2" valign="top"><b>Global Alternate Flow</b></td><td colspan="1" valign="top">GA1</td><td colspan="2" valign="top">The Acad Admin can ‘cancel’ the procedure at any time by exercising such an option and will be directed to the dashboard.</td></tr>
<tr><td colspan="1" valign="top">GA2</td><td colspan="2" valign="top">If a technical error occurs during the execution of any action (e.g., database failure, server issues), the system displays an error message and logs the incident.</td></tr>
</table>

**3)**



|**UC ID**|UC#3|
| - | - |
|**Use case Name**|**Verify Result**|
|**Description**|The ”Verify Result” use case allows the Acad Admin of the college verifies the accuracy and correctness of the final results for a specific examination before making them official|
|**Actor**|Acad Admin|
|**Precondition**|Moderation of grades must be done before moving further.|



<table><tr><th colspan="1" rowspan="2" valign="top"><b>Main Flow</b></th><th colspan="1" valign="top">M1</th><th colspan="1" valign="top">The Acad Admin navigates to the "Verify" section.</th></tr>
<tr><td colspan="1" valign="top">M2</td><td colspan="1" valign="top">system displays the final results for the selected examination.</td></tr>
<tr><td colspan="1"></td><td colspan="1" valign="top">M3</td><td colspan="1" valign="top">Academic Administrator reviews individual student results and overall statistics</td></tr>
<tr><td colspan="1"></td><td colspan="1" valign="top">M4</td><td colspan="1" valign="top">The system displays the Verify button if all grades are checked.</td></tr>
<tr><td colspan="1"></td><td colspan="1" valign="top">M5</td><td colspan="1" valign="top">Academic Administrator enters the Moderated grades(if any) for specific examination.</td></tr>
<tr><td colspan="1"></td><td colspan="1" valign="top">M6</td><td colspan="1" valign="top">System validates the entered grades.</td></tr>
<tr><td colspan="1"></td><td colspan="1" valign="top">M7</td><td colspan="1" valign="top">System saves the submitted grades.</td></tr>
<tr><td colspan="1"></td><td colspan="1" valign="top">M8</td><td colspan="1" valign="top">Academic Administrator reviews that authorities have verified the result</td></tr>
<tr><td colspan="1"></td><td colspan="1" valign="top">M9</td><td colspan="1" valign="top">System saves the authenticated preliminary final results.[A1]</td></tr>
<tr><td colspan="1"></td><td colspan="1" valign="top">M10</td><td colspan="1" valign="top">System compiles any additional adjustments made during authentication and calculates the official final results.</td></tr>
<tr><td colspan="1"></td><td colspan="1" valign="top">M11</td><td colspan="1" valign="top">System displays a confirmation message for successful grade submission.</td></tr>
</table>



|**Post conditions**|Final results for the selected examination have been successfully verified by the authorities and generated by the Academic Administrator.||||
| :- | :- | :- | :- | :- |
|**Specific Alternate Flow**|A1|1|System displays an error message for invalid grades.|Academic Administrator corrects the grades.|



<table><tr><th colspan="1"></th><th colspan="1"></th><th colspan="1" valign="top">2</th><th colspan="1" valign="top">System displays an error message for a submission failure.</th><th colspan="1" valign="top"><p>Academic Administrator</p><p>retries the grade</p><p>submission.</p></th></tr>
<tr><td colspan="1" valign="top"><b>Sub Flow</b></td><td colspan="3" valign="top">NIL</td><td colspan="1"></td></tr>
<tr><td colspan="1" rowspan="2" valign="top"><b>Global Alternate Flow</b></td><td colspan="1"></td><td colspan="2"></td><td colspan="1"></td></tr>
<tr><td colspan="1"></td><td colspan="2"></td><td colspan="1"></td></tr>
<tr><td colspan="1"></td><td colspan="1" valign="top">GA</td><td colspan="1"></td><td colspan="1" valign="top">Academic Administrator cancels the grade submission.</td><td colspan="1" valign="top"><p>No grades are</p><p>submitted. System</p><p>displays the main</p><p>menu.</p></td></tr>
</table>

**4)**



<table><tr><th colspan="1" valign="top"><b>UC ID</b></th><th colspan="2" valign="top">UC#4</th></tr>
<tr><td colspan="1" valign="top"><b>Use case Name</b></td><td colspan="2" valign="top"><b>Generate Final Results</b></td></tr>
<tr><td colspan="1" valign="top"><b>Description</b></td><td colspan="2" valign="top">The Acad Admin generates the final results for a specific examination, compiling and presenting the grades of enrolled students.</td></tr>
<tr><td colspan="1" valign="top"><b>Actor</b></td><td colspan="2" valign="top">Acad Admin</td></tr>
<tr><td colspan="1" valign="top"><b>Precondition</b></td><td colspan="2" valign="top">The Academic Administrator is logged into the examination module, and grades for the selected examination have been submitted and moderated.</td></tr>
<tr><td colspan="1" rowspan="3" valign="top"><b>Main Flow</b></td><td colspan="1" valign="top">1</td><td colspan="1" valign="top">Academic Administrator selects the "Generate Final Result" option.</td></tr>
<tr><td colspan="1" valign="top">2</td><td colspan="1" valign="top">System displays a list of available examinations.</td></tr>
<tr><td colspan="1" valign="top">3</td><td colspan="1" valign="top">Academic Administrator selects the examination for which final results are to be generated.</td></tr>
</table>



<table><tr><th colspan="1" rowspan="6"></th><th colspan="1" valign="top">4</th><th colspan="1" valign="top">System compiles the moderated grades and calculates the final results.</th></tr>
<tr><td colspan="1" valign="top">5</td><td colspan="1" valign="top">System displays the final results, including any adjustments made during moderation.</td></tr>
<tr><td colspan="1" valign="top">6</td><td colspan="1" valign="top">Academic Administrator reviews the generated final results.</td></tr>
<tr><td colspan="1" valign="top">7</td><td colspan="1" valign="top">Academic Administrator confirms the final results for publishing [A1]</td></tr>
<tr><td colspan="1" valign="top">8</td><td colspan="1" valign="top">System saves and publishes the official final results.</td></tr>
<tr><td colspan="1" valign="top">9</td><td colspan="1" valign="top">System displays a confirmation message for successful final result generation.</td></tr>
</table>



|**Post conditions**|Official final results for the selected examination have been successfully generated and published by the Academic Administrator.|||
| - | :- | :- | :- |
|**Alternate Flow**|A1|1|System displays an error message for a result generation failure|
|**Sub Flow**|NIL|||
|**Global Alternate Flow**|GA1|Academic Administrator cancels the final result generation.||

**5)**



<table><tr><th colspan="1" valign="top"><b>UC ID</b></th><th colspan="2" valign="top">UC#5</th></tr>
<tr><td colspan="1" valign="top"><b>Use case Name</b></td><td colspan="2" valign="top"><b>Make Announcements</b></td></tr>
<tr><td colspan="1" valign="top"><b>Description</b></td><td colspan="2" valign="top">The Academic Administrator creates and posts announcements related to examinations, providing important information and updates for students and other stakeholders.</td></tr>
<tr><td colspan="1" valign="top"><b>Actor</b></td><td colspan="2" valign="top">Acad Admin</td></tr>
<tr><td colspan="1" valign="top"><b>Precondition</b></td><td colspan="2" valign="top">The Academic Administrator is logged into the examination module.</td></tr>
<tr><td colspan="1" rowspan="3" valign="top"><b>Main Flow</b></td><td colspan="1" valign="top">1</td><td colspan="1" valign="top">Academic Administrator selects the "Make Announcements" option.</td></tr>
<tr><td colspan="1" valign="top">2</td><td colspan="1" valign="top">System displays the announcement creation interface.</td></tr>
<tr><td colspan="1" valign="top">3</td><td colspan="1" valign="top">Academic Administrator enters the announcement content, including the title and details.</td></tr>
</table>



<table><tr><th colspan="1" rowspan="4"></th><th colspan="1" valign="top">4</th><th colspan="1" valign="top">Academic Administrator specifies the target audience (e.g., all students, specific courses,faculty).</th></tr>
<tr><td colspan="1" valign="top">5</td><td colspan="1" valign="top">Academic Administrator selects the option to post the announcement.</td></tr>
<tr><td colspan="1" valign="top">6</td><td colspan="1" valign="top">System saves and posts the announcement.</td></tr>
<tr><td colspan="1" valign="top">7</td><td colspan="1" valign="top">System notifies the relevant audience about the new announcement.[A1]</td></tr>
</table>



|**Post conditions**|The announcement has been successfully created, posted, and notified to the specified audience.|||
| - | :- | :- | :- |
|**Alternate Flow**|A1|1|System displays an error message for a posting failure.|
|**Sub Flow**|NIL|||
|**Global Alternate Flow**|GA1|Academic Administrator cancels the announcement creation.||

**6)**



|**UC ID**|**UC#6**||
| - | - | :- |
|**Use case Name**|**Time Table**||
|**Description**|<p>**The Acad-Admin creates the examination timetable and seating**</p><p>**arrangement for students in lecture halls based on the courses.**</p>||
|**Actor**|**Acad Admin**||
|**Preconditio n**|**Courses, Classroomsand a list of enrolled students for each course are available in the examination modeule.**||
|**Main Flow**|**1**|**Academic Administrator selects the "Create Timetable seating Arrangement" option.**|



<table><tr><th colspan="1" rowspan="6"></th><th colspan="1" valign="top"><b>2</b></th><th colspan="1" valign="top"><b>System displays list of available courses.</b></th></tr>
<tr><td colspan="1" valign="top"><b>3</b></td><td colspan="1" valign="top"><b>Academic Administrator selects a courses for which the examination timetable and seating arrangement are to be created.</b></td></tr>
<tr><td colspan="1" valign="top"><b>4</b></td><td colspan="1" valign="top"><b>System generates a draft timetable for the selcted course considering the available time slots and lecture halls[A1]</b></td></tr>
<tr><td colspan="1" valign="top"><b>5</b></td><td colspan="1" valign="top"><b>Academic Administrator reviews and adjusts the draft time table as needed , assigning time slots for each exam.</b></td></tr>
<tr><td colspan="1" valign="top"><b>6</b></td><td colspan="1" valign="top"><b>Acad-Admin selects a lecture hall for each exam in time table.</b></td></tr>
<tr><td colspan="1" valign="top"><b>7</b></td><td colspan="1" valign="top"><b>System generataes a seating arrangement for each exam based ont he enrolled students for the selected course.[A2]</b></td></tr>
<tr><td colspan="1"></td><td colspan="1" valign="top"><b>8</b></td><td colspan="1" valign="top"><b>Acad Admin reviews and adjusts the seating arrangemets as needed.</b></td></tr>
<tr><td colspan="1"></td><td colspan="1" valign="top"><b>9</b></td><td colspan="1" valign="top"><b>Acad-Admin finalizes the timetale and seating arrangemet.</b></td></tr>
</table>



||**10**|**System saves the finalizes the time table and seating arrangemet**|
| :- | - | - |



|**Post conditions**|**The examinationtime table and seating arrangement for the selected course have been successfully created and saved by the acad-admin.**|
| :- | :- |



|**Alternate Flow**|**A1**|**1**|**System detects a lack of available lecture halls for exams.**|
| - | - | - | :- |
|||**2**|**Academic Administrator adjusts the timetable or schedules exams in different time slots**|
||**A2**|**1**|**System detects a conflict in the seating arrangement (e.g., two students assigned to the same seat)**|
|||**2**|**Academic Administrator resolves the seating conflict.**|
|**Sub Flow**|**NIL**|||
|**Global Alternate Flow**|**GA1**|**Academic Administrator cancels the timetable creation. No timetable or seating arrangement is created. System displays the main menu.**||

**3.3. Other Functional Requirements**

1 This module will make use of the **Notification module** for sending notifications and alerts to various actors involved in the module suitably for raising issues aganist grades etc.

2 The system should be able to deal with error-less statistics while calculating grades.

**3.4 Other constraints**

1. **User Interfaces**

The user interface should comply with the colour scheming and dashboard design of the FUSIONIIT. Users should be able to navigate from one functionality to other. Inter module navigation should be smooth. All the functionalities should be easy to use and no specific training should be required for the usage of the module

2. **Tech Stack Used**

1\.Backend: Django(Python Based Web-Framework). 2.Frontend:(HTML,CSS,Javascript).

3. **Business rules**

**For ACAD-ADMIN**

- **Submission of Grades:**
  - Business Rule: ACAD-ADMIN are allowed to submit grades for different courses they oversee.
  - Enforcement: The system should provide a secure interface for examination administrators to input and submit grades for enrolled courses.
- **Grade Modification:**
  - Business Rule: ACAD-ADMIN have the authority to modify grades if necessary.
  - Enforcement: Modifications should be logged with timestamp and user details for audit purposes.
- **Result Generation:**
  - Business Rule: ACAD-ADMIIN can generate results after compiling all submitted grades.
  - Enforcement: The system should automatically compile grades and generate results upon administrator request.
- **Announcements and Notifications:**
  - Business Rule: ACAD-ADMIN can make important announcements and notify students about result and grades-related information.
  - Enforcement: Notification mechanisms should be in place to disseminate announcements promptly through official channels.
- **Result Verification:**
  - Business Rule: ACAD-ADMIN are responsible for verifying results if any student finds any discrepancy.
- Enforcement: An efficient system for result verification should be implemented, allowing administrators to address discrepancies promptly.

**For Faculty In Charge:**

- **Grade Submission:**
  - Business Rule: Faculty in charge is only responsible for entering and submitting grades for students based on their performance in exams, assignments, and other assessments.
  - Enforcement: The system should restrict faculty in charge from accessing or modifying other administrative functionalities.
- **Grade Verification:**
  - Business Rule: Faculty in charge must verify and ensure the accuracy of entered grades before submission.
  - Enforcement: The system should incorporate validation checks to ensure grades adhere to predefined criteria before submission.

**General Rules:**

- **Authentication and Authorization:**
  - Business Rule: Access to examination functionalities is restricted based on user roles.
  - Enforcement: User authentication and authorization mechanisms should be implemented to ensure role-based access control.
- **Data Security:**
  - Business Rule: All sensitive data, including grades and results, must be stored securely.
  - Enforcement: The system should use encryption and access controls to protect sensitive information from unauthorized access.
- **Audit Trail:**
  - Business Rule: All actions performed by examination administrators and faculty in charge should be logged for audit purposes.
  - Enforcement: The system should maintain detailed logs, including user actions, timestamps, and system responses.
- **User Notification and Feedback:**
  - Business Rule: Users should be promptly notified of system-related announcements, and mechanisms for user feedback should be available.
  - Enforcement: Notification systems and feedback forms should be incorporated into the user interface.
4. **Non- Functional Requirements**

Non-functional requirements encompass aspects of a system that don't dictate its operational functionality but rather assess its overall quality. These requirements cover criteria that evaluate the performance of the system rather than specific functionalities. In our project, the identified non-functional requirements include:

- **Usability**
- **Reliability**
- **Integrity**
- **Performance**
1. **Usability:**

Usability is a crucial quality attribute used to evaluate the ease of use of the system interface. It encompasses factors such as memorability, learnability, and user satisfaction. The software interface in our project possesses all these qualities, ensuring that it is user-friendly and accessible for individuals of varying expertise. Users can easily comprehend and navigate the interface, enhancing overall usability.

2. **Reliability:**

Reliability assesses the consistency of the system across various platforms. It gauges the system's ability to perform its required functions consistently and without degradation or failure when demanded. In essence, reliability ensures that the system remains dependable under different conditions.

3. **Integrity:**

Integrity involves conducting the right actions in a dependable manner. In the context of our system, data integrity is a fundamental component of security. Broadly, "Data Integrity" refers to the accuracy and consistency of data stored in a database or any other construct. It emphasizes the overall completeness, accuracy, and consistency of the data, ensuring that information remains reliable and unaltered.

5. **Module dependencies with other fusion modules**

▪ **5.1.UI Level:**

- The Examination module is a recent addition to Fusion IIIT, aimed at facilitating a more streamlined and efficient management of the examination processes within the institute
- In the Dashboard Section of FusionIIIT website , a new section specifically for examinations will be incorporated.
- For academic administrators, three options will be displayed:
- 3.1 **Verify Results:** This involves the verification of results for a specific course.
- 3.2 **Generate Results:** After thorough analysis and verification, the results will be generated and subsequently uploaded.
- 3.3 **Announce Results:** Finally, there is an option to announce results, ensuring that students are duly notified.
- Faculty members will have the option to upload results for a designated course.
2. **DB Level Dependencies:** The database with which we are interacting are:
   1) Student DataBase(for extracting student information).
   1) Course DataBase(for extracting courses with their respective faculty).
   1) Notifications DataBase(for storing the time to time notifications that are generated).

      3. **Module Level Dependencies:** The examination module depends upon the

**Course Registration** Module(for fetching the students in the respective course), **Department Module(**for fetching the course and their respective faculty),

**Notifications Module**(for making the announcement for the final result).
