**Software Requirements Specification**

**For**

**Department Module (AC6-Web)**

Faculty Mentor: Dr. Pritee Khanna Mentor: Prajjwal Kapoor(21bcs158)

Team Members:

Aryan Shrivastava(21bcs040) Rushikesh Shinde(21bcs190) Manoj Panjwani(21bec068) Sudarshan Patidar(21bcs208) Jesvia Susan Varghese(21bcsd01)

1. Introduction
1. **Introduction about the Fusion – A Brief Description**

Fusion IIIT serves as a testament to the seamless integration and automation of diverse functions within the precincts of PDPM Indian Institute of Information Technology, Design, and Manufacturing, Jabalpur. Developed with precision through the utilization of Python 3.8 and bolstered by the Django Web framework, this initiative stands as a testament to a student-driven pursuit geared towards the enhancement of the operational fabric of the institute. Its purpose is to provide a comprehensive solution, addressing myriad facets ranging from adept administration management to the facilitation of academic excellence and the efficient handling of departmental tasks, thereby bringing cohesion to the intricate tapestry of campus life.

On the administrative front, Fusion IIIT adeptly manages intricate paperwork and processes. In the academic sphere, it introduces a digital paradigm, simplifying the realms of learning and course management. Its impact, however, transcends these specific domains;Fusion IIIT assumes the role of a genial companion for every facet of the campus, meticulously ensuring the optimal functioning of all processes.

In summary, Fusion IIIT transcends its status as a mere tool;it emerges as a discerning companion, contributing significantly to a more organized and enjoyable milieu for the entire community at PDPM IIITDM Jabalpur.

2. **Purpose of the module**

The purpose of the module is to showcase all available departments, faculty and resources available in this institute, along with the ability to make requests to the faculty and view various announcements made by the faculty and staff members.

The department view will display information regarding the department and facilities offered in the concerned department student details, faculty details, alumni details, and published announcements if any.

3. **Scope of the module**

The Department module will allow students to browse through relevant announcements and view details of faculty or students. This module also allows faculty or admin to make announcements related to either their course or announcements related to their department.

2. User/Actor characteristics
1. **Student :**

   Students can do the following tasks:

- Browse announcements which will show announcements which will be filtered based on courses which the student is attending.
- View department details which will show details about the department and its resources available like labs and equipment.
- View faculty details which will display a list of faculties which will contain a link to their information.
- View alumni details which will display details related to alumni filtered based on their year of passing out.
- View student details which will contain a list of students filtered based on year and program.
2. **Faculty :**

   The faculty can do the following tasks:

- Browse announcements which will show the announcements made by a faculty regarding a particular course or a particular department.
- View department details which will show details about the department and its resources available like labs and equipment.
- View faculty details which will display a list of faculties which will contain a link to their information.
- View alumni details which will display details related to alumni filtered based on the department and their year of passing out.
- View student details which will contain a list of students filtered based on year and program.

**Specific Functionalities:**

- Faculty can announce as per their needs. For Eg. If a faculty needs to make an announcement related to their courses this semester they can select the particular course or if they want to make an announcement for all students of the department they can do so.
3. **Admin :**

   The faculty can do the following tasks:

- Browse announcements which will show the announcements made by a faculty regarding a particular course or a particular department.
- Make announcements which will allow the faculty to make announcements as per their requirements.
- View department details which will show details about the department and its resources available like labs and equipment.
- View faculty details which will display a list of faculties which will contain a link to their information.
- View alumni details which will display details related to alumni filtered based on the department and their year of passing out.
- View student details which will contain a list of students filtered on the basis of year and program.

**Specific Functionalities:**

- Admin can make an announcement as per their needs .

3 Functional Requirements

1. **Use Case Diagram**

![](Aspose.Words.63df42fd-6885-4712-9063-f1cc106823cb.001.png)

2. **Use Case Description** Use Case #1

 

