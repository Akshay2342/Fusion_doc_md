**Fusion ERP** 

**Software Requirements Specification** 

**for** 

**AC7-EXAMINATION** 

**Mobile App**

**Mentor: Dr. Munesh Singh  Prepared by:**  

Jatin Yadav        -  21bcs104 Mayank Gurjar   -  21bcs131 Pankaj    -  21bcs154 Anushka Bisen   -  21bec022 Ashish    -  21bec027  Shreya Singh   -  21bcs195 (Lead) 

**Introduction** 

1. **Introduction about the Fusion**  

` `FusionIIIT stands as a testament to the seamless integration and automation of         diverse functions within PDPM Indian Institute of Information Technology, Design and Manufacturing, Jabalpur. Crafted with precision using Python 3.8 and powered by the Django Web framework, this initiative is a student-driven endeavor designed to elevate the institute's operational landscape. Encompassing everything from efficient administration management to academic prowess and miscellaneous departmental tasks, FusionIIIT is a holistic solution that harmonizes the intricacies of campus life. 

Imagine it as a digital wizard that takes care of everything, from organizing the administrative stuff to making academics smoother. It's not just limited to the usual tasks; FusionIIIT jumps into various departments and sections, making sure every corner of campus life runs smoothly. 

In the admin side, it handles the complicated paperwork and processes. For academics, it brings a digital touch, making learning and managing courses easier. But it doesn't stop there; FusionIIIT is like a friendly companion for all the different parts of the campus, making sure everything works well. 

In simpler terms, FusionIIIT is not just a tool – it's a helpful friend, making life at PDPM IIITDM Jabalpur more organized and enjoyable for everyone. 

2. **Purpose of the module**

The Examination Module serves as a comprehensive platform designed to facilitate the streamlined and efficient management of the result declaration process within an academic institution. This module is a crucial component of the academic ecosystem, providing a user- friendly interface for faculty members to submit grades and marks, while also offering robust tools for academic administrators to analyze results and ensure a fair and smooth outcome for students.

3. **Scope of the module**

The Examination Module is designed to serve as a robust platform for the streamlined and effective declaration of academic results, involving two primary actors: faculty and administrators. For faculty members, the module provides a user-friendly interface where they can submit grades and marks seamlessly.On the other hand, administrators leverage the module's analytical tools to gain insights into overall performance trends. They can conduct in-depth result analyses, comparing data across courses and semesters.Examination Module plays a crucial role in ensuring a fair, transparent, and efficient result declaration process within academic institutions.

**User/Actor characteristics** 

1. **Acad Admin:**

Represents individuals who intend to handle all examination related functionalities and oversees the strategic implementation, management, and optimization of the system. 

Role: Verifies and analyzes grades submitted by faculty. **Specific Functionalities:**

1. Submits grades for different courses enrolled. 
1. Modify grades if anywhere required. 
1. Generate results after compiling all grades. 
1. Make Important Announcements and notify students about result and grades related information. 
5. Verify the result if any student finds any discrepancy. 
2. **Faculty In charge:** 

Role: The only role of the faculty is to submit the grades after checking and verifying the marks. 

**Specific Functionalities:**

1. Enter and submit grades for students based on their performance in exams,Assignments,and Other assessments.
1. Verify and ensure the accuracy of the entered grades before submission. 

` `**Functional Requirements** 

1. **Use Case Diagram**

![](Aspose.Words.12bd7340-a340-4770-b93a-75162eb8b363.001.jpeg)

2. **Use case Description**



