Fusion ERP

**Software Requirements Specification**

For

**Awards and Scholarships Module (AC5 - WEB)**

Team mentor - **Dr. Ayan Seal**

Prepared by -

1. Nitya Tiwari (21BCS150)
1. Siddhi Gubrele (21BCS201)
1. Swati Tiwari (21BCS218)
1. Utkarsh Chaturvedi (21BCS227)
1. Utkarsh Raj (21BCS228)

Team Lead - Sudheer Dagar

<a name="_page1_x72.00_y120.93"></a>**Table of Contents**

[**Table of Contents** ](#_page1_x72.00_y120.93)[Revision History**](https://docs.google.com/document/d/1LlYkc220ir_8dbX34LshMYrsDrpdXUY0/edit#heading=h.30j0zll)

**Introduction**

1. Introduction to Fusion
1. About the module
1. Scope of the module
1. Purpose
1. Actors and functionality

**User/Actor[ Description**](https://docs.google.com/document/d/1LlYkc220ir_8dbX34LshMYrsDrpdXUY0/edit#heading=h.2et92p0)**

4. User
4. Student
4. SPACS Convener (Faculty)
4. SPACS Assistant (staff)

**Functional Requirements**

8. [Use case Diagram](https://docs.google.com/document/d/1LlYkc220ir_8dbX34LshMYrsDrpdXUY0/edit#heading=h.2s8eyo1)
8. Use case description
1. Use case Description for user as an actor
1. Use case Description for Student as an actor
1. Use case Description for SPACS Convenor as an actor
1. Use case Description for SPACS Assistant as an actor

3\.3 Other Functional Requirements (Suggestions)

**Non-Functional Requirements**

1. PERFORMANCE REQUIREMENTS
1. Security Requirements
1. Accessibility
1. Business Rules

[**List of open issues with the module 10** ](https://docs.google.com/document/d/1LlYkc220ir_8dbX34LshMYrsDrpdXUY0/edit#heading=h.1ksv4uv)[Suggestions**](https://docs.google.com/document/d/1LlYkc220ir_8dbX34LshMYrsDrpdXUY0/edit#heading=h.44sinio)

1. **Introduction**
1. **Introduction to Fusion**

FusionIIIT at PDPM Indian Institute of Information Technology, Design and Manufacturing, Jabalpur, stands as a testament to the seamless integration and automation of diverse functions. Crafted with precision using Python 3.8 and powered by the Django Web framework, this student-driven initiative aims to elevate the institute's operational landscape. From efficient administration management to academic excellence and miscellaneous departmental tasks, FusionIIIT is a comprehensive solution that harmonizes the intricacies of campus life.

Picture FusionIIIT as a digital wizard that takes care of everything, from organizing administrative tasks to smoothing out academic processes. Its reach extends beyond the usual responsibilities, delving into various departments and sections to ensure the seamless functioning of every aspect of campus life.

On the administrative side, FusionIIIT efficiently handles complex paperwork and processes. In the realm of academics, it introduces a digital touch, simplifying learning and course management. However, its role doesn't end there; FusionIIIT acts as a friendly companion across different parts of the campus, ensuring the smooth operation of all aspects of campus life.

In essence, FusionIIIT transcends being a mere tool; it's a helpful friend, dedicated to making life at PDPM IIITDM Jabalpur more organized and enjoyable for everyone.

2. **About the module**

The Award and Scholarship Portal is designed to serve as a comprehensive platform for students at IIITDMJ. Through this portal, all students can access information regarding various convocation medals, awards, and scholarships. Eligible students have the opportunity to submit applications for these honors. The portal ensures that students receive timely notifications regarding application deadlines and the necessary procedures. This automated system aims to provide a streamlined and efficient alternative to the current manual application process.

3. **Scope of the module**
1) **Purpose**

This software is primarily intended for utilization by students affiliated with IIITDM Jabalpur. Its purpose is to furnish comprehensive details pertaining to a variety of scholarships and awards. Users are also provided with the functionality to submit applications and monitor the real-time status of their applications. The Awards and Scholarship Portal represents an innovative system designed to replace the existing manual and cumbersome processes associated with applying for diverse awards and scholarships.

**Flow :**

At IIITDM Jabalpur, the student body, staff, and faculty are integral components of the institution. One notable scholarship available is the Merit Cum Means (MCM) Scholarship. Additionally, various awards and prizes, such as the Chairman's Gold Medal, Director’s Gold Medals, D&M Proficiency Gold Medals, Academic Proficiency Medals, D&M Proficiency Prizes, Director’s Silver Medals, Notional Prizes, and Certificates of Merit, are offered.

Students meeting the specified criteria outlined in the SPACS manual can apply for the MCM scholarship and other available awards. The SPACS Assistant (Staff) is responsible for physically verifying the documents submitted by students and updating this information within the portal. Subsequently, the SPACS Convener (Faculty) reviews the submitted applications and bestows awards to eligible students. For detailed information regarding the list, eligibility criteria, and application procedures for various awards and scholarships, please refer to the following document: https://www.iiitdmj.ac.in/academics/download/SPACS-fellowships.pdf

2) **Actors & Functionality**



|**S. No.**|**Actor**|**Functionality**|
| - | - | - |
|**1.**|User|<p>- Browse through the catalog of available medals, scholarships, and other awards.</p><p>- View details of previous awardees</p><p>&emsp;- View details of SPACS members.</p>|
|**2.**|Student|<p>- Log into the system.</p><p>- Browse details and modalities regarding eligibility and application procedures.</p><p>- Apply for specific medals, scholarships, or awards.</p><p>- Track application status.</p><p>- Upload necessary documents.</p>|
|**3.**|SPACS Convener (Faculty)|<p>- Circulate notifications about awards.</p><p>- Introduce new awards and modify existing ones.</p><p>- Manage Medals/Awards/Scholarships catalog.</p><p>- Decide recipients of awards.</p>|
|**4.**|SPACS Assistant (Staff)|<p>- Physically verify documents.</p><p>- Update application status of students in the portal.</p><p>- Notify students about lack of required information in applications.</p>|
2. **User/Actor Description(characteristics)**
1. **User:**
- **Role:**
  - A person who has logged into the system.
- **Functionalities:**
  - Browse through the catalog of available medals, scholarships, and other awards.
  - View details of previous awardees.
- View details of SPACS members.
2. **Student:**
- **Role:**
  - A student of IIITDM Jabalpur who logs into the system.
- **Functionalities:**
  - Log into the system.
  - Browse details and modalities regarding eligibility and application procedures.
  - Apply for specific medals, scholarships, or awards.
  - Track application status.
  - Upload necessary documents while applying for scholarships/medals.
3. **SPACS Convener (Faculty):**
- **Role:**
  - Faculty member responsible for SPACS (Scholarship and Awards Committee).
- **Functionalities:**
  - Circulate notifications about awards.
  - Introduce new awards and modify existing ones.
  - Manage Medals/Awards/Scholarships catalog.
  - Act as the final authority to decide recipients of awards.
4. **SPACS Assistant (Staff):**
- **Role:**
  - Staff member assisting SPACS.
- **Functionalities:**
  - Physically verify documents submitted by students.
  - Update application status of students in the portal.
  - Notify students in case of lack of required information in their applications.
3. **Functional Requirements**
1. **Use case Diagram**

![](Aspose.Words.d4969777-0b4a-4882-82d2-543a8d3766c2.001.jpeg)

2. **Use case description**
1. **Use Case Description for a User as an actor to the system**

**Use case # 1**



|**UC ID**|UC#1||
| - | - | :- |
|**Use case Name**|**browse\_catalogue**||
|**Description**|User of the system can browse the available medals/scholarships categorically||
|**Actor**|Students, SPACS Convener, SPACS Assistant||
|**Precondition**|The user must be logged-in and the system is having the updated catalog of all the convocation medals, MCM scholarship and Other Prizes.||
|**Main Flow**|1|Actor logs into the system and opens Awards and Scholarship Page.|



<table><tr><th colspan="1" rowspan="2"></th><th colspan="2">2</th><th colspan="1">Actor selects the ‘Browse Award Catalog’ option.</th></tr>
<tr><td colspan="2">3</td><td colspan="1">Actor selects the required award/scholarship/ medals and views the necessary details.</td></tr>
<tr><td colspan="1"><b>Post conditions</b></td><td colspan="3" valign="top">The necessary details of the awards are displayed.</td></tr>
<tr><td colspan="1"><b>Alternate Flow</b></td><td colspan="3" valign="top">NIL</td></tr>
<tr><td colspan="1"><b>Sub Flow</b></td><td colspan="3">NIL</td></tr>
<tr><td colspan="1"><b>Global Alternate Flow</b></td><td colspan="1" valign="top">GA1</td><td colspan="2" valign="top">The actor can return to the dashboard at any time by clicking on the dashboard button.</td></tr>
<tr><td colspan="1"></td><td colspan="1"></td><td colspan="2"><b>Post Condition:</b> The system returns to the actor’s dashboard.</td></tr>
</table>

**Use case # 2**



<table><tr><th colspan="1"><b>UC ID</b></th><th colspan="2">UC#2</th></tr>
<tr><td colspan="1"><b>Use case Name</b></td><td colspan="2" valign="top"><b>view_staff_details</b></td></tr>
<tr><td colspan="1" valign="top"><b>Description</b></td><td colspan="2">Users of the system can view administration in charge of the system, and other related staff details. This is required so student may contact authority to ask query regarding any of medals/scholarship.</td></tr>
<tr><td colspan="1"><b>Actor</b></td><td colspan="2">Students, SPACS Convener, SPACS Assistant</td></tr>
<tr><td colspan="1" valign="top"><b>Precondition</b></td><td colspan="2">System must have information about administration/staff. The user must be logged in and The Awards and Scholarship page is opened.</td></tr>
<tr><td colspan="1" rowspan="2" valign="top"><b>Main Flow</b></td><td colspan="1" valign="top">1</td><td colspan="1">In the Awards and Scholarships page, the Actor selects the ‘SPACS member details’ option.</td></tr>
<tr><td colspan="1" valign="top">2</td><td colspan="1">Actor gets the list of SPACS Convener, SPACS Assistant and other members of SPACS involved in the system (if any).</td></tr>
<tr><td colspan="1"><b>Post conditions</b></td><td colspan="2" valign="top">All the necessary details of the staff involved in the system are displayed.</td></tr>
<tr><td colspan="1" valign="top"><b>Alternate Flow</b></td><td colspan="2" valign="top">NIL</td></tr>
<tr><td colspan="1"><b>Sub Flow</b></td><td colspan="2">NIL</td></tr>
<tr><td colspan="1" rowspan="2"><b>Global Alternate Flow</b></td><td colspan="1" rowspan="2" valign="top">GA1</td><td colspan="1" valign="top">The actor can return to the dashboard at any time by clicking on the dashboard button.</td></tr>
<tr><td colspan="1" valign="top"><b>Post Condition:</b> The system returns to the actor’s dashboard.</td></tr>
</table>

**Use case # 3**



<table><tr><th colspan="1"><b>UC ID</b></th><th colspan="2">UC#3</th></tr>
<tr><td colspan="1"><b>Use case Name</b></td><td colspan="2" valign="top"><b>view_previous_winners</b></td></tr>
<tr><td colspan="1"><b>Description</b></td><td colspan="2">Users can view previous year’s winners for various convocation medals and MCM Scholarships.</td></tr>
<tr><td colspan="1"><b>Actor</b></td><td colspan="2">Students, SPACS Convener, SPACS Assistant</td></tr>
<tr><td colspan="1" valign="top"><b>Precondition</b></td><td colspan="2" valign="top">System must have information about winners of medals/scholarships/awards and actor must be logged into the system and the Awards and Scholarship page is opened.</td></tr>
<tr><td colspan="1" rowspan="3" valign="top"><b>Main Flow</b></td><td colspan="1">1</td><td colspan="1">Actor selects the ‘Previous Award Winners’ option.</td></tr>
<tr><td colspan="1">2</td><td colspan="1">Actor then selects respective batch and award from the dropdown list provided</td></tr>
<tr><td colspan="1">3</td><td colspan="1">He clicks the ‘Submit’ button.</td></tr>
<tr><td colspan="1"><b>Post conditions</b></td><td colspan="2" valign="top">List of winners for the selected option are displayed in chronological order.</td></tr>
</table>



<table><tr><th colspan="1"><b>Alternate Flow</b></th><th colspan="2" valign="top">NIL</th></tr>
<tr><td colspan="1"><b>Sub Flow</b></td><td colspan="2">NIL</td></tr>
<tr><td colspan="1" rowspan="2"><b>Global Alternate Flow</b></td><td colspan="1" rowspan="2" valign="top">GA1</td><td colspan="1" valign="top">The actor can return to the dashboard at any time by clicking on the dashboard button.</td></tr>
<tr><td colspan="1" valign="top"><b>Post Condition:</b> The system returns to the actor’s dashboard.</td></tr>
</table>

2. **Use Case Description for a Student (extending User) as an actor to the system**

**Use case # 4**



<table><tr><th colspan="1"><b>UC ID</b></th><th colspan="2">UC#4</th></tr>
<tr><td colspan="1" valign="top"><b>Use case Name</b></td><td colspan="2" valign="top"><b>apply_for_convocation_medals</b></td></tr>
<tr><td colspan="1" valign="top"><b>Description</b></td><td colspan="2" valign="top"><p>The student can apply for Convocation Medals by filling out a form and uploading necessary documents.</p><p><i>Guidelines:</i> https://www.iiitdmj.ac.in/academics/download/SPACS-fellowships.pdf</p></td></tr>
<tr><td colspan="1"><b>Actor</b></td><td colspan="2">Student</td></tr>
<tr><td colspan="1" valign="top"><b>Precondition</b></td><td colspan="2">Student Logged in, opens Awards and Scholarship portal and applications are invited for the same.</td></tr>
<tr><td colspan="1" rowspan="5" valign="top"><b>Main Flow</b></td><td colspan="1">1</td><td colspan="1">Students click on the ‘Apply for Awards’ option and then Convocation Medals.</td></tr>
<tr><td colspan="1" valign="top">2</td><td colspan="1">Student reads the instructions for applying for the Convocation Medals and clicks on ‘Proceed’ button.</td></tr>
<tr><td colspan="1" valign="top">2</td><td colspan="1">Student selects the type of application from the available options and the respective form is displayed.</td></tr>
<tr><td colspan="1">3</td><td colspan="1">Student fills up all the necessary details in the form.[S1]</td></tr>
<tr><td colspan="1">4</td><td colspan="1">After successful uploading, students click on the ‘Submit’ button.</td></tr>
<tr><td colspan="1"><b>Post conditions</b></td><td colspan="2" valign="top">Application and documents submitted for verification.</td></tr>
<tr><td colspan="1" rowspan="2" valign="top"><b>Sub Flow</b></td><td colspan="1">S1</td><td colspan="1">He can upload supporting documents.</td></tr>
<tr><td colspan="1"></td><td colspan="1"><b>Post-condition</b> - Documents are attached along with the form.</td></tr>
<tr><td colspan="1" valign="top"><b>Alternate Flow</b></td><td colspan="1"></td><td colspan="1" valign="top">NIL</td></tr>
<tr><td colspan="1" rowspan="2"><b>Global Alternate Flow</b></td><td colspan="1" rowspan="2" valign="top">GA1</td><td colspan="1" valign="top">The actor can return to the dashboard at any time by clicking on the dashboard button.</td></tr>
<tr><td colspan="1" valign="top"><b>Post Condition:</b> The system returns to the actor’s dashboard.</td></tr>
</table>

**Use case # 5**



|**UC ID**|UC#5|
| - | - |
|**Use case Name**|**apply\_for\_mcm\_scholarship**|
|**Description**|<p>The student can apply for MCM scholarship by filling out a form and uploading necessary documents.</p><p>*Guidelines:* https://www.iiitdmj.ac.in/academics/download/SPACS-fellowships.pdf"</p>|
|**Actor**|Student|
|**Precondition**|Student Logged in, opens Scholarship and Awards portal and applications are invited for the same|



<table><tr><th colspan="1" rowspan="4" valign="top"><b>Main Flow</b></th><th colspan="1">1</th><th colspan="1">Students click on the ‘Apply for Awards’ option and select MCM Scholarship.</th></tr>
<tr><td colspan="1">2</td><td colspan="1">MCM Scholarship form is displayed.</td></tr>
<tr><td colspan="1">3</td><td colspan="1">Student fills up the necessary details in the form[S1]</td></tr>
<tr><td colspan="1">4</td><td colspan="1">After successful uploading, students click on the ‘Submit Application’ button.</td></tr>
<tr><td colspan="1" valign="top"><b>Post conditions</b></td><td colspan="2" valign="top">Application and documents submitted for verification.</td></tr>
<tr><td colspan="1" rowspan="2" valign="top"><b>Sub Flow</b></td><td colspan="1" valign="top">S1</td><td colspan="1" valign="top">He can upload supporting documents like income certificate and all the required documents (Refer to appendix A for MCM scholarship details).</td></tr>
<tr><td colspan="1"></td><td colspan="1"><b>Post-condition</b> - Documents are attached along with the form.</td></tr>
<tr><td colspan="1" valign="top"><b>Alternate Flow</b></td><td colspan="1"></td><td colspan="1" valign="top">NIL</td></tr>
<tr><td colspan="1" rowspan="2"><b>Global Alternate Flow</b></td><td colspan="1" rowspan="2" valign="top">GA1</td><td colspan="1" valign="top">The actor can return to the dashboard at any time by clicking on the dashboard button.</td></tr>
<tr><td colspan="1" valign="top"><b>Post Condition:</b> The system returns to the actor’s dashboard.</td></tr>
</table>

**Use case # 6**



<table><tr><th colspan="1"><b>UC ID</b></th><th colspan="2">UC#6</th></tr>
<tr><td colspan="1"><b>Use case Name</b></td><td colspan="2" valign="top"><b>track_application_status</b></td></tr>
<tr><td colspan="1"><b>Description</b></td><td colspan="2">Students view application status for each of the applied medals/scholarships.</td></tr>
<tr><td colspan="1"><b>Actor</b></td><td colspan="2">Student</td></tr>
<tr><td colspan="1" valign="top"><b>Precondition</b></td><td colspan="2" valign="top">Student must have applied for an award/scholarship and have a valid application number assigned</td></tr>
<tr><td colspan="1" rowspan="4" valign="top"><b>Main Flow</b></td><td colspan="1">1</td><td colspan="1">Students click on the ‘View Application Status’ option.</td></tr>
<tr><td colspan="1">2</td><td colspan="1">Student selects the ‘Current’ option.</td></tr>
<tr><td colspan="1">3</td><td colspan="1">All the applications status is displayed here along with the application ID.</td></tr>
<tr><td colspan="1" valign="top">4</td><td colspan="1">Student can also selects the ‘History’ option to view the status of the past applied applications.</td></tr>
<tr><td colspan="1"><b>Post conditions</b></td><td colspan="2" valign="top">The status of all applications submitted by the student in the past are displayed.</td></tr>
<tr><td colspan="1" valign="top"><b>Alternate Flow</b></td><td colspan="2" valign="top">NIL</td></tr>
<tr><td colspan="1"><b>Sub Flow</b></td><td colspan="2">NIL</td></tr>
<tr><td colspan="1" rowspan="2" valign="top"><b>Global Alternate Flow</b></td><td colspan="1" rowspan="2" valign="top">GA1</td><td colspan="1" valign="top">The actor can return to the dashboard at any time by clicking on the dashboard button.</td></tr>
<tr><td colspan="1" valign="top"><b>Post Condition:</b> The system returns to the actor’s dashboard.</td></tr>
</table>

3. **Use Case Description for SPACS convener(extending user) as an actor to the system**

**Use case # 7**



|**UC ID**|UC#7|
| - | - |
|**Use case Name**|**process\_verified\_applications**|
|**Description**|<p>The actor is able to browse the awards/scholarships applications. While browsing he also gets a facility to sort them according to CPI, Income etc.</p><p>This feature provides in depth statistics about the applicants.</p>|
|**Actor**|SPACS Convener|



<table><tr><th colspan="1" valign="top"><b>Precondition</b></th><th colspan="2">Actor logs into the system, opens ‘Awards and Scholarships’ portal and the output of ‘process_submitted_applications’</th></tr>
<tr><td colspan="1" rowspan="5" valign="top"><b>Main Flow</b></td><td colspan="1">1</td><td colspan="1">Click on ‘Browse Applications’</td></tr>
<tr><td colspan="1">2</td><td colspan="1">Select an award/scholarship</td></tr>
<tr><td colspan="1" valign="top">3</td><td colspan="1">All the verified applications for the above selected option are displayed and can be sorted according to various factors as displayed in description.</td></tr>
<tr><td colspan="1" valign="top">4</td><td colspan="1" valign="top">Actor selects one of the applications and checks that application.</td></tr>
<tr><td colspan="1" valign="top">5</td><td colspan="1" valign="top">Actor checks the hardcopies of submitted files (if required), then he updates the status of the application to the APPROVED. [A1]</td></tr>
<tr><td colspan="1" valign="top"><b>Post conditions</b></td><td colspan="2" valign="top">Actor grants the application and the respective student is regarding the same.</td></tr>
<tr><td colspan="1" rowspan="2" valign="top"><b>Alternate Flow</b></td><td colspan="1" valign="top">A1</td><td colspan="1">If an actor finds any false information he REJECTS the application by clicking the REJECT button corresponding to that application.</td></tr>
<tr><td colspan="1"></td><td colspan="1"><b>Post Condition</b>: The corresponding application gets rejected and the applicant (student) is informed regarding the same.</td></tr>
<tr><td colspan="1"><b>Sub Flow</b></td><td colspan="2">NIL</td></tr>
<tr><td colspan="1" rowspan="2"><b>Global Alternate Flow</b></td><td colspan="1" rowspan="2" valign="top">GA1</td><td colspan="1" valign="top">The actor can return to the dashboard at any time by clicking on the dashboard button.</td></tr>
<tr><td colspan="1" valign="top"><b>Post Condition:</b> The system returns to the actor’s dashboard.</td></tr>
</table>

**Use case # 8**



|**UC ID**|UC#8|
| - | - |
|**Use case Name**|**manage\_catalogue**|
|**Description**|The actor can make changes to the application procedure and also scrap the existing awards/prizes/scholarship.|



<table><tr><th colspan="1"><b>Actor</b></th><th colspan="2">SPACS Convener</th></tr>
<tr><td colspan="1"><b>Precondition</b></td><td colspan="2">Logs into the system, opens awards/scholarships portal</td></tr>
<tr><td colspan="1" rowspan="3" valign="top"><b>Main Flow</b></td><td colspan="1" valign="top">1</td><td colspan="1">Select ‘Manage Catalog’ option on the screen and list of awards and scholarships are displayed.</td></tr>
<tr><td colspan="1" valign="top">2</td><td colspan="1">If an award/medal has to be modified/deleted then click on ‘edit button’ next to the award/medal</td></tr>
<tr><td colspan="1">3</td><td colspan="1">Make the necessary changes and click on the ‘Save changes’ button.</td></tr>
<tr><td colspan="1" valign="top"><b>Post conditions</b></td><td colspan="2" valign="top">The award/scholarship database is updated accordingly, and the SPACS manual needs to be updated as a result.</td></tr>
<tr><td colspan="1" valign="top"><b>Alternate Flow</b></td><td colspan="2" valign="top">NIL</td></tr>
<tr><td colspan="1"><b>Sub Flow</b></td><td colspan="2">NIL</td></tr>
<tr><td colspan="1" rowspan="2" valign="top"><b>Global Alternate Flow</b></td><td colspan="1" rowspan="2" valign="top">GA1</td><td colspan="1" valign="top">The actor can return to the dashboard at any time by clicking on the dashboard button.</td></tr>
<tr><td colspan="1" valign="top"><b>Post Condition:</b> The system returns to the actor’s dashboard.</td></tr>
</table>

**Use case # 9**



<table><tr><th colspan="1"><b>UC ID</b></th><th colspan="2">UC#9</th></tr>
<tr><td colspan="1"><b>Use case Name</b></td><td colspan="2" valign="top"><b>invite_applications</b></td></tr>
<tr><td colspan="1" valign="top"><b>Description</b></td><td colspan="2">He can invite the applications for the MCM scholarship or awards (if necessary) for all the students who satisfy the criteria as mentioned in SPACS manual.</td></tr>
<tr><td colspan="1"><b>Actor</b></td><td colspan="2">SPACS Convener</td></tr>
<tr><td colspan="1"><b>Precondition</b></td><td colspan="2">Logs into the system</td></tr>
<tr><td colspan="1" rowspan="4" valign="top"><b>Main Flow</b></td><td colspan="1" valign="top">1</td><td colspan="1">Select ‘Invite applications’ option and the list of awards or scholarship is displayed for selection</td></tr>
<tr><td colspan="1">2</td><td colspan="1">Selects one award or MCM scholarship and click NEXT.</td></tr>
<tr><td colspan="1" valign="top">3</td><td colspan="1">He has to select the Year of Students to which he wants to invite the MCM applications or awards and click NEXT.</td></tr>
<tr><td colspan="1" valign="top">4</td><td colspan="1" valign="top">After successful completion, Clicks INVITE button.</td></tr>
<tr><td colspan="1" valign="top"><b>Post conditions</b></td><td colspan="2" valign="top">The notification is pushed to all the recipients on their homepage upon logging in.</td></tr>
<tr><td colspan="1" valign="top"><b>Alternate Flow</b></td><td colspan="2" valign="top">NIL</td></tr>
<tr><td colspan="1"><b>Sub Flow</b></td><td colspan="2">NIL</td></tr>
<tr><td colspan="1" rowspan="2" valign="top"><b>Global Alternate Flow</b></td><td colspan="1" rowspan="2" valign="top">GA1</td><td colspan="1" valign="top">The actor can return to the dashboard at any time by clicking on the dashboard button.</td></tr>
<tr><td colspan="1" valign="top"><b>Post Condition:</b> The system returns to the actor’s dashboard.</td></tr>
</table>

4. **Use Case Description for SPACS assistant (extends user) as an actor to the system**

**Use case # 10**



|**UC ID**|UC#10|
| - | - |



<table><tr><th colspan="1"><b>Use case Name</b></th><th colspan="2" valign="top"><b>process_submitted_applications</b></th></tr>
<tr><td colspan="1" valign="top"><b>Description</b></td><td colspan="2"><p>The actor is able to browse the awards/scholarships applications. While browsing he also gets a facility to sort them according to CPI, Income etc.</p><p>This feature provides in -depth statistics about the applicants.</p></td></tr>
<tr><td colspan="1"><b>Actor</b></td><td colspan="2">SPACS Assistant</td></tr>
<tr><td colspan="1"><b>Precondition</b></td><td colspan="2">Actor logs into the system, opens ‘Awards and Scholarships’ portal</td></tr>
<tr><td colspan="1" rowspan="5" valign="top"><b>Main Flow</b></td><td colspan="1">1</td><td colspan="1">Click on ‘Browse applications’</td></tr>
<tr><td colspan="1">2</td><td colspan="1">Select an award/scholarship</td></tr>
<tr><td colspan="1">3</td><td colspan="1">All the Submitted applications for the above selected option are displayed</td></tr>
<tr><td colspan="1" valign="top">4</td><td colspan="1" valign="top">Actor selects one of the applications and checks that application.</td></tr>
<tr><td colspan="1" valign="top">5</td><td colspan="1" valign="top">Actor checks the hardcopies of submitted files (if required), then he updates the status of the application to the VERIFIED. [A1]</td></tr>
<tr><td colspan="1" valign="top"><b>Post conditions</b></td><td colspan="2" valign="top">Actor verifies the application and the respective student is notified regarding the same.</td></tr>
<tr><td colspan="1" rowspan="2" valign="top"><b>Alternate Flow</b></td><td colspan="1" valign="top">A1</td><td colspan="1" valign="top">If an actor finds any false information he REJECTS the application by clicking the REJECT button corresponding to that application.</td></tr>
<tr><td colspan="1"></td><td colspan="1" valign="top"><b>Post Condition</b>: The corresponding application gets rejected and the applicant (student) is notified regarding the same.</td></tr>
<tr><td colspan="1"><b>Sub Flow</b></td><td colspan="2">NIL</td></tr>
<tr><td colspan="1" rowspan="2"><b>Global Alternate Flow</b></td><td colspan="1" rowspan="2" valign="top">GA1</td><td colspan="1" valign="top">The actor can return to the dashboard at any time by clicking on the dashboard button.</td></tr>
<tr><td colspan="1" valign="top"><b>Post Condition:</b> The system returns to the actor’s dashboard.</td></tr>
</table>

3. **Other Functional Requirements (Suggestions)**



<table><tr><th colspan="1" valign="top"><b>UC ID</b></th><th colspan="1" valign="top">UC#11</th></tr>
<tr><td colspan="1" valign="top"><b>Use case Name</b></td><td colspan="1" valign="top">Withdraw Application</td></tr>
<tr><td colspan="1" valign="top"><b>Description</b></td><td colspan="1" valign="top">The actor is able to withdraw his/her application if any other private or government scholarship scheme is awarded to them within the stipulated duration.</td></tr>
<tr><td colspan="1"><b>Actor</b></td><td colspan="1">Student</td></tr>
<tr><td colspan="1"><b>Precondition</b></td><td colspan="1">Actor logs into the system, opens ‘Awards and Scholarships’ portal</td></tr>
<tr><td colspan="1" rowspan="4" valign="top"><b>Main Flow</b></td><td colspan="1">Click on ‘Withdraw applications’</td></tr>
<tr><td colspan="1">Select an award/scholarship to be withdrawn</td></tr>
<tr><td colspan="1">All the Submitted applications for the above selected option are displayed</td></tr>
<tr><td colspan="1" valign="top">Actor selects one of the applications and clicks on the withdraw button.</td></tr>
<tr><td colspan="1" valign="top"><b>Post conditions</b></td><td colspan="1" valign="top">The application’s withdrawn and the respective student is notified regarding the same.</td></tr>
<tr><td colspan="1" valign="top"><b>Alternate Flow</b></td><td colspan="1" valign="top">NIL</td></tr>
<tr><td colspan="1"><b>Sub Flow</b></td><td colspan="1">NIL</td></tr>
<tr><td colspan="1" rowspan="2" valign="top"><b>Global Alternate Flow</b></td><td colspan="1" valign="top">The actor can return to the dashboard at any time by clicking on the dashboard button.</td></tr>
<tr><td colspan="1" valign="top"><b>Post Condition:</b> The system returns to the actor’s dashboard.</td></tr>
</table>

4. **Non-Functional Requirements**
1. **PERFORMANCE REQUIREMENTS:**
- The product shall be based on the web and has to be run from a web server.
- The product shall take initial load time depending on internet connection strength which also depends on the media from which the product is run.
- The performance shall very loosely depend upon hardware components of the user given a web-browser minimum-requirements are met.
- A lot of data has to be queried from the database which may lead to decrease in response time of the pages to load if too many users request the services from the system.
2. **Security Requirements:**
- The profile of a student must not be accessible to other students.
- The documents uploaded by the students should not be shared to any third party and should be kept stored on the database only till the duration validation and approval.
3. **Accessibility:**
- The system shall provide a uniform look and feel between all the system and web pages.
- The portal should be up and running 24 hours a day. Client side of the system can

  be accessed from any device capable of running a fully-functional web-browser.

- To use complete system features the user must login with the id provided.
4. **Business Rules:**
- Applications are invited only for a specific period of time .i.e as mentioned in the notification.
- No student is allowed to fill the other student’s application forms.
- For more details, please refer to the IIITDM SPACE-fellowships manual.
5. **List of open issues with the module**



|S. No|Issue details|Category|How can it be resolved?|Any other relevant information|
| :- | - | - | :- | :- |
|1|Problem regarding convocation medal invitation|Implementation of functionality|Implement respective functionality of medals for all batches|NA|
|2|Incomplete Notifications|Notification related|Add the notification feature|NA|
|3|UI/UX|UI|Good UI for filling the form|NA|
|4|Number of Form filling at a time|Unimplemente d functionality|Check whether form is filled before or not|Only one form we have to submit in a given deadline|
|5|Sorting and other features|Unimplemente d functionality|Implement sorting on basis of cpi and other filters|NA|

6. **Suggestions:**

In the present system we are filling the various fields like correspondence address, financial assistance etc. again and again in different convocation medals forms. This can be removed and those fields can be filled only once and can be retrieved from the previously entered data.

In MCM form, there is some information like 10th school fee, 10th school name, 12th school name, 12th fee etc. remains the same for the entire 4 years of our stay in IIITDM Jabalpur. It would be better if we store that information once after filling and from the next application we do not need to fill those details.

The approval process of MCM for the verified MCM applications can be automated.

**Appendix A: Merit Cum Means (MCM) Scholarship Form**

**Indian Institute of Information Technology, Design and Manufacturing, Jabalpur**

**Application form for Merit Cum Means Scholarship**

1. Name of the Applicant: Capital Letter
1. Category (SC/ST/OBC/GEN)
1. State:
1. (i) Institute Roll No.

   2) Hall and Room No.
   2) Allahabad Bank Account No.