<table><tr><th colspan="1" valign="top">UCID</th><th colspan="2" valign="top">UC#1</th></tr>
<tr><td colspan="1" valign="top">Use case name</td><td colspan="2" valign="top">Browse announcement</td></tr>
<tr><td colspan="1" valign="top">Description</td><td colspan="2" valign="top"><p>Users of the system can browse the available notifications/announcements as per the need of the user.</p><p>Announcements will be fetched on the basis of the course in which the student is enrolled and only those announcements will be visible to a particular student.for a user which is student.</p></td></tr>
<tr><td colspan="1" valign="top">Actor</td><td colspan="2" valign="top">Admin,Student,Faculty</td></tr>
<tr><td colspan="1" valign="top">Precondition</td><td colspan="2" valign="top">The user must be logged in and the system is having the updated information of all the departments and announcements made.</td></tr>
<tr><td colspan="1" rowspan="2" valign="top">Main Flow</td><td colspan="1" valign="top">1\.</td><td colspan="1" valign="top">Actor logs into the system and opens the Department Page.</td></tr>
<tr><td colspan="1" valign="top">2\.</td><td colspan="1" valign="top">Actor selects the Browse announcement tab.</td></tr>
<tr><td colspan="1" valign="top">Post condition</td><td colspan="2" valign="top">The necessary details of the department are displayed.</td></tr>
<tr><td colspan="1" valign="top">Alternate Flow</td><td colspan="2" valign="top">nil</td></tr>
<tr><td colspan="1" valign="top">Sub flow</td><td colspan="2" valign="top">nil</td></tr>
<tr><td colspan="1" valign="top">Global Alternate flow</td><td colspan="1" valign="top">GA1</td><td colspan="1" valign="top">The actor can return to the dashboard at any time by clicking on the dashboard button.</td></tr>
</table>

Use Case #2



<table><tr><th colspan="1" valign="top">UCID</th><th colspan="2" valign="top">UC#2</th></tr>
<tr><td colspan="1" valign="top">Use case name</td><td colspan="2" valign="top">Make New announcement for the admin.</td></tr>
<tr><td colspan="1" valign="top">Description</td><td colspan="2" valign="top">Admin can make new announcement related to department for student and Faculty related to that specific department</td></tr>
<tr><td colspan="1" valign="top">Actor</td><td colspan="2" valign="top">Admin</td></tr>
<tr><td colspan="1" valign="top">Precondition</td><td colspan="2" valign="top">Admin logged in ,opened Department module</td></tr>
<tr><td colspan="1" rowspan="2" valign="top">Main Flow</td><td colspan="1" valign="top">1\.</td><td colspan="1" valign="top">Admin selects the “Make Announcement “tab</td></tr>
<tr><td colspan="1" valign="top">2\.</td><td colspan="1" valign="top">Admin types the announcement and clicks publish.</td></tr>
<tr><td colspan="1" valign="top">Post condition</td><td colspan="2" valign="top">The announcement made by the admin is visible to the faculty and students under the “browse announcement “option.</td></tr>
<tr><td colspan="1" valign="top">Alternate Flow</td><td colspan="2" valign="top">nil</td></tr>
<tr><td colspan="1" valign="top">Sub flow</td><td colspan="2" valign="top">nil</td></tr>
<tr><td colspan="1" rowspan="2" valign="top">Global Alternate flow</td><td colspan="1" rowspan="2" valign="top">GA1</td><td colspan="1" valign="top">The actor can return to the dashboard at any time by clicking on the dashboard button.</td></tr>
<tr><td colspan="1" valign="top">Post condition : the system returns to the actor’s dashboard.</td></tr>
</table>

Use case#3