<table><tr><th colspan="1"><b>UC ID</b></th><th colspan="2">UC#1</th></tr>
<tr><td colspan="1"><b>Use case Name</b></td><td colspan="2"><b>Submit Grade</b></td></tr>
<tr><td colspan="1"><b>Description</b></td><td colspan="2">The Academic Administrator submits grades for a specific examination, entering the results for each student.</td></tr>
<tr><td colspan="1"><b>Actor</b></td><td colspan="2">Academic Administrator , Faculty</td></tr>
<tr><td colspan="1"><b>Precondition</b></td><td colspan="2">The Academic Administrator is logged into the examination module.</td></tr>
<tr><td colspan="1" rowspan="7" valign="top"><b>Main Flow</b></td><td colspan="1">1</td><td colspan="1">Academic Administrator selects the "Submit Grade” option.</td></tr>
<tr><td colspan="1">2</td><td colspan="1">System displays a list of available examinations.</td></tr>
<tr><td colspan="1">3</td><td colspan="1">Academic Administrator selects the examination for which grades are to be submitted.</td></tr>
<tr><td colspan="1">4</td><td colspan="1">System displays a list of enrolled students for the selected examination.</td></tr>
<tr><td colspan="1">5</td><td colspan="1">Academic Administrator enters the grades for each student.</td></tr>
<tr><td colspan="1">6</td><td colspan="1">System validates the entered grades.[A1]</td></tr>
<tr><td colspan="1">7</td><td colspan="1">System saves the submitted grades.[A2]</td></tr>
</table>



<table><tr><th colspan="1"></th><th colspan="1">8</th><th colspan="2">System displays a confirmation message for successful grade submission.</th></tr>
<tr><td colspan="1"><b>Post conditions</b> </td><td colspan="3">` `Grades for the selected examination have been successfully submitted by the Academic Administrator.</td></tr>
<tr><td colspan="1" rowspan="4"><b>Alternate Flow</b></td><td colspan="1" rowspan="2">A1</td><td colspan="1">1</td><td colspan="1">System displays an error message for invalid grades.</td></tr>
<tr><td colspan="1">2</td><td colspan="1">Academic Administrator corrects the grades.</td></tr>
<tr><td colspan="1" rowspan="2" valign="top">A2</td><td colspan="1">1</td><td colspan="1">System displays an error message for a submission failure.</td></tr>
<tr><td colspan="1">2</td><td colspan="1">Academic Administrator retries the grade submission.</td></tr>
<tr><td colspan="1" valign="top"><b>Sub Flow</b></td><td colspan="3" valign="top">NIL</td></tr>
<tr><td colspan="1"><b>Global Alternate Flow</b></td><td colspan="1">GA1</td><td colspan="2">Academic Administrator cancels the grade submission.  No grades are submitted. System displays the main menu.</td></tr>
</table>



<table><tr><th colspan="1"><b>UC ID</b></th><th colspan="2">UC#2</th></tr>
<tr><td colspan="1"><b>Use case Name</b></td><td colspan="2">` `<b>Moderate Grade</b></td></tr>
<tr><td colspan="1"><b>Description</b></td><td colspan="2" valign="top">The Academic Administrator moderates grades for a specific examination, reviewing and adjusting the submitted grades if necessary.</td></tr>
<tr><td colspan="1"><b>Actor</b></td><td colspan="2">Academic Administrator</td></tr>
<tr><td colspan="1"><b>Precondition</b></td><td colspan="2">The Academic Administrator is logged into the examination module.</td></tr>
<tr><td colspan="1" rowspan="9" valign="top"><b>Main Flow</b></td><td colspan="1">1</td><td colspan="1">Academic Administrator selects the “Moderate Grade" option.</td></tr>
<tr><td colspan="1">2</td><td colspan="1">System displays a list of available examinations.</td></tr>
<tr><td colspan="1">3</td><td colspan="1">Academic Administrator selects the examination for which grades are to be moderated .</td></tr>
<tr><td colspan="1">4</td><td colspan="1" valign="top">System displays a list of enrolled students and their submitted grades for the selected examination.</td></tr>
<tr><td colspan="1">5</td><td colspan="1" valign="top">Academic Administrator reviews the submitted grades and identifies any adjustments needed.</td></tr>
<tr><td colspan="1">6</td><td colspan="1">Academic Administrator adjusts grades as necessary.</td></tr>
<tr><td colspan="1">7</td><td colspan="1">System validates the moderated grades.[A1]</td></tr>
<tr><td colspan="1">8</td><td colspan="1">System saves the moderated grades.</td></tr>
<tr><td colspan="1">9</td><td colspan="1" valign="top">System displays a confirmation message for successful grade moderation.</td></tr>
</table>