1. E Mail ID Address and Mobile No.
1. a. Name of

Father b Name of

Mother

3. Name of present Guardian

   (His relationship with the student if parents are not alive)

4. Name of brother (s) and their occupation
4. Name of sister (s) and their occupation
7. Present Postal address of father/ guardian
1. Fathers Gross Annual Income
1. Mothers gross annual income (if applicable)
1. Annual Income from other source

   (i.e Investment in Bank/ post office/ UTI/ LIC/ Shares/ Debenture/ Landed Property/ Income in the name of the students etc, if any)

8. Total of 7 (1) + (2) + (3) above ………………………………………. Rs. …......
9. Fathers/ Guardians Occupational Status (tick as applicable)

1\. In service (Government/ Private/ Public)

(Supported by IT form 16/ Saral Form whose annual income is above Rs. 50000/-)

2) Other than Salaried/ Pensioner

(supported by Annual Income Certificate to be issued by SDO/BDO/MRO/Tahasilder/Local Municipal Corporation/ Gram Panchayat, etc)

If business/ Medical/ Legal Practitioner/ Consultant etc

1. Name and Address of Firm/ Organization/ Shop
1. Nature of Business/ Trade
1. Trade/ Professional License / Registration No. (Copy to be enclosed)
1. Sales Tax/ Commercial Tax Registration No/ Zone
3) Pensioners/ Family Pensioners