<table><tr><th colspan="1" valign="top">UCID</th><th colspan="2" valign="top">UC#3</th></tr>
<tr><td colspan="1" valign="top">Use case name</td><td colspan="2" valign="top">make new announcement</td></tr>
<tr><td colspan="1" valign="top">Description</td><td colspan="2" valign="top">Faculty can make new announcement related to department for student or other users related to that specific department</td></tr>
<tr><td colspan="1" valign="top">Actor</td><td colspan="2" valign="top">Faculty</td></tr>
<tr><td colspan="1" valign="top">Precondition</td><td colspan="2" valign="top">Faculty logged in ,opened Department module</td></tr>
<tr><td colspan="1" rowspan="4" valign="top">Main Flow</td><td colspan="1" valign="top">1\.</td><td colspan="1" valign="top">Faculty selects the “Make Announcement “tab</td></tr>
<tr><td colspan="1" valign="top">2\.</td><td colspan="1" valign="top">Faculty selects who he/she wants to make an announcement for i.e either M.Tech/B.Tech students or all students.</td></tr>
<tr><td colspan="1" valign="top">3\.</td><td colspan="1" valign="top">Faculty selects a year. Then the Faculty selects the course which the faculty wants to make an announcement for.</td></tr>
<tr><td colspan="1" valign="top">4\.</td><td colspan="1" valign="top">Faculty publishes the announcement.</td></tr>
<tr><td colspan="1" valign="top">Post condition</td><td colspan="2" valign="top">The announcement made by the faculty is visible to the admin and particular students under the “browse announcement “ option.</td></tr>
<tr><td colspan="1" valign="top">Alternate Flow</td><td colspan="2" valign="top">nil</td></tr>
<tr><td colspan="1" valign="top">Sub flow</td><td colspan="2" valign="top">nil</td></tr>
<tr><td colspan="1" rowspan="2" valign="top">Global Alternate flow</td><td colspan="1" rowspan="2" valign="top">GA1</td><td colspan="1" valign="top">The actor can return to the dashboard at any time by clicking on the dashboard button.</td></tr>
<tr><td colspan="1" valign="top">Post condition : the system returns to the actor’s dashboard.</td></tr>
</table>

Use case #7



<table><tr><th colspan="1" valign="top">UCID</th><th colspan="2" valign="top">UC#4</th></tr>
<tr><td colspan="1" valign="top">Use case name</td><td colspan="2" valign="top">view student detail</td></tr>
<tr><td colspan="1" valign="top">Description</td><td colspan="2" valign="top">The actor can view the student registered in respective departments in the institute according to the batches.</td></tr>
<tr><td colspan="1" valign="top">Actor</td><td colspan="2" valign="top">Student, Faculty,Admin</td></tr>
<tr><td colspan="1" valign="top">Precondition</td><td colspan="2" valign="top">Actor logged in, opens the Department module and the system has updated information about the students.</td></tr>
<tr><td colspan="1" rowspan="3" valign="top">Main Flow</td><td colspan="1" valign="top">1\.</td><td colspan="1" valign="top">Users select the respective department on the main page of the module.</td></tr>
<tr><td colspan="1" valign="top">2\.</td><td colspan="1" valign="top">Users clicks the students tab and selects the batches</td></tr>
<tr><td colspan="1" valign="top">3\.</td><td colspan="1" valign="top">Users clicks on the respective batch to view the details</td></tr>
<tr><td colspan="1" valign="top">Post condition</td><td colspan="2" valign="top">List of the student for the selected option are displayed</td></tr>
<tr><td colspan="1" valign="top">Alternate Flow</td><td colspan="2" valign="top">nil</td></tr>
<tr><td colspan="1" valign="top">Sub flow</td><td colspan="2" valign="top">nil</td></tr>
<tr><td colspan="1" rowspan="2" valign="top">Global Alternate flow</td><td colspan="1" rowspan="2" valign="top">GA1</td><td colspan="1" valign="top">The actor can return to the dashboard at any time by clicking on the dashboard button.</td></tr>
<tr><td colspan="1" valign="top">Post condition: the system returns to the actor’s dashboard.</td></tr>
</table>



