**Fusion ERP**

**Software Requirements Specification**

**For**

**AC-6 Department Module (Mobile App)**

**Prepared By**

Anoop Kumar(21BCS026) Alok Kumar(21BCS018) Ankit Singh(21BCS024) Dharavath Vinod(21BCS076) Vishal Parihar(21BCS244)

**Student Mentor: Varun Sandeep Singh(21BCS237) Faculty Mentor: Prof. Pritee Khanna**

Table of Contents

1. Introduction………………………………………………………………………..3
1. Introduction about the Fusion – A brief Description………….….3
1. Purpose of the module …………………………………………………………………………4
1. Scope of the module………………………………………………………………………………4
2. User/Actor Characteristics…………………………………………….5
1. Student……………………………………......................................................................5
1. Faculty………………………………………….……………………………………………………………….5
1. Admin…………………............................................................................................6
3. Functional Requirements…….…….…………………………………7
1. Use case diagram…………………………………………………………………………..……….7
1. Use case description……………………………………………………………………….……..8
1. Other constraints…………………………………………………………………………………...15
1. User Interfaces………………………………………………………………………..….…15
1. Software (Tech) Stack used……………………………………………………..15
4. Non-Functional Requirements….………………………………16
1. Performance…………………………………………………………………………………………….16
1. Scalability…………………………………………………………………………………………………16
1. Availability………………………………………………………………………………………………..16
1. Security………………………………………………………………………………………………………16
5. Module dependencies with other modules.….………16
1. Integration at UI level………………………………………………………………………...16
1. Database level dependencies…………………………………………………………..17
1. Module level dependencies……………………………………………………………….17
1. **Introduction**
1. **Introduction about the Fusion – A brief Description**

Embark on a transformative journey with the FusionIIIT Mobile App, a cutting-edge solution meticulously crafted using Flutter and Dart to enhance the operational landscape of PDPM Indian Institute of Information Technology, Design and Manufacturing, Jabalpur. Developed by proactive students, this mobile app serves as a dynamic companion, seamlessly integrating and automating diverse functions across the campus.

Picture the FusionIIIT Mobile App as your digital ally, streamlining administrative tasks, elevating academic experiences, and ensuring the smooth functioning of various departments. Whether you're navigating complex paperwork on the admin side or seeking a digital touch for enhanced learning and course management, FusionIIIT Mobile App goes beyond the ordinary to foster a well-organized and enjoyable campus life.

Much like its web counterpart, the FusionIIIT Mobile App is not just a tool; it's a friendly companion that accompanies you through every facet of campus life. From simplifying administrative processes to enhancing academic efficiency, this app is designed to make your experience at PDPM IIITDM Jabalpur more organized and enjoyable. Embrace the future of campus management with FusionIIIT Mobile App – your key to a seamlessly integrated and automated campus experience.

2. **Purpose of the module**

This document outlines the specific requirements for the development of the "Department Module" within the Institute's Enterprise Resource Planning (ERP) system. The Department Module aims to establish a comprehensive platform, enabling all students at IIITDMJ to access detailed information about various departments and facilitate their registration into specific departments. Furthermore, it will ensure the timely dissemination of notifications regarding meetings, webinars, and essential announcements made by faculty members. The system will empower faculty members to efficiently access and modify student data, offering an automated and streamlined alternative to the current manual application procedures.

3. **Scope of the module**

The Department module is designed to efficiently view all details regarding students , faculty , department and alumni. Seamless interactions with faculty is facilitated through this module . It has three primary actors : Student , Faculty and Admin.

2. **User/Actor characteristics**
1. **Student**

A student of IIITDM Jabalpur who first logs into the system. He is able to browse through the details of the student, faculty, Alumni and the department

**Role:** View the details of students , faculty, department and alumni. **Specific Functionalities:**

- View Student details
- VIew Faculty details
- View Department details
- View Alumni details
- Browse announcements made by faculty/administrator
2. **Faculty**

Faculty can view details of students,faculty,department and alumni.

**Role:** Make announcement related to academics ,internships or initiatives

**Specific Functionalities:**

- View Student details
- VIew Faculty details
- View Department details
- View Alumni details
- Make announcements
- Browse announcements
3. **Admin**

