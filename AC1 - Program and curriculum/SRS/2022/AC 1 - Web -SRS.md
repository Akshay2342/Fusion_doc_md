Software Requirements

Specification

**for**

**AC-1 (Web Application)**

**Programme and Curriculum**

**Prepared by:**


**21BCS126-Mamidi Ravi Chendraa**

**21BCS066-Chilukuri Surya Manikanta Chowdary 21BCS082-G Srinath Reddy**

**21BCS081-Duggireddy Gnana Sainath Reddy 21BCS125-Maloth Ritesh Pragnu Naik 21BCS197-Shubh mehta (Student mentor)**

**Faculty Mentor - Dr. Vinod Kumar Jain (Head CSE)**

Table of Contents
1. #### **Introduction**
   1. Introduction about the Fusion
   1. Purpose of the module
   1. Scope of the module
1. #### **User/Actor Description(characteristics)**
1. **Functional Requirements**
   1. Use case Diagram
   1. Use case description
   1. Other Functional Requirements
   1. Other Constraints
      1. User Interfaces
      1. Software (Tech) Stack Used
      1. Business rules (if any) – (Functional level constraints other than pre- condition/ post-conditions in use cases)
1. #### **Non-Functional Requirements**
1. **Module dependencies with other fusion modules**

5\.1. UI Level

5\.2 DB Level Dependencies

5\.3. Module Level Dependencies

1. # **Introduction**
   1. ### **Introduction about the Fusion**
FusionIIIT stands as a testament to the seamless integration and automation of diverse functions within PDPM Indian Institute of Information Technology, Design and

Manufacturing, Jabalpur. Crafted with precision using Python 3.8 and powered by the Django Web framework, this initiative is a student-driven endeavor designed to elevate the institute's operational landscape. Encompassing everything from efficient administration management to academic prowess and miscellaneous departmental tasks, FusionIIIT is a holistic solution that harmonizes the intricacies of campus life.

Imagine it as a digital wizard that takes care of everything, from organizing the administrative stuff to making academics smoother. It's not just limited to the usual tasks; FusionIIIT jumps into various departments and sections, making sure every corner of campus life runs smoothly.

In the admin side, it handles the complicated paperwork and processes. For academics, it

brings a digital touch, making learning and managing courses easier. But it doesn't stop there; FusionIIIT is like a friendly companion for all the different parts of the campus, making sure everything works well.

In simpler terms, FusionIIIT is not just a tool – it's a helpful friend, making life at PDPM IIITDM Jabalpur more organized and enjoyable for everyone.


1. #### **Purpose**
The objective of this module is to provide addition of new programmes and effective management of various curriculum for different programmes offered in institute. Each programme could update its curriculum for respective batch.

This module not only serves the above purpose but in addition to that , viewing the various programmes and curriculums, batches, disciplines offered in the institute is also provided along with viewing timetable and academic calendar too.


1. #### **Product Scope**
The scope of the application covers the entire Programmes & its Curriculums offered by the Institute where the user can view their desired curriculum

,programme, discipline and batch,along with academic calendar and timetable.


1. # **User/Actor Description(characteristics)**
   1. ### **Student:**
Represents	individuals	who	intend	to	browse	program	catalog,	browsing curriculum catalog.

**Role:** can browse program catalog, browse curriculum catalog.
#### **Specific Functionalities:**
- Can Search specific programme, curriculum, courses, based on name or discipline.
- Can view course info in detail.
  1. ## **ACAD ADMINISTRATOR:**
Responsible for managing and updating information related to academic program and curriculum.

**Role:** Add and update programme , curriculum , courses .
#### **Specific Functionalities:**
- Can add or modify the contents of Programme , Curriculum , Courses.

1. ## **HEAD OF DEPARTMENT:**
Represents individuals who are the head of certain departments in the institute.

**Role:** Same as a User's roles and also forwards or rejects the course proposal form to the Dean of academics.
#### **Specific Functionalities:**
- Forwards/rejects the course proposal form to the dean academics.