<table><tr><th colspan="1" valign="top">UCID</th><th colspan="2" valign="top">UC#5</th></tr>
<tr><td colspan="1" valign="top">Use case name</td><td colspan="2" valign="top">view faculty detail</td></tr>
<tr><td colspan="1" valign="top">Description</td><td colspan="2" valign="top">The actor can view the faculty registered in respective departments in the institute according to the department.</td></tr>
<tr><td colspan="1" valign="top">Actor</td><td colspan="2" valign="top">Student, Faculty,Admin</td></tr>
<tr><td colspan="1" valign="top">Precondition</td><td colspan="2" valign="top">Actor logged in, opens the Department module and the system has updated information of the faculties.</td></tr>
<tr><td colspan="1" rowspan="3" valign="top">Main Flow</td><td colspan="1" valign="top">1\.</td><td colspan="1" valign="top">Users select the respective department on the main page of the module.</td></tr>
<tr><td colspan="1" valign="top">2\.</td><td colspan="1" valign="top">Users select the “Faculty tab”.</td></tr>
<tr><td colspan="1" valign="top">3\.</td><td colspan="1" valign="top">Users clicks on view faculty to view the details</td></tr>
<tr><td colspan="1" valign="top">Post condition</td><td colspan="2" valign="top">List of the faculties for the selected option are displayed</td></tr>
<tr><td colspan="1" valign="top">Alternate Flow</td><td colspan="2" valign="top">nil</td></tr>
<tr><td colspan="1" valign="top">Sub flow</td><td colspan="2" valign="top">nil</td></tr>
<tr><td colspan="1" rowspan="2" valign="top">Global Alternate flow</td><td colspan="1" rowspan="2" valign="top">GA1</td><td colspan="1" valign="top">The actor can return to the dashboard at any time by clicking on the dashboard button.</td></tr>
<tr><td colspan="1" valign="top">Post condition: the system returns to actor’s dashboard.</td></tr>
</table>



<table><tr><th colspan="1" valign="top">UCID</th><th colspan="2" valign="top">UC#6</th></tr>
<tr><td colspan="1" valign="top">Use case name</td><td colspan="2" valign="top">view department details</td></tr>
<tr><td colspan="1" valign="top">Description</td><td colspan="2" valign="top">The actor can view the faculty registered in respective departments in the institute according to the department.</td></tr>
<tr><td colspan="1" valign="top">Actor</td><td colspan="2" valign="top">Student, Faculty,Admin</td></tr>
<tr><td colspan="1" valign="top">Precondition</td><td colspan="2" valign="top">User logged in, opens the Department module and the system has updated information of the department.</td></tr>
<tr><td colspan="1" valign="top">Main Flow</td><td colspan="1" valign="top">1\.</td><td colspan="1" valign="top">User selects the respective department on the main page of the module.</td></tr>
<tr><td colspan="1" valign="top">Post condition</td><td colspan="2" valign="top">List of the department for the selected option are displayed</td></tr>
<tr><td colspan="1" valign="top">Alternate Flow</td><td colspan="2" valign="top">nil</td></tr>
<tr><td colspan="1" valign="top">Sub flow</td><td colspan="2" valign="top">nil</td></tr>
<tr><td colspan="1" rowspan="2" valign="top">Global Alternate flow</td><td colspan="1" rowspan="2" valign="top">GA1</td><td colspan="1" valign="top">The actor can return to the dashboard at any time by clicking on the dashboard button.</td></tr>
<tr><td colspan="1" valign="top">Post condition : the system returns to the actor’s dashboard.</td></tr>
</table>