Head of department

**Role:** Responsible for circulating notification / making announcement regarding meetings/webinar/conferences. Each Department has different admin and the respective admin can make the announcement for that department .

**Specific Functionalities:**

- View Student details
- VIew Faculty details
- View Department details
- View Alumni details
- Make announcements for the faculty and students
- Browse announcements
3. **Functional Requirements**
1. **Use case diagram**

   ![](Aspose.Words.03b6b10e-f281-46bd-b878-717d3c69ada8.001.png)

2. **Use case description Use case #1**



<table><tr><th colspan="1" valign="top">UC ID</th><th colspan="2" valign="top">UC#1</th></tr>
<tr><td colspan="1" valign="top">Use case name</td><td colspan="2" valign="top">View_student_detail</td></tr>
<tr><td colspan="1" valign="top">Description</td><td colspan="2" valign="top">The actor can view the student registered in respective departments in the institute according to the batches.</td></tr>
<tr><td colspan="1" valign="top">Actor</td><td colspan="2" valign="top">Student,Faculty,Admin</td></tr>
<tr><td colspan="1" valign="top">Precondition</td><td colspan="2" valign="top">Actor logged in, opens Department module and system has updated information of the students.</td></tr>
<tr><td colspan="1" rowspan="3" valign="top">Main Flow</td><td colspan="1" valign="top">1\.</td><td colspan="1" valign="top">Actor selects the respective department on the main page of the module.</td></tr>
<tr><td colspan="1" valign="top">2\.</td><td colspan="1" valign="top">Actor clicks the “Students” tab and selects the batches.</td></tr>
<tr><td colspan="1" valign="top">3\.</td><td colspan="1" valign="top">Actor clicks on the respective batch to view the details.</td></tr>
<tr><td colspan="1" valign="top">Post condition</td><td colspan="2" valign="top">List of the student for the selected option are displayed</td></tr>
<tr><td colspan="1" valign="top">Alternate Flow</td><td colspan="2" valign="top">nil</td></tr>
<tr><td colspan="1" valign="top">Sub flow</td><td colspan="2" valign="top">nil</td></tr>
<tr><td colspan="1" rowspan="2" valign="top">Global Alternate flow</td><td colspan="1" rowspan="2" valign="top">GA1</td><td colspan="1" valign="top">The actor can return to the dashboard at any time by clicking on the dashboard button.</td></tr>
<tr><td colspan="1" valign="top">Post condition: The system returns to the actor’s dashboard.</td></tr>
</table>

**Use case #3****
<table><tr><th colspan="1" valign="top">UC ID</th><th colspan="2" valign="top">UC#2</th></tr>
<tr><td colspan="1" valign="top">Use case name</td><td colspan="2" valign="top">View_faculty_detail</td></tr>
<tr><td colspan="1" valign="top">Description</td><td colspan="2" valign="top">The actor can view the faculty registered in respective departments in the institute according to the department.</td></tr>
<tr><td colspan="1" valign="top">Actor</td><td colspan="2" valign="top">Student,Faculty,Admin</td></tr>
<tr><td colspan="1" valign="top">Precondition</td><td colspan="2" valign="top">Actor logged in, opens Department module and system has updated information of the faculties.</td></tr>
<tr><td colspan="1" rowspan="3" valign="top">Main Flow</td><td colspan="1" valign="top">1\.</td><td colspan="1" valign="top">Actor selects the respective department on the main page of the module.</td></tr>
<tr><td colspan="1" valign="top">2\.</td><td colspan="1" valign="top">Actor selects the “Faculty tab”.</td></tr>
<tr><td colspan="1" valign="top">3\.</td><td colspan="1" valign="top">Actor clicks on the view faculty to view the details.</td></tr>
<tr><td colspan="1" valign="top">Post condition</td><td colspan="2" valign="top">List of the faculties for the selected option are displayed</td></tr>
<tr><td colspan="1" valign="top">Alternate Flow</td><td colspan="2" valign="top">nil</td></tr>
<tr><td colspan="1" valign="top">Sub flow</td><td colspan="2" valign="top">nil</td></tr>
<tr><td colspan="1" rowspan="2" valign="top">Global Alternate flow</td><td colspan="1" rowspan="2" valign="top">GA1</td><td colspan="1" valign="top">The actor can return to the dashboard at any time by clicking on the dashboard button.</td></tr>
<tr><td colspan="1" valign="top">Post condition: The system returns to the actor’s dashboard.</td></tr>
</table>