<table><tr><th colspan="1"><b>Post conditions</b> </th><th colspan="3" valign="top">` `Grades for the selected examination have been successfully moderated by the Academic Administrator.</th></tr>
<tr><td colspan="1" rowspan="2"><b>Alternate Flow</b></td><td colspan="1" rowspan="2">A1</td><td colspan="1">1</td><td colspan="1" valign="top">System displays an error message for invalid moderated grades.</td></tr>
<tr><td colspan="1">2</td><td colspan="1" valign="top">Academic Administrator corrects the grades.</td></tr>
<tr><td colspan="1" valign="top"><b>Sub Flow</b></td><td colspan="3" valign="top">NIL</td></tr>
<tr><td colspan="1"><b>Global Alternate Flow</b></td><td colspan="1">GA1</td><td colspan="2" valign="top">Academic Administrator cancels the grade moderation.  No grades are moderated. System displays the main menu .</td></tr>
</table>



<table><tr><th colspan="1"><b>UC ID</b></th><th colspan="2">UC#3</th></tr>
<tr><td colspan="1"><b>Use case Name</b></td><td colspan="2"><b>Authenticated Result</b></td></tr>
<tr><td colspan="1"><b>Description</b></td><td colspan="2" valign="top"><p>The Academic Administrator verifies the results for a specific examination, considering any adjustments made during the moderation process and producing the </p><p>official results for making an announcement.</p></td></tr>
<tr><td colspan="1"><b>Actor</b></td><td colspan="2">Academic Administrator</td></tr>
<tr><td colspan="1"><b>Precondition</b></td><td colspan="2">` `Moderation of grades for the selected examination has been completed.</td></tr>
<tr><td colspan="1" rowspan="9" valign="top"><b>Main Flow</b></td><td colspan="1">1</td><td colspan="1">Academic Administrator selects the “Verify Result” option.</td></tr>
<tr><td colspan="1">2</td><td colspan="1">System displays a list of available examinations.</td></tr>
<tr><td colspan="1">3</td><td colspan="1" valign="top">The Academic Administrator selects the examination for which final results are to be verified.</td></tr>
<tr><td colspan="1">4</td><td colspan="1">Academic administrator verifies the final generated result . </td></tr>
<tr><td colspan="1">5</td><td colspan="1" valign="top">System compiles the moderated grades and calculates the preliminary final results.</td></tr>
<tr><td colspan="1">6</td><td colspan="1">The Academic Administrator reviews the generated results.</td></tr>
<tr><td colspan="1">7</td><td colspan="1" valign="top">System displays the preliminary final results, including any adjustments made during moderation.</td></tr>
<tr><td colspan="1">8</td><td colspan="1" valign="top">Academic Administrator reviews that authorities have verified the result</td></tr>
<tr><td colspan="1">9</td><td colspan="1">System saves the authenticated preliminary final results.[A1]</td></tr>
</table>



<table><tr><th colspan="1" rowspan="3"></th><th colspan="1">10</th><th colspan="2">Academic Administrator proceeds to finalize the results</th></tr>
<tr><td colspan="1">11</td><td colspan="2" valign="top">System compiles any additional adjustments made during authentication and calculates the official final results.</td></tr>
<tr><td colspan="1">12</td><td colspan="2">System displays a confirmation message </td></tr>
<tr><td colspan="1"><b>Post conditions</b> </td><td colspan="3" valign="top">` `Final results for the selected examination have been successfully verified by the authorities and generated by the Academic Administrator.</td></tr>
<tr><td colspan="1" rowspan="2"><b>Alternate Flow</b></td><td colspan="1" rowspan="2">A1</td><td colspan="1">1</td><td colspan="1" valign="top">System displays an error message for a result generation failure.</td></tr>
<tr><td colspan="1">2</td><td colspan="1" valign="top">Academic Administrator investigates and corrects the issue.</td></tr>
<tr><td colspan="1" valign="top"><b>Sub Flow</b></td><td colspan="3" valign="top">NIL</td></tr>
<tr><td colspan="1"><b>Global Alternate Flow</b></td><td colspan="1">GA1</td><td colspan="2"><p>Academic Administrator </p><p>cancels the result generation. No results are generated. System displays the main menu.</p></td></tr>
</table>