1. ## **DEAN ACADEMICS:**
Represents an individual who is a high-ranked academic official and oversees all the major academic operations including curriculum, workloads, approval of courses,evaluating and supervising departments of the institute.

**Role:** Browse the program catalog, browse the curriculum catalog (same as a generic user) and also approve or reject the course proposal form.
#### **Specific Functionalities:**
- Approves or rejects the course proposal form.
  1. ## **FACULTY:**
Represents individuals who can view the current semester courses and can request for course addition/updation.

**Role:** Browse the program catalog, browse the curriculum catalog, and can apply for addition/modification of a course.
#### **Specific Functionalities:**
- Can apply for addition or modification of courses through the course proposal form.

1. # **Functional Requirements**


1. ### **Use case Diagram:**








![](Aspose.Words.77ffcdcf-f699-4feb-a938-e59aa921cc34.001.jpeg)

1. #### **Use case Description:**


1. **Browse\_programme\_catalog**

<table><tr><th colspan="1" valign="top"><b>UCID</b></th><th colspan="2" valign="top"><b>UC#1</b></th></tr>
<tr><td colspan="1" valign="top"><b>Usecase name</b></td><td colspan="2" valign="top"><b>browse_programme_catalog</b></td></tr>
<tr><td colspan="1" valign="top"><b>Actor</b></td><td colspan="2" valign="top"><p></p><p><b>Student, Acad Admin , HOD , Faculty , Dean</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>Description</b></td><td colspan="2" valign="top"><p></p><p><b>The user of the system can browse the available programme categorically.</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>Pre Condition</b></td><td colspan="2" valign="top"><b>The User must be logged-in through their credentials</b></td></tr>
<tr><td colspan="1" rowspan="3" valign="top"><b>Main Flow</b></td><td colspan="1" valign="top"><b>1</b></td><td colspan="1" valign="top"><p></p><p><b>The Actor logs into the system.</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>2</b></td><td colspan="1" valign="top"><p></p><p><b>The Actor then opens the Programme and Curriculum module.</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>3</b></td><td colspan="1" valign="top"><p></p><p><b>The Actor can see the available Programmes the Institute can offer.[S1]</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>Sub flow</b></td><td colspan="2" valign="top"><b>Extend “browse_curriculum_catalogue”.</b></td></tr>
<tr><td colspan="1" valign="top"><b>Post Condition</b></td><td colspan="2" valign="top"><b>The necessary details of the Programmes are displayed.</b></td></tr>
</table>

1. **Browse\_curriculum\_catalog**