<table><tr><th colspan="1" valign="top">UC ID</th><th colspan="2" valign="top">UC#3</th></tr>
<tr><td colspan="1" valign="top">Use case name</td><td colspan="2" valign="top">View _department_detail</td></tr>
<tr><td colspan="1" valign="top">Description</td><td colspan="2" valign="top">The actor can view the faculty registered in respective departments in the institute according to the department.</td></tr>
<tr><td colspan="1" valign="top">Actor</td><td colspan="2" valign="top">Student,Faculty,Admin</td></tr>
<tr><td colspan="1" valign="top">Precondition</td><td colspan="2" valign="top">Actor logged in, opens Department module and system has updated information of the department.</td></tr>
<tr><td colspan="1" valign="top">Main Flow</td><td colspan="1" valign="top">1\.</td><td colspan="1" valign="top">Actor selects the respective department on the main page of the module.</td></tr>
<tr><td colspan="1" valign="top">Post condition</td><td colspan="2" valign="top">List of the department for the selected option are displayed</td></tr>
<tr><td colspan="1" valign="top">Alternate Flow</td><td colspan="2" valign="top">nil</td></tr>
<tr><td colspan="1" valign="top">Sub flow</td><td colspan="2" valign="top">nil</td></tr>
<tr><td colspan="1" rowspan="2" valign="top">Global Alternate flow</td><td colspan="1" rowspan="2" valign="top">GA1</td><td colspan="1" valign="top">The actor can return to the dashboard at any time by clicking on the dashboard button.</td></tr>
<tr><td colspan="1" valign="top">Post condition: The system returns to the actor’s dashboard.</td></tr>
</table>


**Use case #4**



<table><tr><th colspan="1" valign="top">UC ID</th><th colspan="2" valign="top">UC#4</th></tr>
<tr><td colspan="1" valign="top">Use case name</td><td colspan="2" valign="top">View_alumni_detail</td></tr>
<tr><td colspan="1" valign="top">Description</td><td colspan="2" valign="top">The actor can view the Alumni registered in respective departments of the institute according to the department.</td></tr>
<tr><td colspan="1" valign="top">Actor</td><td colspan="2" valign="top">Student,Faculty,Admin</td></tr>
<tr><td colspan="1" valign="top">Precondition</td><td colspan="2" valign="top">Actor logged in, opens Department module and system has updated information of the Alumni.</td></tr>
<tr><td colspan="1" rowspan="3" valign="top">Main Flow</td><td colspan="1" valign="top">1\.</td><td colspan="1" valign="top">Actor selects the respective department on the main page of the module.</td></tr>
<tr><td colspan="1" valign="top">2\.</td><td colspan="1" valign="top">Actor selects the “Alumni tab”.</td></tr>
<tr><td colspan="1" valign="top">3\.</td><td colspan="1" valign="top">Actor clicks on the view Alumni to view the details</td></tr>
<tr><td colspan="1" valign="top">Post condition</td><td colspan="2" valign="top">List of the Alumni for the selected option are displayed</td></tr>
<tr><td colspan="1" valign="top">Alternate Flow</td><td colspan="2" valign="top">nil</td></tr>
<tr><td colspan="1" valign="top">Sub flow</td><td colspan="2" valign="top">nil</td></tr>
<tr><td colspan="1" rowspan="2" valign="top">Global Alternate flow</td><td colspan="1" rowspan="2" valign="top">GA1</td><td colspan="1" valign="top">The actor can return to the dashboard at any time by clicking on the dashboard button.</td></tr>
<tr><td colspan="1" valign="top">Post condition: The system returns to the actor’s dashboard.</td></tr>
</table>