(Supported by Non Employment certificate to be issued by SDO/BDO/MRO/ Tahsilder/ Local Municipal Corporation Gram Panchayat etc

10. Mothers Occupation

    (With address of Employer, if employed)

11. Declaration

I declare the followings:

1. No disciplinary action has been taken against me by the Institute in the preceding academic year 2016-17.
1. I am not in receipt of any other scholarship/stipend/ financial assistance, etc. from any other sources.

Encl:

Signature of father/ Guardian Signature of Student

Questionnaire to be filled by students applying for MCM (Merit Cum means) scholarship

Name:- Roll No. Sign:-

1. Please write in detail about Father’s Occupation/Profession:-
   1. Government Service/Private Service/Business
   1. Describe the post and work if in service OR Describe the Business:-
1. Please write in detail about Mother’s Occupation/Profession:-
1. No. of Four wheeler (Giver description regarding make and year):-
1. No of Two wheeler (Giver description regarding make and year):-
1. House :
1. Rented/ Owned
1. Plot area and constructed

Area. 6.High School (10th Standard)

1. Name of School
1. Fees per

month:- 7.Inter (12th Standard)

1. Name of School:-
1. Fees per month:-

8\.Amount of Educational Bank Loan along with name of Bank:

**Part II**

**(Declaration by the father/ guardian of the student)**

I declare that my Annual Family Income from other sources during the financial year ……………… was as under:

1\. Landed Properties (Certificate from Tahsilder/ Gram Panchayet): 2.Agriculture: 3.Investment in Bank/ Post Office/Unit Trust:

4. Shares Certificates/ debenture:
4. Other Sources:

Total

Further I declare that the information given above is true. I understand that the Merit cum Means Scholarship/ free ship if awarded to my son/ daughter is liable to be withheld or discontinued at the discretion of the authorities of the PDPM-IIITDM Jabalpur, with out assigning any reason. If subsequently (after award of MCM scholarship to my ward) it is found that he/ she has been granted any other scholarship/ stipend/ financial assistance etc. by any Govt/ Non Government organization for the period, I shall be bound to refund the whole amount of scholarship/ free ship/ stipend and financial assistance etc to the scholarship awarding authority immediately. I shall also be personally held responsible for the refund of the scholarship/ free ship amount (paid to my son/ daughter by Institute) **and willing to be prosecuted as per law** in the event of any information in this declaration and also in the enclosed scholarship application form, being proved incorrect later on.

Date

Signature of the father/ guardian: Full Name:

Address with pin code:

Phone/ mobile number if any

**Form A**

Annual income Certificate for those Parents/ Guardians who are in service (Govt or Private)

**Income from Salary**

Name and Address of the Employer

Certified that is employed in this organization in the capacity of (Designation…………………………………) Post held by the Employee………………………….., and that the break up of his/ her gross annual income from salary received in the financial year is as follows:

**Item**

Basic Salary if consolidated/ pay Band:

Grade Pay:

DA/ADA/ Relief:

Special Pay and Honorarium, Bonus etc if any: Other Allowances if any:

Employer Signature with seal

**Total Amount for 12 months**

Designation Date

**N.B:** All the entries as stated in column 2 above must be supported by attested copy of IT **Form 16/ SARAL** form for the corresponding year.

Guardians whose annual gross income is below Rs. 50,000/- need not submit IT return. They have to submit a certificate from Employer/ Salary disbursing officer stating that their annual income is not taxable and they need not produce **IT Form 16**.

**Form – B**

**Format of Income Affidavit**

(For use of those parents/ guardians who are not in employment anywhere and derives income from sources other than salary / pension)

(To be submitted on Non Judicial stamp paper of Rs. 20/- and sworn in before a first class Magistrate/ Notary public)

I, Shri/ Smt. ……………………………………………….a resident of ………………………….. Solemnly declare that:

1. My son/ daughter, Shri/ Miss ……………………………………………. Is currently studying at the PDPM Indian Institute of Information Technology, Design and Manufacturing Jabalpur, in 4-year B Tech programme in Engineering.
1. He/ She is an applicant for the award of Merit Cum Means Scholarship for the Academic year

   ………………………………………

3. I, declare that my spouse is employed/ not employed of my family in the financial year ………………………………….. i.e during the period from 1st April……….. to March 31 was as mentioned hereunder (supported by document):

(A) From my own professional as indicated: Rs pa

i) Income from Business/Medical Practice Legal Practice Rs pa