<table><tr><th colspan="1"><b>UC ID</b></th><th colspan="2">UC#4</th></tr>
<tr><td colspan="1"><b>Use case Name</b></td><td colspan="2"><b>Publish Result</b></td></tr>
<tr><td colspan="1"><b>Description</b></td><td colspan="2" valign="top">The Academic Administrator generates the final results for a specific examination, compiling and presenting the grades of enrolled students.</td></tr>
<tr><td colspan="1"><b>Actor</b></td><td colspan="2">Academic Administrator</td></tr>
<tr><td colspan="1"><b>Precondition</b></td><td colspan="2" valign="top">The Academic Administrator is logged into the examination module, and grades for the selected examination have been submitted and moderated.</td></tr>
<tr><td colspan="1" rowspan="9"><b>Main Flow</b></td><td colspan="1">1</td><td colspan="1" valign="top">Academic Administrator selects the “Generate Final Result” option.</td></tr>
<tr><td colspan="1">2</td><td colspan="1">System displays a list of available examinations.</td></tr>
<tr><td colspan="1">3</td><td colspan="1" valign="top">The Academic Administrator selects the examination for which results are to be generated.</td></tr>
<tr><td colspan="1">4</td><td colspan="1">Academic administrator verifies the final generated result . </td></tr>
<tr><td colspan="1">5</td><td colspan="1" valign="top">System displays the final results, including the overall performance of each student.</td></tr>
<tr><td colspan="1">6</td><td colspan="1">The Academic Administrator reviews the generated results.</td></tr>
<tr><td colspan="1">7</td><td colspan="1">Academic Administrator confirms the results for publishing.[A1]</td></tr>
<tr><td colspan="1">8</td><td colspan="1">System saves and publishes the final results.</td></tr>
<tr><td colspan="1">9</td><td colspan="1" valign="top">System displays a confirmation message for successful result generation.</td></tr>
</table>



<table><tr><th colspan="1"><b>Post conditions</b> </th><th colspan="3" valign="top">` `Final results for the selected examination have been successfully generated and published by the Academic Administrator.</th></tr>
<tr><td colspan="1" rowspan="2" valign="top"><b>Alternate Flow</b></td><td colspan="1" rowspan="2" valign="top">A1</td><td colspan="1">1</td><td colspan="1" valign="top">System displays an error message for a result generation failure.</td></tr>
<tr><td colspan="1">2</td><td colspan="1" valign="top">Academic Administrator investigates and corrects the issue.</td></tr>
<tr><td colspan="1" valign="top"><b>Sub Flow</b></td><td colspan="3" valign="top">NIL</td></tr>
<tr><td colspan="1"><b>Global Alternate Flow</b></td><td colspan="1">GA1</td><td colspan="2"><p>Academic Administrator </p><p>cancels the result generation. No results are generated. System displays the main menu.</p></td></tr>
</table>