**Use case #5****
<table><tr><th colspan="1" valign="top">UC ID</th><th colspan="2" valign="top">UC#5</th></tr>
<tr><td colspan="1" valign="top">Use case name</td><td colspan="2" valign="top">Browse_announcement</td></tr>
<tr><td colspan="1" valign="top">Description</td><td colspan="2" valign="top">User of the system can browse the available notifications/announcement</td></tr>
<tr><td colspan="1" valign="top">Actor</td><td colspan="2" valign="top">Admin,Student,Faculty</td></tr>
<tr><td colspan="1" valign="top">Precondition</td><td colspan="2" valign="top">The user must be logged in and the system is having the updated information of all the departments and announcements made.</td></tr>
<tr><td colspan="1" rowspan="2" valign="top">Main Flow</td><td colspan="1" valign="top">1\.</td><td colspan="1" valign="top">Actor logs into the system and opens Department Page.</td></tr>
<tr><td colspan="1" valign="top">2\.</td><td colspan="1" valign="top">Actor selects the Browse announcement option</td></tr>
<tr><td colspan="1" valign="top">Post condition</td><td colspan="2" valign="top"><p>The necessary details of the department are displayed .</p><p>The system returns to the actor’s dashboard</p></td></tr>
<tr><td colspan="1" valign="top">Alternate Flow</td><td colspan="2" valign="top">nil</td></tr>
<tr><td colspan="1" valign="top">Sub flow</td><td colspan="2" valign="top">nil</td></tr>
<tr><td colspan="1" valign="top">Global Alternate flow</td><td colspan="1" valign="top">GA1</td><td colspan="1" valign="top">The actor can return to the dashboard at any time by clicking on the dashboard button.</td></tr>
</table>


**Use case #6**

Use case description for Admin (extending User) as an actor.



<table><tr><th colspan="1" valign="top">UC ID</th><th colspan="2" valign="top">UC#6</th></tr>
<tr><td colspan="1" valign="top">Use case name</td><td colspan="2" valign="top">make_announcement</td></tr>
<tr><td colspan="1" valign="top">Description</td><td colspan="2" valign="top">Admin can make new announcement related to department for student and Faculty related to that specific department</td></tr>
<tr><td colspan="1" valign="top">Actor</td><td colspan="2" valign="top">Admin</td></tr>
<tr><td colspan="1" valign="top">Precondition</td><td colspan="2" valign="top">Admin logged in ,opened Department module</td></tr>
<tr><td colspan="1" rowspan="2" valign="top">Main Flow</td><td colspan="1" valign="top">1\.</td><td colspan="1" valign="top">Admin selects the “Make Announcement “ tab</td></tr>
<tr><td colspan="1" valign="top">4\.</td><td colspan="1" valign="top">Admin types the announcement and clicks publish</td></tr>
<tr><td colspan="1" valign="top">Post condition</td><td colspan="2" valign="top">The announcement made by the admin is visible to the faculty and students under the “browse announcement “ option.</td></tr>
<tr><td colspan="1" valign="top">Alternate Flow</td><td colspan="2" valign="top">nil</td></tr>
<tr><td colspan="1" valign="top">Sub flow</td><td colspan="2" valign="top">nil</td></tr>
<tr><td colspan="1" rowspan="2" valign="top">Global Alternate flow</td><td colspan="1" rowspan="2" valign="top">GA1</td><td colspan="1" valign="top">The actor can return to the dashboard at any time by clicking on the dashboard button.</td></tr>
<tr><td colspan="1" valign="top">Post condition: The system returns to the actor’s dashboard.</td></tr>
</table>

**Use case #7**

Use case description for Faculty (extending User) as an actor.