Engineering Consultancy etc

ii)Income from Agriculture Rs pa iii) Income from Landed Properties Rs. ………….........pa iv) Income from Investment in Bank/ Post office etc Rs pa

v) Income from Share Certificates/ Debentures Rs pa vi) Income

from any other sources (i.e. Retirement Rs. ………….........pa Benefits for VRS/ VSS etc if any

(B)Income of my wife (if any) pa

(if employed, salary certificate from employer to be enclosed) Rs pa © Income in the name of my son/ ward (if any) Rs pa

Total Income (A + B + C) Rs pa

Further, I declare that the information given above is true. I understand that the Merit Cum Means scholarship if awarded to my son/ daughter is liable to be withheld or discontinued at the discretion of the authorities of the PDPM Indian Institute of Information Technology, Design and Manufacturing Jabalpur, without assigning any reason. If subsequently (after award of MCM Scholarship to my ward) it is found that he/ she has been granted any other has been granted any other scholarship/ stipend/ Financial assistance etc by any Government / Non Government organization for the same period, I shall be bound to refund the whole amount of scholarship/ free ship/ stipend/ Financial Assistance etc to the scholarship awarding authority immediately. I shall also be personally held responsible for the refund of the scholarship/ free ship amount (paid to my son/ daughter by the Institute) **and willing to be prosecuted as per law** in the event of any information in this declaration and also in the enclosed scholarship application form, being proved incorrect later on.

(Signature of father/ guardian)

Sworn before me this ……………….. Day of ………………..2017 and signed

(Seal)

(Signature of first class Magistrate/ Notary public)

**Form C**

**(For pensioner/ family pensioner only)**

(Income/ salary certificate for those parents/ guardians who are in pensioners or retired from service or their wives are getting family pension**)**

Income from Pension/ Family pension: Rs. ………………………..

1. Name and Address of the Ex Employer with PPO Number:
1. Certified that ……………………………… was employed in this organization/ superannuated from , in the capacity of (post held by retired employee) and that the break up of his/ her annual income from Pension/ family pension received in the financial year is as follows:

**Item Total amount for 12 months**

1) Basic pension/ family pension Rs.
1) Dearness Relief: Rs.
1) Other allowances, if any Rs.

Signature of ex employer Pension disbursing officer Designation

Date

*(Official Seal)*