<table><tr><th colspan="1" valign="top"><b>UCID</b></th><th colspan="2" valign="top"><b>UC#2</b></th></tr>
<tr><td colspan="1" valign="top"><b>Usecase name</b></td><td colspan="2" valign="top"><b>Browse_curriculum_catalogue</b></td></tr>
<tr><td colspan="1" valign="top"><b>Actor</b></td><td colspan="2" valign="top"><p></p><p><b>Student, Acad Admin , HOD , Faculty , Dean</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>Description</b></td><td colspan="2" valign="top"><p></p><p><b>The user of the system can browse the available curriculums categorically.</b></p><p>[<b>https://www.iiitdmj.ac.in/academics/curriculum.php</b>](http://www.iiitdmj.ac.in/academics/curriculum.php)</p></td></tr>
<tr><td colspan="1" valign="top"><b>Pre Condition</b></td><td colspan="2" valign="top"><b>The User must be logged-in through their credentials</b></td></tr>
<tr><td colspan="1" rowspan="4" valign="top"><b>Main Flow</b></td><td colspan="1" valign="top"><b>1</b></td><td colspan="1" valign="top"><p></p><p><b>The Actor logs into the system.</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>2</b></td><td colspan="1" valign="top"><p></p><p><b>The Actor then opens the Programme and Curriculum module.</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>3</b></td><td colspan="1" valign="top"><p></p><p><b>The Actor then selects the desired programme.</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>4</b></td><td colspan="1" valign="top"><p></p><p><b>The Actor now can see the various curriculums for that programme by clicking the curriculum link.</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>Post Condition</b></td><td colspan="2" valign="top"><b>The necessary details of the curriculum are displayed.</b></td></tr>
</table>

1. **add\_programme**


<table><tr><th colspan="1" valign="top"><b>UCID</b></th><th colspan="2" valign="top"><b>UC#3</b></th></tr>
<tr><td colspan="1" valign="top"><b>Usecase name</b></td><td colspan="2" valign="top"><b>add_programme</b></td></tr>
<tr><td colspan="1" valign="top"><b>Actor</b></td><td colspan="2" valign="top"><p></p><p><b>Acad Admin</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>Description</b></td><td colspan="2" valign="top"><p></p><p><b>The Acad Admin can add a new programme that institute can offer</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>Pre Condition</b></td><td colspan="2" valign="top"><b>The User must be logged-in through their credentials</b></td></tr>
<tr><td colspan="1" rowspan="5" valign="top"><b>Main Flow</b></td><td colspan="1" valign="top"><b>1</b></td><td colspan="1" valign="top"><b>The User logs into the system</b></td></tr>
<tr><td colspan="1" valign="top"><b>2</b></td><td colspan="1" valign="top"><p><b>The actor then opens the programme and</b></p><p><b>curriculum module and clicks on add programme option.[S1]</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>3</b></td><td colspan="1" valign="top"><p></p><p><b>The Actor then adds the discipline, batch year, and the no. of semesters.</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>4</b></td><td colspan="1" valign="top"><p></p><p><b>The Actor then can add courses/elective courses, or labs in each Semester, and the academic load of a</b></p><p><b>particular course.</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>5</b></td><td colspan="1" valign="top"><p></p><p><b>After successfully entering the details, the Actor then clicks on Submit.</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>Sub Flow</b></td><td colspan="2" valign="top"><b>S1. Extend “update_programme”.</b></td></tr>
<tr><td colspan="1" valign="top"><b>Post Condition</b></td><td colspan="2" valign="top"><p><b>The programme is added successfully and is saved in the database and the programme needs to be assigned a</b></p><p><b>curriculum and discipline.</b></p></td></tr>
</table>

1. **update\_programme**


<table><tr><th colspan="1" valign="top"><b>UCID</b></th><th colspan="2" valign="top"><b>UC#4</b></th></tr>
<tr><td colspan="1" valign="top"><b>Usecase name</b></td><td colspan="2" valign="top"><b>update_programme</b></td></tr>
<tr><td colspan="1" valign="top"><b>Actor</b></td><td colspan="2" valign="top"><p></p><p><b>Acad Admin</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>Description</b></td><td colspan="2" valign="top"><p></p><p><b>The Acad Admin can update a programme that institute can offer</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>Pre Condition</b></td><td colspan="2" valign="top"><b>The User must be logged-in through their credentials</b></td></tr>
<tr><td colspan="1" rowspan="4" valign="top"><b>Main Flow</b></td><td colspan="1" valign="top"><b>1</b></td><td colspan="1" valign="top"><b>The User logs into the system</b></td></tr>
<tr><td colspan="1" valign="top"><b>2</b></td><td colspan="1" valign="top"><p><b>The actor then opens the programme and</b></p><p><b>curriculum module and clicks on update programme option.</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>3</b></td><td colspan="1" valign="top"><p></p><p><b>The Actor then does the desired changes</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>4</b></td><td colspan="1" valign="top"><p></p><p><b>After successfully updating the details, the Actor then clicks on Submit.</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>Post Condition</b></td><td colspan="2" valign="top"><b>The programme is updated successfully and is saved in the database.</b></td></tr>
</table>

1. **add\_new\_course\_proposal\_form**


<table><tr><th colspan="1" valign="top"><b>UCID</b></th><th colspan="2" valign="top"><b>UC#5</b></th></tr>
<tr><td colspan="1" valign="top"><b>Usecase name</b></td><td colspan="2" valign="top"><b>add_new_course_proposal_form</b></td></tr>
<tr><td colspan="1" valign="top"><b>Actor</b></td><td colspan="2" valign="top"><p></p><p><b>Faculty</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>Description</b></td><td colspan="2" valign="top"><p></p><p><b>The user of the system can apply for addition or modification of a course.</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>Pre Condition</b></td><td colspan="2" valign="top"><b>The User must be logged-in through their credentials</b></td></tr>
<tr><td colspan="1" rowspan="4" valign="top"><b>Main Flow</b></td><td colspan="1" valign="top"><b>1</b></td><td colspan="1" valign="top"><p></p><p><b>The Actor logs into the system.</b></p></td></tr>
<tr><td colspan="1" valign="top"><p></p><p><b>2</b></p></td><td colspan="1" valign="top"><p></p><p><b>The Actor then opens the programme and curriculum module.</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>3</b></td><td colspan="1" valign="top"><p></p><p><b>The Actor then selects the “course proposal form”.</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>4</b></td><td colspan="1" valign="top"><p></p><p><b>The Actor then fills in the necessary details and then submits the form.[S1]</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>Sub Flows</b></td><td colspan="2" valign="top"><b>S1. Extend “update_course_proposal_form”.</b></td></tr>
<tr><td colspan="1" valign="top"><b>Post Condition</b></td><td colspan="2" valign="top"><b>The form is submitted successfully and is forwarded to the respective head of department.</b></td></tr>
</table>

1. **update\_course\_proposal\_form**


<table><tr><th colspan="1" valign="top"><b>UCID</b></th><th colspan="2" valign="top"><b>UC#6</b></th></tr>
<tr><td colspan="1" valign="top"><b>Usecase name</b></td><td colspan="2" valign="top"><b>update_course_proposal_form</b></td></tr>
<tr><td colspan="1" valign="top"><b>Actor</b></td><td colspan="2" valign="top"><p></p><p><b>Faculty</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>Description</b></td><td colspan="2" valign="top"><p></p><p><b>The user of the system can apply for addition or modification of a course.</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>Pre Condition</b></td><td colspan="2" valign="top"><b>The User must be logged-in through their credentials</b></td></tr>
<tr><td colspan="1" rowspan="4" valign="top"><b>Main Flow</b></td><td colspan="1" valign="top"><b>1</b></td><td colspan="1" valign="top"><p></p><p><b>The Actor logs into the system.</b></p></td></tr>
<tr><td colspan="1" valign="top"><p></p><p><b>2</b></p></td><td colspan="1" valign="top"><p></p><p><b>The Actor then opens the programme and curriculum module.</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>3</b></td><td colspan="1" valign="top"><p></p><p><b>The Actor then selects “course modification form”.</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>4</b></td><td colspan="1" valign="top"><p></p><p><b>The Actor then updates the necessary details and then submits the form.</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>Post Condition</b></td><td colspan="2" valign="top"><b>The form is submitted successfully and is forwarded to the respective head of department.</b></td></tr>
</table>

1. **forward/reject\_course\_proposal\_form**


<table><tr><th colspan="1" valign="top"><b>UCID</b></th><th colspan="2" valign="top"><b>UC#7</b></th></tr>
<tr><td colspan="1" valign="top"><b>Usecase name</b></td><td colspan="2" valign="top"><b>forward/reject_course_proposal_form</b></td></tr>
<tr><td colspan="1" valign="top"><b>Actor</b></td><td colspan="2" valign="top"><p></p><p><b>Head of Department</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>Description</b></td><td colspan="2" valign="top"><p></p><p><b>The user of the system can forward/reject the course addition or modification proposal applied by the faculty.</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>Pre Condition</b></td><td colspan="2" valign="top"><b>The User must be logged-in through their credentials</b></td></tr>
<tr><td colspan="1" rowspan="4" valign="top"><b>Main Flow</b></td><td colspan="1" valign="top"><b>1</b></td><td colspan="1" valign="top"><p></p><p><b>The Actor logs into the system.</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>2</b></td><td colspan="1" valign="top"><p></p><p><b>The Actor then opens the notifications module.</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>3</b></td><td colspan="1" valign="top"><p></p><p><b>The Actor then checks the notifications related to course addition or modifications proposals.</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>4</b></td><td colspan="1" valign="top"><p></p><p><b>The Actor then verifies and decides to forward or reject.</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>Post Condition</b></td><td colspan="2" valign="top"><b>The course proposal form will be forwarded to the dean academics for approval or is not forwarded if rejected by Head of department.</b></td></tr>
</table>


1. **approve/reject\_course\_proposal\_form**


<table><tr><th colspan="1" valign="top"><b>UCID</b></th><th colspan="2" valign="top"><b>UC#8</b></th></tr>
<tr><td colspan="1" valign="top"><b>Usecase name</b></td><td colspan="2" valign="top"><b>approve/reject_course_proposal_form</b></td></tr>
<tr><td colspan="1" valign="top"><b>Actor</b></td><td colspan="2" valign="top"><p></p><p><b>Dean academics</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>Description</b></td><td colspan="2" valign="top"><p></p><p><b>The user of the system can approve/reject the course addition or modification proposal applied by the faculty.</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>Pre Condition</b></td><td colspan="2" valign="top"><b>The User must be logged-in through their credentials</b></td></tr>
<tr><td colspan="1" rowspan="4" valign="top"><b>Main Flow</b></td><td colspan="1" valign="top"><b>1</b></td><td colspan="1" valign="top"><p></p><p><b>The Actor logs into the system.</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>2</b></td><td colspan="1" valign="top"><p></p><p><b>The Actor then opens the notifications module.</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>3</b></td><td colspan="1" valign="top"><p></p><p><b>The Actor then checks the notifications related to course addition or modifications proposals.</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>4</b></td><td colspan="1" valign="top"><p></p><p><b>The Actor then verifies and decides to approve or reject.</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>Post Condition</b></td><td colspan="2" valign="top"><b>The course proposal form will be approved and the Acad admin will be notified to add/modify the course.</b></td></tr>
</table>

1. **add\_curriculum**

<table><tr><th colspan="1" valign="top"><b>UCID</b></th><th colspan="2" valign="top"><b>UC#9</b></th></tr>
<tr><td colspan="1" valign="top"><b>Usecase name</b></td><td colspan="2" valign="top"><b>add_curriculum</b></td></tr>
<tr><td colspan="1" valign="top"><b>Actor</b></td><td colspan="2" valign="top"><p></p><p><b>Acad Admin</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>Description</b></td><td colspan="2" valign="top"><p></p><p><b>The Acad admin can add a new curriculum.</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>Pre Condition</b></td><td colspan="2" valign="top"><b>The User must be logged-in through their credentials</b></td></tr>
<tr><td colspan="1" rowspan="5" valign="top"><b>Main Flow</b></td><td colspan="1" valign="top"><b>1</b></td><td colspan="1" valign="top"><p></p><p><b>The Actor logs into the system.</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>2</b></td><td colspan="1" valign="top"><p></p><p><b>The Actor then opens the Programme and Curriculum module.</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>3</b></td><td colspan="1" valign="top"><p></p><p><b>Actor clicks on the ‘Add curriculum’ option.</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>4</b></td><td colspan="1" valign="top"><p></p><p><b>Then, the Actor selects the disciplines/elective course, no. of semesters, labs in each Semester, and the Academic load of a particular course.</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>5</b></td><td colspan="1" valign="top"><p></p><p><b>After successfully adding the details,the Actor clicks on Submit.[S1]</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>Sub Flows</b></td><td colspan="2" valign="top"><b>S1. Extend “update_curriculum”.</b></td></tr>
<tr><td colspan="1" valign="top"><b>Post Condition</b></td><td colspan="2" valign="top"><b>The new curriculum is added with mentioned details.</b></td></tr>
</table>

1. **update\_curriculum**


<table><tr><th colspan="1" valign="top"><b>UCID</b></th><th colspan="2" valign="top"><b>UC#10</b></th></tr>
<tr><td colspan="1" valign="top"><b>Usecase name</b></td><td colspan="2" valign="top"><b>update_curriculum</b></td></tr>
<tr><td colspan="1" valign="top"><b>Actor</b></td><td colspan="2" valign="top"><p></p><p><b>Acad Admin</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>Description</b></td><td colspan="2" valign="top"><p></p><p><b>The user of the system can update the existing course.</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>Pre Condition</b></td><td colspan="2" valign="top"><b>The User must be logged-in through their credentials</b></td></tr>
<tr><td colspan="1" rowspan="5" valign="top"><b>Main Flow</b></td><td colspan="1" valign="top"><b>1</b></td><td colspan="1" valign="top"><p></p><p><b>The Actor logs into the system.</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>2</b></td><td colspan="1" valign="top"><p></p><p><b>The Actor then opens the Programme and Curriculum module.</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>3</b></td><td colspan="1" valign="top"><p></p><p><b>Actor clicks on the “Update curriculum’ option.</b></p></td></tr>
<tr><td colspan="1" valign="top"><p></p><p><b>4</b></p></td><td colspan="1" valign="top"><p></p><p><b>Then, the Actor updates the necessary details.</b></p></td></tr>
<tr><td colspan="1" valign="top"><p></p><p><b>5</b></p></td><td colspan="1" valign="top"><p></p><p><b>After successfully changing the details,the Actor clicks on Submit.</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>Post Condition</b></td><td colspan="2" valign="top"><b>An update notification is displayed and the curriculum is successfully updated.</b></td></tr>
</table>

1. **add\_new\_course**


<table><tr><th colspan="1" valign="top"><b>UCID</b></th><th colspan="2" valign="top"><b>UC#11</b></th></tr>
<tr><td colspan="1" valign="top"><b>Usecase name</b></td><td colspan="2" valign="top"><b>add_course</b></td></tr>
<tr><td colspan="1" valign="top"><b>Actor</b></td><td colspan="2" valign="top"><p></p><p><b>Acad Admin</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>Description</b></td><td colspan="2" valign="top"><p></p><p><b>The user of the system can add a new course.</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>Pre Condition</b></td><td colspan="2" valign="top"><b>The User must be logged-in through their credentials</b></td></tr>
<tr><td colspan="1" rowspan="5" valign="top"><b>Main Flow</b></td><td colspan="1" valign="top"><b>1</b></td><td colspan="1" valign="top"><p></p><p><b>The Actor logs into the system.</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>2</b></td><td colspan="1" valign="top"><p></p><p><b>The Actor then opens the Programme and Curriculum module.</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>3</b></td><td colspan="1" valign="top"><p></p><p><b>The Actor clicks on the ‘ Add new course’ option</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>4</b></td><td colspan="1" valign="top"><p><b>Actor enters the course name along with all the metadata like Course code,Prerequisites,etc.</b></p><p><b>After that, the Actor can add the syllabus of a particular course.</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>5</b></td><td colspan="1" valign="top"><p></p><p><b>After successfully filling the details, the Actor clicks on Submit.[S1]</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>Sub Flows</b></td><td colspan="1" valign="top"><b>S1</b></td><td colspan="1" valign="top"><b>Extend “update_course”.</b></td></tr>
<tr><td colspan="1" valign="top"><b>Post Condition</b></td><td colspan="2" valign="top"><b>An update notification is displayed and the course is added successfully and is added to the database.</b></td></tr>
</table>

1. **update\_course**

<table><tr><th colspan="1" valign="top"><b>UCID</b></th><th colspan="2" valign="top"><b>UC#12</b></th></tr>
<tr><td colspan="1" valign="top"><b>Usecase name</b></td><td colspan="2" valign="top"><b>update_course</b></td></tr>
<tr><td colspan="1" valign="top"><b>Actor</b></td><td colspan="2" valign="top"><p></p><p><b>Acad Admin</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>Description</b></td><td colspan="2" valign="top"><p></p><p><b>The user of the system can update the existing course details.</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>Pre Condition</b></td><td colspan="2" valign="top"><b>The User must be logged-in through their credentials</b></td></tr>
<tr><td colspan="1" rowspan="5" valign="top"><b>Main Flow</b></td><td colspan="1" valign="top"><b>1</b></td><td colspan="1" valign="top"><p></p><p><b>The Actor logs into the system.</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>2</b></td><td colspan="1" valign="top"><p></p><p><b>The Actor then opens the Programme and Curriculum module.</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>3</b></td><td colspan="1" valign="top"><p></p><p><b>The Actor clicks on the ‘ Update course’ option.</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>4</b></td><td colspan="1" valign="top"><p></p><p><b>Acad Admin updates the necessary meta-data of the course according to the form received from dean academics like course code,prerequisites and the syllabus of a particular course .</b></p></td></tr>
<tr><td colspan="1" valign="top"><p></p><p><b>5</b></p></td><td colspan="1" valign="top"><p></p><p><b>After successfully updating the details, the Actor clicks on Submit.</b></p></td></tr>
<tr><td colspan="1" valign="top"><b>Post Condition</b></td><td colspan="2" valign="top"><b>An update notification is displayed and course details are successfully updated.</b></td></tr>
</table>

1. #### **Other Functional Requirements :**
   1. Search Functionality
   1. Filter and Sort
   1. Integration with other modules like course registration.


1. #### **Other Constraints:**
   1. **User Interfaces :**

A user will be logged in with the password and user-id he/she has with him/her and proceeding further to his home page (Programme and Curriculum Management Module) where he/she will be shown his/her profile by default beside that the programme name (B-Tech/B-Des,

M-Tech/M-Des, etc) will be also displayed. Then the user has to click on any program. After clicking, a new page will come, where he/she needs to fill in the details of the branch, batch, semester, etc in order to view the particular curriculum.

1. **Tech Stack Used :** Database : PostgreSql Backend : Django

4. # **.Non-Functional Requirements**
   1. ### **Performance :**
The system should respond to user interactions quickly. Response time for viewing programmes ,curriculums ,timetables and academic calendar, updates, and notifications should be less .

1. ### **Scalability:**
   The	system	should	handle	a	mass	of	concurrent	users.	System performance should be evaluated under increasing load conditions.
1. ### **Availability:**
   The system should be available 99.9% of the time.
1. ### **Security:**
   Ensure data confidentiality and integrity. Role-based authorization ensures that users can only perform actions relevant to their designated roles.
5. # **Module dependencies with other fusion modules**

1. #### **UI Level**
User Authentication and Authorization:

0. Dependency: Implementing a secure and role-based authentication system is crucial. Students should have read-only access, while academic administrators should have permissions to update or add new courses.

Search and Filtering Functionality:

0. Dependency: Users, especially students, need the ability to search for programs and courses easily. Admins should have filtering options for efficient course management.
0. Implementation: Include search bars, filters, and sorting options to enhance the user experience. Ensure that admins have convenient tools for quickly finding and managing courses.
0. **Example** : **Full-text search (fts)** in a web application involves using a search engine or a database feature that allows searching through the content of textual data efficiently.



Data Presentation and Visualization:

0. Dependency: Effective presentation of program details, courses, and curriculum is essential for user understanding. Admins need

   user-friendly interfaces to add or update course information.

0. Implementation: Use visually appealing and organized layouts to display program details. Implement forms and interfaces for admins to interact with data, including features for adding, updating, and deleting courses.


#### **5.2 DB Level Dependencies**
The schemas that are needed by other modules are:

1 . course

2 . programme\_curriculum\_course;

3 . programme\_curriculum\_course\_prerequisite\_courses

4 . programme\_curriculum\_course\_disciplines


#### **5.3. Module Level Dependencies**

Course registration, notifications and course management modules are the modules dependent on this module.

The course registration module will require various details like course name, course id, discipline offered, prerequisites of the course.

The course management module will require course name ,course id and discipline offered, prerequisites of the course.

The notifications module will require to generate several important notifications like modification of course, curriculum to the respective users.