<table><tr><th colspan="1" valign="top">UC ID</th><th colspan="2" valign="top">UC#7</th></tr>
<tr><td colspan="1" valign="top">Use case name</td><td colspan="2" valign="top">make_announcement</td></tr>
<tr><td colspan="1" valign="top">Description</td><td colspan="2" valign="top">Faculty can make new announcement related to department for student and admin related to that specific department</td></tr>
<tr><td colspan="1" valign="top">Actor</td><td colspan="2" valign="top">Faculty</td></tr>
<tr><td colspan="1" valign="top">Precondition</td><td colspan="2" valign="top">Faculty logged in ,opened Department module</td></tr>
<tr><td colspan="1" rowspan="4" valign="top">Main Flow</td><td colspan="1" valign="top">1\.</td><td colspan="1" valign="top">Faculty selects the “Make Announcement “ tab</td></tr>
<tr><td colspan="1" valign="top">2\.</td><td colspan="1" valign="top">Faculty selects who he/she wants to make an announcement for i.e. either B.Tech/M.Tech students or all students.</td></tr>
<tr><td colspan="1" valign="top">3\.</td><td colspan="1" valign="top">Faculty selects a year .Then faculty selects the course which the faculty wants to make an announcement for.</td></tr>
<tr><td colspan="1" valign="top">4\.</td><td colspan="1" valign="top">Faculty types the announcement and clicks publish</td></tr>
<tr><td colspan="1" valign="top">Post condition</td><td colspan="2" valign="top">The announcement made by the faculty is visible to the admin and particular students under the “browse announcement “ option.</td></tr>
<tr><td colspan="1" valign="top">Alternate Flow</td><td colspan="2" valign="top">nil</td></tr>
<tr><td colspan="1" valign="top">Sub flow</td><td colspan="2" valign="top">nil</td></tr>
<tr><td colspan="1" valign="top">Global Alternate flow</td><td colspan="1" valign="top">GA1</td><td colspan="1" valign="top">The actor can return to the dashboard at any time by clicking on the dashboard button.</td></tr>
</table>



|||Post condition: The system returns to the actor’s dashboard.|
| :- | :- | :- |

3. **Other constraints**
1. **User Interface**
- The application's interface will be developed using Flutter and Dart and is intended to be hosted on a mobile platform.
- The module will experience differing initial load times based on the strength of the mobile device's internet connection, influenced by the source media from which it is accessed.
- The mobile app's user interface should prioritize simplicity and ease of use in its design.
2. **Software(Tech) Stack Used**
- **Flutter SDK**: The official software development kit for building natively compiled applications for mobile, web, and desktop from a single codebase.
- **Dart Programming Language**: The language used to write Flutter applications, providing a reactive and component-based structure.
- **Flutter Framework**: The UI toolkit that facilitates the creation of natively compiled applications for mobile, web, and desktop from a single codebase.
- **Android Studio**: Popular integrated development environments (IDEs) for Flutter development, offering features like code completion, debugging, and more.
- **Visual Studio Code with Flutter Extension**: A lightweight and powerful code editor with extensions for Flutter development.
- **Firebase**: A mobile and web application development platform that provides various services such as authentication, cloud storage, and a real-time database.
- **Git**: A version control system commonly used to manage and track changes in the source code.
- **GitHub**: Platforms for hosting and collaborating on Git repositories.
4. **Non-Functional Requirements**
1. **Performance**

The system is required to exhibit prompt responsiveness to user interactions. Specifically, the response time for actions related to booking,inventory updates, and notifications is mandated to be minimized.

2. **Scalability**

The system must demonstrate the capability to accommodate a substantial volume of concurrent users. Evaluation of system performance should be conducted under conditions of increasing load.

3. **Availability**

The system is expected to maintain an availability rate of 99.9%, ensuring continuous operational functionality.

4. **Security**

Robust measures must be implemented to ensure the confidentiality and integrity of data. Role-based authorization mechanisms should be in place to restrict users to actions pertinent to their designated roles

5. **Module dependencies with other modules**
1. **Integration at the UI level**

Users log into the Fusion application and land on the main dashboard. The user (student, faculty, and other community members of IIITDMJ ) can navigate to the department module . Navigation should include direct links or buttons in Fusion's menu, ensuring a clear path for each actor (Student, Faculty,Admin) to access their specific functionalities within the Department Module.

2. **Database level dependencies**



|**S.No**|**Table Name**|**Primary Key**|**Foreign Key**|**Owner**|**Reference Table**|
| - | - | :- | :- | - | :- |
|1\.|department\_a nnouncements|id|maker\_id \_id|fusion\_ad min|globals\_extr ainfo|
|2\.|department\_s pecialrequest|id|request\_ maker\_id|fusion\_ad min|globals\_extr ainfo|

3. **Module level dependencies**

Department registration Module interact with Notification, and Dashboard.

Faculty details are gathered from HR department and Alumni details are gathered from Training & Placement cell.

Student details from course registration .