<table><tr><th colspan="1"><b>UC ID</b></th><th colspan="3">UC#5</th></tr>
<tr><td colspan="1"><b>Use case Name</b></td><td colspan="3">` `<b>Announcements</b></td></tr>
<tr><td colspan="1"><b>Description</b></td><td colspan="3">The Academic Administrator creates and posts announcements related to examinations, providing important information and updates for students and other stakeholders.</td></tr>
<tr><td colspan="1"><b>Actor</b></td><td colspan="3">Academic Administrator</td></tr>
<tr><td colspan="1"><b>Precondition</b></td><td colspan="3">The Academic Administrator is logged into the examination module.</td></tr>
<tr><td colspan="1" rowspan="7"><b>Main Flow</b></td><td colspan="1">1</td><td colspan="2">Academic Administrator selects the “Make Announcements" option.</td></tr>
<tr><td colspan="1">2</td><td colspan="2">System displays the announcement creation interface.</td></tr>
<tr><td colspan="1">3</td><td colspan="2">Academic Administrator enters the announcement content, including the title and details.</td></tr>
<tr><td colspan="1">4</td><td colspan="2">Academic Administrator specifies the target audience (e.g., all students, specific courses).</td></tr>
<tr><td colspan="1">5</td><td colspan="2">Academic Administrator selects the option to post the announcement.</td></tr>
<tr><td colspan="1">6</td><td colspan="2">System saves and posts the announcement.</td></tr>
<tr><td colspan="1">7</td><td colspan="2">System notifies the relevant audience about the new announcement.[A1]</td></tr>
<tr><td colspan="1"><b>Post conditions</b> </td><td colspan="3">` `The announcement has been successfully created, posted, and notified to the specified audience.</td></tr>
<tr><td colspan="1"></td><td colspan="1"></td><td colspan="1">1</td><td colspan="1">System displays an error message for a posting failure.</td></tr>
</table>

**Alternate Flow** A1

**Alternate Flow**

A1

|||2|Academic Administrator corrects the announcement details and retries posting.|
| :- | :- | - | :- |
|**Sub Flow**|NIL|||
|**Global Alternate Flow**|GA1|Academic Administrator cancels the announcement creation. No announcement is posted. System displays the main menu.||



<table><tr><th colspan="1"><b>UC ID</b></th><th colspan="2">UC#6</th></tr>
<tr><td colspan="1"><b>Use case Name</b></td><td colspan="2"><b>Timetable</b></td></tr>
<tr><td colspan="1"><b>Description</b></td><td colspan="2">The Academic Administrator creates the examination timetable and seating arrangement for students in lecture halls based on the courses.</td></tr>
<tr><td colspan="1"><b>Actor</b></td><td colspan="2">Academic Administrator</td></tr>
<tr><td colspan="1"><b>Precondition</b></td><td colspan="2" valign="top">Courses, classrooms, and a list of enrolled students for each course are available in the examination module.</td></tr>
<tr><td colspan="1" rowspan="9" valign="top"><b>Main Flow</b></td><td colspan="1">1</td><td colspan="1" valign="top">Academic Administrator selects the "Create Timetable and Seating Arrangement" option.</td></tr>
<tr><td colspan="1">2</td><td colspan="1">System displays a list of available courses.</td></tr>
<tr><td colspan="1">3</td><td colspan="1">Academic Administrator selects a course for which the examination timetable and seating arrangement are to be created.</td></tr>
<tr><td colspan="1">4</td><td colspan="1" valign="top">System generates a draft timetable for the selected course, considering the available time slots and lecture halls.[A1]</td></tr>
<tr><td colspan="1">5</td><td colspan="1" valign="top">Academic Administrator reviews and adjusts the draft timetable as needed, assigning specific time slots for each exam.</td></tr>
<tr><td colspan="1">6</td><td colspan="1" valign="top">Academic Administrator selects a lecture hall for each exam in the timetable.</td></tr>
<tr><td colspan="1">7</td><td colspan="1" valign="top">System generates a seating arrangement for each exam based on the enrolled students for the selected course.[A2]</td></tr>
<tr><td colspan="1">8</td><td colspan="1" valign="top">Academic Administrator reviews and adjusts the seating arrangement as needed.</td></tr>
<tr><td colspan="1">9</td><td colspan="1" valign="top">Academic Administrator finalizes the timetable and seating arrangement.</td></tr>
</table>