<table><tr><th colspan="1" valign="top">UCID</th><th colspan="2" valign="top">UC#7</th></tr>
<tr><td colspan="1" valign="top">Use case name</td><td colspan="2" valign="top">View Alumni Details.</td></tr>
<tr><td colspan="1" valign="top">Description</td><td colspan="2" valign="top">The actor can view the faculty registered in respective departments in the institute according to the department.</td></tr>
<tr><td colspan="1" valign="top">Actor</td><td colspan="2" valign="top">Student, Faculty,Admin</td></tr>
<tr><td colspan="1" valign="top">Precondition</td><td colspan="2" valign="top">User logged in, opens the Department module and the system has updated information of the department.</td></tr>
<tr><td colspan="1" valign="top">Main Flow</td><td colspan="1" valign="top">1\.</td><td colspan="1" valign="top">User selects the view Alumni tab on the main page of the module.</td></tr>
<tr><td colspan="1" valign="top">Post condition</td><td colspan="2" valign="top">List of the Alumni for the selected option are displayed</td></tr>
<tr><td colspan="1" valign="top">Alternate Flow</td><td colspan="2" valign="top">nil</td></tr>
<tr><td colspan="1" valign="top">Sub flow</td><td colspan="2" valign="top">nil</td></tr>
<tr><td colspan="1" rowspan="2" valign="top">Global Alternate flow</td><td colspan="1" rowspan="2" valign="top">GA1</td><td colspan="1" valign="top">The actor can return to the dashboard at any time by clicking on the dashboard button.</td></tr>
<tr><td colspan="1" valign="top">Post condition : the system returns to the actor’s dashboard.</td></tr>
</table>

3. **Otherconstraints**
1. User Interfaces

The user interface should comply with the color scheming and dashboard design of the FUSIONIIT. Users should be able to navigate from one functionality to another. Inter module navigation should be smooth. Allthe functionalities should be easy to use and no specific training should be required for the usage of the module


2. Tech Stack Used
- **Django**: Django is a high-level Python web framework that encourages rapid development and clean, pragmatic design. It follows the Model-View-Controller (MVC) architectural pattern.
- **Visual Studio Cod**e: Alightweight and versatile code editor commonly used for developing Flutter applications, which offers extensive Flutter and Dart extensions for enhanced development capabilities.
4. Non- Functional Requirements
1. **Performance:**
- The department module should provide quick response times for user interactions, such as department registration, student data modification, and notification retrieval.
- Response time for actions like department registration, student data updates, and notification retrieval should be within acceptable limits, with a maximum page load time of 3 seconds.
2. **Scalability:**
- The system should scale efficiently to accommodate a growing number of students and departments.
- Performance evaluations should be conducted under increasing load conditions to ensure the system remains responsive as the user base expands.
3. **Availability:**
- The department module should aim for a high availability rate, with a target of 99.9% uptime.
- Scheduled maintenance activities should be planned during non-peak hours to minimize impact on users.

4. **Security:**
- Data confidentiality and integrity should be maintained, with secure storage and transmission of sensitive information.
- Role-based authorization should be implemented to ensure that only authorized users, such as faculty members, can view and modify student data.
- Passwords should be securely hashed and stored to prevent unauthorized access.
- The department module should comply with data protection laws and ensure the privacy of student and faculty information.
5. **Usability:**
- The user interface of the department module should be designed to be intuitive and user-friendly,ensuring a positive user experience for both students and faculty.
6. **Reliability:**
- The system should have a high level of reliability,with minimal downtime for maintenance or unexpected issues.
5. Module dependencies with other fusion modules

**5.1. UILevel**

User logs into Fusion portion and lands on the main dashboard.The user (student,faculty,department admin) can click on the department button and go to the department page .From there students are able to view announcements regarding their department,courses and view student,faculty,and alumni details.

The faculty is able to make announcements and browse announcements from the department page.

2. **DB Level :**



|**S.No**|**Table Name**|**Primary Key**|**Foreign Key**|**owner**|**Reference Table**|
| - | - | - | - | - | - |
|1\.|department\_annou ncements|id|maker\_id\_id|fusion\_ admin|globals\_extrainf o|
|2\.|department\_specia lrequest|id|request\_maker\_id|fusion\_ admin|globals\_extrainf o|

3. **Module Level :**

The module will use the notification module for notifying information about announcements.