<table><tr><th colspan="1"></th><th colspan="1">10</th><th colspan="2">System saves the final timetable and seating arrangement.</th></tr>
<tr><td colspan="1"><b>Post conditions</b> </td><td colspan="3" valign="top">The examination timetable and seating arrangement for the selected course have been successfully created and saved by the Academic Administrator.</td></tr>
<tr><td colspan="1" rowspan="4"><b>Alternate Flow</b></td><td colspan="1" rowspan="2">A1</td><td colspan="1">1</td><td colspan="1">System detects a lack of available lecture halls for exams.</td></tr>
<tr><td colspan="1">2</td><td colspan="1">Academic Administrator adjusts the timetable or schedules exams in different time slots.</td></tr>
<tr><td colspan="1" rowspan="2">A2</td><td colspan="1">1</td><td colspan="1">System detects a conflict in the seating arrangement (e.g., two students assigned to the same seat).</td></tr>
<tr><td colspan="1">2</td><td colspan="1">Academic Administrator resolves the seating conflict.</td></tr>
<tr><td colspan="1" valign="top"><b>Sub Flow</b></td><td colspan="3" valign="top">NIL</td></tr>
<tr><td colspan="1"><b>Global Alternate Flow</b></td><td colspan="1">GA1</td><td colspan="2">Academic Administrator cancels the timetable creation. No timetable or seating arrangement is created. System displays the main menu.</td></tr>
</table>

**3.4 Other Constraints**

1. **User Interfaces** 

Users  should  be  able  to  navigate  from  one  functionality  to  another.  Inter  module navigation  should  be  smooth. All  the  functionalities  should  be  easy  to  use  and  no specific training should be required for the usage of the module.The upload functionality supports various file formats, making it versatile and accommodating different assessment types. Clear prompts and guidance are provided to facilitate a smooth data entry experience. 

2. **Software (Tech) Stack Used**
1. **Django**
1. **Flutter**
3. **Dart**
3. **Postgresql**

**Non functional requirements** 

Non-functional requirements are those requirements that don’t define the actual working of the system. Non-functional requirements are used to judge the quality of the system. 

Non-functional requirements cover all the remaining requirements which are not 

covered by the functional requirements. They specify criteria that judge the operation of a system, rather than specific behaviors. Non-functional requirements in our project are: 

- Usability 
- Reliability 
- Integrity 
- Performance 
1. **Usability** 

Usability is a quality attribute used to assess how easy the interface is to use. Usability is ease of use. It tells how user friendly the interface is. 

It includes memorability, learnability, and satisfaction. Our software interface has all the above qualities. Any kind of user can easily understand the interface. 

2. **Reliability** 

Reliability is how much the system is consistent in different platforms. The ability of an apparatus system to consistently perform its required function, on demand and without degradation or failure. 

3. **Integrity** 

Integrity means doing the right thing in a reliable way. Data integrity is a fundamental component of security. In its broadcast use, “Data Integrity” refers to the accuracy and 

consistency of data stored in a database or another construct. Data integrity is the overall completeness, accuracy and consistency of data. 

4. **PERFORMANCE** 

Performance is also a major non-functional requirement. Performance Requirements about resources required, response time, transaction rate or anything else having to do with performance. 

**Module dependencies with other fusion modules:**  

1. **UI Level** 
1. This is the first time we are going to integrate the Examination Module in Fusion, there is no section named examination present earlier. 
1. In the Mobile app in the modules section, we will add one more column for examination. 
1. If you are an acad admin then you will be displayed three options: 
1. **Verify Results** : Results will be verified for a particular course. 
1. **Generate Results** : After analyzing and verifying, the results will be                       

generated and uploaded. 

3. **Announce Results** : At the end, students will be notified with the 

announcement of the result. 

4. If you are a faculty member then you will get an option to upload results for a particular course. 
2. **DB Level Dependencies** 

The database with which we are interacting are: 

1) **Student DataBase**(for extracting student information). 
1) **Course DataBase**(for extracting courses with their respective faculty).  
1) **Notifications DataBase**(for storing the time to time notifications that are generated). 

**5.3. Module Level Dependencies:**

The examination module depends upon the **Course Registration Module**(for fetching the students in the respective course), **Department Module**(for fetching the course and their respective faculty), **Notifications Module**(for making the announcement for the final result). 
