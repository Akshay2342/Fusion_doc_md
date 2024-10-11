Fusion ERP 

Software Requirements Specifications                          For 

`     `AC-5 Awards and Scholarships  

Team Members: 

Abhishek Muwal(21BCS005) Ajay Sharma(21BCS014) Aryan(21BCS036) 

Deepak Meena (21BCS071) Sukram(21BCS212) 

Student Mentor: Soham Bakul Sarode 

***Faculty Mentor: Dr. Ayan Seal*** 

- 1.Introduction 
1. Introduction about the Fusion-A breif Description 

`     `FusionIIIT at PDPM Indian Institute of Information Technology, Design and Manufacturing, Jabalpur, is a comprehensive initiative developed by students to streamline and automate various functions across the campus. This digital platform, built with precision using Python 3.8 and Django Web framework, serves as a testament to seamless integration within the institute. 

The scope of FusionIIIT extends beyond administrative tasks, encompassing academic management and other departmental responsibilities. It acts as a digital wizard, addressing the intricacies of campus life and ensuring a harmonized operational landscape. 

On the administrative front, FusionIIIT takes care of complex paperwork and processes, simplifying tasks that would otherwise be time-consuming. In academics, it introduces a digital touch to enhance the learning experience and streamline course management. However, its impact is not limited to these areas, as FusionIIIT extends its support to various departments and sections, ensuring the smooth functioning of every aspect of campus life. 

In essence, FusionIIIT is described as more than just a tool; it is portrayed as a friendly companion that contributes to the organization and enjoyment of life at PDPM IIITDM Jabalpur for everyone involved. By handling diverse responsibilities and providing support across different domains, FusionIIIT aims to make the overall campus experience more organized and enjoyable. 

2. Purpose of the Module 

   The primary goal of this module is to establish a centralized platform for all students at IIITDMJ to access information about convocation medals, awards, and scholarships. Additionally, eligible students should be able to apply for these honors through the portal. The system aims to streamline the application process, providing automation and reducing the challenges associated with the current manual application procedures. 

3. Scope of the Module 

   This software will be mostly used by the students of IIITDM Jabalpur to get all the necessary details 

   about various scholarships and awards. They also get the feature to apply for the same and track 

   the application status. 

- 2.User/Actor Characteristics 
1. User: 

`           `A user is the person who have logged in the system.  

**Role:** Browse through catalogue of awards and scholarships          ***Specific Functionalities:*** 

- Browse available medals and scholarships 
- Browse previous winners of medals and scholarships 
- View the details of SPACS members 
2. Student: 

`        `A student is main user who will use this portal to apply for various scholarships and awards. 

**Role:** Browse through catalogue and fill forms for the available awards and scholarships. ***Specific Functionalities:*** 

- Submit applications through the ERP portal 
- Fill the form and upload required documents 
- Receives notifications about the application approval/rejection 
- Can track the application status and also see the application history 
3. SPACS CONVENER: 

`    `He is responsible for circulating notifications about the awards and also decides the recipients. 

**Role:** Invite applications and decides the winners of awards and scholarships ***Specific Functionalities:*** 

- Invite applications for awards and scholarships 
- Circulate information regarding new applications 
- Can introduce new awards and modify the existing ones 
- Finally decides who will be awarded for the medals and scholarships 
4. SPACS ASSISTANT: 

He is the person who will be responsible for physical verification of documents. **Role:** Physically verifies the documents and notify to students  

***Specific Functionalities:*** 

- Will verify the application documents physically 
- Update the application status of students in the portal 
- Notify the students in case of lack of required document 
- 3. Funtional Requirements 
1. Use Case Diagram: 

![](Aspose.Words.c154b3e5-6f3c-4428-91d6-bcdb87880290.001.jpeg)

2. Use Case Description 
1. **Use Case Description for a User as an actor to the system** 

**Use case # 1** 



|**UC ID** |UC#1 ||
| - | - | :- |
|**Use case Name** |**browse\_catalogue** ||
|**Description** |User of the system can browse the available medals/scholarships categorically ||
|**Actor** |Students, SPACS Convener, SPACS Assistant ||
|**Precondition** |The user must be logged-in and the system is having the updated catalogue of all the convocation medals, MCM scholarship and Other Prizes. ||
|**Main Flow** |1 |Actor logs into the system and opens Awards and Scholarship Page. |



<table><tr><th colspan="1" rowspan="2"></th><th colspan="2" valign="top">2 </th><th colspan="1" valign="top">Actor selects the ‘Browse Award Catalogue’ option. </th></tr>
<tr><td colspan="2" valign="top">3 </td><td colspan="1" valign="top">Actor selects the required award/scholarship/ medals and views the necessary details. </td></tr>
<tr><td colspan="1"><b>Post conditions</b> </td><td colspan="3" valign="top">The necessary details of the awards are displayed. </td></tr>
<tr><td colspan="1"><b>Alternate Flow</b> </td><td colspan="3" valign="top">NIL </td></tr>
<tr><td colspan="1" valign="top"><b>Sub Flow</b> </td><td colspan="3" valign="top">NIL </td></tr>
<tr><td colspan="1"><b>Global Alternate Flow</b> </td><td colspan="1" valign="top">GA1 </td><td colspan="2" valign="top">The actor can return to the dashboard at any time by clicking on dashboard button. </td></tr>
<tr><td colspan="1"></td><td colspan="1"></td><td colspan="2" valign="top"><b>Post Condition:</b> The system returns to the actor’s dashboard. </td></tr>
</table>

**Use case # 2** 



<table><tr><th colspan="1" valign="top"><b>UC ID</b> </th><th colspan="2" valign="top">UC#2 </th></tr>
<tr><td colspan="1"><b>Use case Name</b> </td><td colspan="2" valign="top"><b>view_staff_details</b> </td></tr>
<tr><td colspan="1" valign="top"><b>Description</b> </td><td colspan="2">User of the system can view administration in charge of the system, and other related staff details. This is required so student may contact authority to ask query regarding any of medals/scholarship. </td></tr>
<tr><td colspan="1" valign="top"><b>Actor</b> </td><td colspan="2" valign="top">Students, SPACS Convener, SPACS Assistant </td></tr>
<tr><td colspan="1" valign="top"><b>Precondition</b> </td><td colspan="2">System must have information about administration/staff. The user must be logged in and Awards and Scholarship page is opened. </td></tr>
<tr><td colspan="1" rowspan="2" valign="top"><b>Main Flow</b> </td><td colspan="1" valign="top">1 </td><td colspan="1" valign="top">In Awards and Scholarships page, Actor selects the ‘SPACS member details’ option. </td></tr>
<tr><td colspan="1" valign="top">2 </td><td colspan="1">Actor gets the list of SPACS Convener, SPACS Assistant and other members of SPACS involved in the system (if any). </td></tr>
<tr><td colspan="1"><b>Post conditions</b> </td><td colspan="2" valign="top">All the necessary details of the staff involved in the system are displayed. </td></tr>
<tr><td colspan="1"><b>Alternate Flow</b> </td><td colspan="2" valign="top">NIL </td></tr>
<tr><td colspan="1" valign="top"><b>Sub Flow</b> </td><td colspan="2" valign="top">NIL </td></tr>
<tr><td colspan="1" rowspan="2"><b>Global Alternate Flow</b> </td><td colspan="1" rowspan="2" valign="top">GA1 </td><td colspan="1" valign="top">The actor can return to the dashboard at any time by clicking on dashboard button. </td></tr>
<tr><td colspan="1" valign="top"><b>Post Condition:</b> The system returns to the actor’s dashboard. </td></tr>
</table>

**Use case # 3** 



<table><tr><th colspan="1" valign="top"><b>UC ID</b> </th><th colspan="2" valign="top">UC#3 </th></tr>
<tr><td colspan="1"><b>Use case Name</b> </td><td colspan="2" valign="top"><b>view_previous_winners</b> </td></tr>
<tr><td colspan="1" valign="top"><b>Description</b> </td><td colspan="2" valign="top">User can view previous year’s winners for various convocation medals and MCM Scholarships. </td></tr>
<tr><td colspan="1" valign="top"><b>Actor</b> </td><td colspan="2" valign="top">Students, SPACS Convener, SPACS Assistant </td></tr>
<tr><td colspan="1" valign="top"><b>Precondition</b> </td><td colspan="2">System must have information about winners of medals/scholarships/awards and actor must be logged into the system and Awards and Scholarship page is opened. </td></tr>
<tr><td colspan="1" rowspan="3" valign="top"><b>Main Flow</b> </td><td colspan="1">1 </td><td colspan="1">Actor selects the ‘Previous Award Winners’ option. </td></tr>
<tr><td colspan="1">2 </td><td colspan="1">Actor then selects respective batch and award from the dropdown list provided </td></tr>
<tr><td colspan="1">3 </td><td colspan="1">He clicks ‘Submit’ button. </td></tr>
<tr><td colspan="1"><b>Post conditions</b> </td><td colspan="2" valign="top">List of winners for the selected option are displayed in chronological order. </td></tr>
</table>



<table><tr><th colspan="1"><b>Alternate Flow</b> </th><th colspan="2" valign="top">NIL </th></tr>
<tr><td colspan="1" valign="top"><b>Sub Flow</b> </td><td colspan="2" valign="top">NIL </td></tr>
<tr><td colspan="1" rowspan="2"><b>Global Alternate Flow</b> </td><td colspan="1" rowspan="2" valign="top">GA1 </td><td colspan="1" valign="top">The actor can return to the dashboard at any time by clicking on dashboard button. </td></tr>
<tr><td colspan="1" valign="top"><b>Post Condition:</b> The system returns to the actor’s dashboard. </td></tr>
</table>

2. **Use case description for Student (extending User) as an actor to the system** 

**Use case # 4** 



<table><tr><th colspan="1" valign="top"><b>UC ID</b> </th><th colspan="2" valign="top">UC#4 </th></tr>
<tr><td colspan="1"><b>Use case Name</b> </td><td colspan="2" valign="top"><b>apply_for_convocation_medals</b> </td></tr>
<tr><td colspan="1" valign="top"><b>Description</b> </td><td colspan="2" valign="top">The student can apply for Convocation Medals by filling out a form and uploading necessary documents. </td></tr>
<tr><td colspan="1" valign="top"><b>Actor</b> </td><td colspan="2" valign="top">Student </td></tr>
<tr><td colspan="1" valign="top"><b>Precondition</b> </td><td colspan="2">Student Logged in, opens Awards and Scholarship portal and applications are invited for the same. </td></tr>
<tr><td colspan="1" rowspan="5" valign="top"><b>Main Flow</b> </td><td colspan="1">1 </td><td colspan="1">Student clicks on ‘Apply for Awards’ option and then Convocation Medals. </td></tr>
<tr><td colspan="1" valign="top">2 </td><td colspan="1">Student reads the instructions for applying for the Convocation Medals and clicks on ‘Proceed’ button. </td></tr>
<tr><td colspan="1" valign="top">2 </td><td colspan="1">Student selects the type of application from the available options and the respective form is displayed. </td></tr>
<tr><td colspan="1" valign="top">3 </td><td colspan="1" valign="top">Student fills up all the necessary details in the form.[S1] </td></tr>
<tr><td colspan="1" valign="top">4 </td><td colspan="1" valign="top">After successful upload student clicks on the ‘Submit’ button. </td></tr>
<tr><td colspan="1"><b>Post conditions</b> </td><td colspan="2" valign="top">Application and documents submitted for verification. </td></tr>
<tr><td colspan="1" rowspan="2" valign="top"><b>Sub Flow</b> </td><td colspan="1" valign="top">S1 </td><td colspan="1" valign="top">He can upload supporting documents. </td></tr>
<tr><td colspan="1"></td><td colspan="1" valign="top"><b>Post-condition</b> - Documents are attached along with the form. </td></tr>
<tr><td colspan="1"><b>Alternate Flow</b> </td><td colspan="1"></td><td colspan="1" valign="top">NIL </td></tr>
<tr><td colspan="1" rowspan="2"><b>Global Alternate Flow</b> </td><td colspan="1" rowspan="2" valign="top">GA1 </td><td colspan="1" valign="top">The actor can return to the dashboard at any time by clicking on dashboard button. </td></tr>
<tr><td colspan="1" valign="top"><b>Post Condition:</b> The system returns to the actor’s dashboard. </td></tr>
</table>

**Use case # 5** 



|**UC ID** |UC#5 |
| - | - |
|**Use case Name** |**apply\_for\_mcm\_scholarship** |
|**Description** |The student can apply for MCM scholarship by filling out a form and uploading necessary documents. |
|**Actor** |Student |
|**Precondition** |Student Logged in, opens Scholarship and Awards portal and applications are invited for the same |



<table><tr><th colspan="1" rowspan="4" valign="top"><b>Main Flow</b> </th><th colspan="1">1 </th><th colspan="1">Student clicks on ‘Apply for Awards’ option and selects MCM Scholarship. </th></tr>
<tr><td colspan="1">2 </td><td colspan="1">MCM Scholarship form is displayed. </td></tr>
<tr><td colspan="1" valign="top">3 </td><td colspan="1" valign="top">Student fills up the necessary details in the form[S1] </td></tr>
<tr><td colspan="1" valign="top">4 </td><td colspan="1" valign="top">After successful upload student clicks on the ‘Submit Application’ button. </td></tr>
<tr><td colspan="1"><b>Post conditions</b> </td><td colspan="2" valign="top">Application and documents submitted for verification. </td></tr>
<tr><td colspan="1" rowspan="2" valign="top"><b>Sub Flow</b> </td><td colspan="1" valign="top">S1 </td><td colspan="1">He can upload supporting documents like income certificate and all the required documents (Refer to appendix A for MCM scholarship details). </td></tr>
<tr><td colspan="1"></td><td colspan="1" valign="top"><b>Post-condition</b> - Documents are attached along with the form. </td></tr>
<tr><td colspan="1"><b>Alternate Flow</b> </td><td colspan="1"></td><td colspan="1" valign="top">NIL </td></tr>
<tr><td colspan="1" rowspan="2"><b>Global Alternate Flow</b> </td><td colspan="1" rowspan="2" valign="top">GA1 </td><td colspan="1" valign="top">The actor can return to the dashboard at any time by clicking on dashboard button. </td></tr>
<tr><td colspan="1" valign="top"><b>Post Condition:</b> The system returns to the actor’s dashboard. </td></tr>
</table>

**Use case # 6** 



<table><tr><th colspan="1" valign="top"><b>UC ID</b> </th><th colspan="2" valign="top">UC#6 </th></tr>
<tr><td colspan="1"><b>Use case Name</b> </td><td colspan="2" valign="top"><b>track_application_status</b> </td></tr>
<tr><td colspan="1" valign="top"><b>Description</b> </td><td colspan="2" valign="top">Student views application status for each of the applied medal/scholarship. </td></tr>
<tr><td colspan="1" valign="top"><b>Actor</b> </td><td colspan="2" valign="top">Student </td></tr>
<tr><td colspan="1" valign="top"><b>Precondition</b> </td><td colspan="2">Student must have applied for an award/scholarship and have a valid application number assigned </td></tr>
<tr><td colspan="1" rowspan="4" valign="top"><b>Main Flow</b> </td><td colspan="1">1 </td><td colspan="1">Student clicks on ‘View Application Status’ option. </td></tr>
<tr><td colspan="1">2 </td><td colspan="1">Student selects the ‘Current’ option. </td></tr>
<tr><td colspan="1" valign="top">3 </td><td colspan="1" valign="top">All the applications status is displayed here along with the application ID. </td></tr>
<tr><td colspan="1" valign="top">4 </td><td colspan="1">Student can also selects the ‘History’ option to view the status of the past applied applications. </td></tr>
<tr><td colspan="1"><b>Post conditions</b> </td><td colspan="2" valign="top">The status of all applications submitted by the student in the past are displayed. </td></tr>
<tr><td colspan="1"><b>Alternate Flow</b> </td><td colspan="2" valign="top">NIL </td></tr>
<tr><td colspan="1" valign="top"><b>Sub Flow</b> </td><td colspan="2" valign="top">NIL </td></tr>
<tr><td colspan="1" rowspan="3" valign="top"><b>Global Alternate Flow</b> </td><td colspan="1" rowspan="3" valign="top">GA1 </td><td colspan="1" valign="top">The actor can return to the dashboard at any time by clicking on dashboard button. </td></tr>
<tr><td colspan="1" valign="top"><b>Post Condition:</b> The system returns to the actor’s dashboard. </td></tr>
<tr><td colspan="1"></td></tr>
</table>
**Use case # 7** 



<table><tr><th colspan="1" valign="top"><b>UC ID</b> </th><th colspan="2" valign="top">UC#7 </th></tr>
<tr><td colspan="1"><b>Use case Name</b> </td><td colspan="2" valign="top"><b>Receives_Notification</b> </td></tr>
<tr><td colspan="1" valign="top"><b>Description</b> </td><td colspan="2">The "Receives_Notifications" use case enables a user to receive and interact with notifications generated by the Notification System. The primary actor for this use case is the User, and the secondary actor is the Notification System, responsible for generating and delivering notifications. </td></tr>
<tr><td colspan="1" valign="top"><b>Actor</b> </td><td colspan="2" valign="top">Students, SPACS Convener, SPACS Assistant </td></tr>
<tr><td colspan="1" valign="top"><b>Precondition</b> </td><td colspan="2" valign="top">User has an active account. </td></tr>
<tr><td colspan="1" rowspan="2" valign="top"><b>Main Flow</b> </td><td colspan="1" valign="top">1 </td><td colspan="1" valign="top">The Notification System identifies events requiring notifications. </td></tr>
<tr><td colspan="1" valign="top">2 </td><td colspan="1" valign="top">The Notification System generates notifications based on identified events.    </td></tr>
</table>



<table><tr><th colspan="1" rowspan="2">![](Aspose.Words.c154b3e5-6f3c-4428-91d6-bcdb87880290.002.png)</th><th colspan="1" valign="top">3 </th><th colspan="1" valign="top">The Notification System sends notifications to the User. </th></tr>
<tr><td colspan="1" valign="top">4 </td><td colspan="1" valign="top">. The User receives and views the notifications through the User Interface. </td></tr>
<tr><td colspan="1"><b>Post conditions</b> </td><td colspan="2" valign="top">User successfully receives notifications. </td></tr>
<tr><td colspan="1"><b>Alternate Flow</b> </td><td colspan="2" valign="top">Delayed Notification Delivery. </td></tr>
<tr><td colspan="1" valign="top"><b>Sub Flow</b> </td><td colspan="2" valign="top">NIL </td></tr>
<tr><td colspan="1" rowspan="2"><b>Global Alternate Flow</b> </td><td colspan="1" rowspan="2" valign="top">GA1 </td><td colspan="1" valign="top">`  `Notification System Failure </td></tr>
<tr><td colspan="1" valign="top"><b>Post Condition:</b> The system returns to the actor’s dashboard. </td></tr>
</table>

**Use case # 8** 



<table><tr><th colspan="1" valign="top"><b>UC ID</b> </th><th colspan="2" valign="top">UC#8 </th></tr>
<tr><td colspan="1"><b>Use case Name</b> </td><td colspan="2" valign="top"><b>View_History</b> </td></tr>
<tr><td colspan="1" valign="top"><b>Description</b> </td><td colspan="2" valign="top">The "View_History" use case allows an authenticated user to retrieve and view their historical data through the system. This historical data may include past interactions, transactions, or any relevant activities stored in the database. </td></tr>
<tr><td colspan="1" valign="top"><b>Actor</b> </td><td colspan="2" valign="top">Students, SPACS Convener, SPACS Assistant </td></tr>
<tr><td colspan="1" valign="top"><b>Precondition</b> </td><td colspan="2" valign="top">User is authenticated and has a valid session.   </td></tr>
<tr><td colspan="1" rowspan="3" valign="top"><b>Main Flow ![](Aspose.Words.c154b3e5-6f3c-4428-91d6-bcdb87880290.003.png)</b></td><td colspan="1" valign="top">1 </td><td colspan="1" valign="top">User requests to view their history through the User Interface. </td></tr>
<tr><td colspan="1" valign="top">2 </td><td colspan="1" valign="top">System retrieves historical data from the Database.                                           </td></tr>
<tr><td colspan="1" valign="top">3 </td><td colspan="1" valign="top">System presents the historical data to the User through the User Interface.  . </td></tr>
<tr><td colspan="1"><b>Post conditions</b> </td><td colspan="2" valign="top">User successfully views their history.   </td></tr>
<tr><td colspan="1"><b>Alternate Flow</b> </td><td colspan="2" valign="top">Technical Issue Retrieving Data </td></tr>
<tr><td colspan="1" valign="top"><b>Sub Flow</b> </td><td colspan="2" valign="top">NIL </td></tr>
<tr><td colspan="1" rowspan="2"><b>Global Alternate Flow</b> </td><td colspan="1" rowspan="2" valign="top">GA1 </td><td colspan="1" valign="top">No Historical Data </td></tr>
<tr><td colspan="1" valign="top"><b>Post Condition:</b> The system returns to the actor’s dashboard. </td></tr>
</table>

3. **Use case diagram and description for SPACS Convener (extending User) asan actor to the system** 

**Use case # 9** 



|**UC ID** |UC#9 |
| - | - |
|**Use case Name** |**process\_verified\_applications** |
|**Description** |<p>The actor is able to browse the awards/scholarships applications. While browsing he also gets a facility to sort them according to CPI, Income etc. </p><p>This feature provides an in depth statistics about the applicants. </p>|
|**Actor** |SPACS Convener |



<table><tr><th colspan="1" valign="top"><b>Precondition</b> </th><th colspan="2">Actor logs into the system, opens ‘Awards and Scholarships’ portal and the output of ‘process_submitted_applications’ </th></tr>
<tr><td colspan="1" rowspan="5" valign="top"><b>Main Flow</b> </td><td colspan="1">1 </td><td colspan="1">Click on ‘Browse Applications’ </td></tr>
<tr><td colspan="1">2 </td><td colspan="1">Select an award/scholarship </td></tr>
<tr><td colspan="1" valign="top">3 </td><td colspan="1">All the verified applications for the above selected option are displayed and can be sorted according to various factors as displayed in description. </td></tr>
<tr><td colspan="1" valign="top">4 </td><td colspan="1" valign="top">Actor selects one of the applications and checks that application. </td></tr>
<tr><td colspan="1" valign="top">5 </td><td colspan="1" valign="top">Actor checks the hardcopies of submitted files (if required), then he updates the status of the application to the APPROVED. [A1] </td></tr>
<tr><td colspan="1"><b>Post conditions</b> </td><td colspan="2" valign="top">Actor grants the application and the respective student is regarding the same. </td></tr>
<tr><td colspan="1" rowspan="2" valign="top"><b>Alternate Flow</b> </td><td colspan="1" valign="top">A1 </td><td colspan="1">If actor finds any false information he REJECTS the application by clicking the REJECT button corresponding to that application. </td></tr>
<tr><td colspan="1"></td><td colspan="1"><b>Post Condition</b>: The corresponding application gets rejected and the applicant (student) is informed regarding the same. </td></tr>
<tr><td colspan="1" valign="top"><b>Sub Flow</b> </td><td colspan="2" valign="top">NIL </td></tr>
<tr><td colspan="1" rowspan="2"><b>Global Alternate Flow</b> </td><td colspan="1" rowspan="2" valign="top">GA1 </td><td colspan="1" valign="top">The actor can return to the dashboard at any time by clicking on dashboard button. </td></tr>
<tr><td colspan="1" valign="top"><b>Post Condition:</b> The system returns to the actor’s dashboard. </td></tr>
</table>

**Use case # 10** 



|**UC ID** |UC#10 |
| - | - |
|**Use case Name** |**manage\_catalogue** |
|**Description** |The actor can make changes to the application procedure and also scrap the existing awards/prizes/scholarship. |



<table><tr><th colspan="1" valign="top"><b>Actor</b> </th><th colspan="2" valign="top">SPACS Convener </th></tr>
<tr><td colspan="1" valign="top"><b>Precondition</b> </td><td colspan="2" valign="top">Logs into the system, opens awards/scholarships portal </td></tr>
<tr><td colspan="1" rowspan="3" valign="top"><b>Main Flow</b> </td><td colspan="1" valign="top">1 </td><td colspan="1">Selects ‘Manage Catalogue’ option on the screen and list of awards and scholarships are displayed. </td></tr>
<tr><td colspan="1" valign="top">2 </td><td colspan="1">If an award/medal has to be modified/deleted then click on ‘edit button’ next to the award/medal </td></tr>
<tr><td colspan="1" valign="top">3 </td><td colspan="1" valign="top">Make the necessary changes and click on ‘Save changes’ button. </td></tr>
<tr><td colspan="1"><b>Post conditions</b> </td><td colspan="2">The award/scholarship database is updated accordingly, and the SPACS manual needs to be updated as a result. </td></tr>
<tr><td colspan="1"><b>Alternate Flow</b> </td><td colspan="2" valign="top">NIL </td></tr>
<tr><td colspan="1" valign="top"><b>Sub Flow</b> </td><td colspan="2" valign="top">NIL </td></tr>
<tr><td colspan="1" rowspan="2"><b>Global Alternate Flow</b> </td><td colspan="1" rowspan="2" valign="top">GA1 </td><td colspan="1" valign="top">The actor can return to the dashboard at any time by clicking on dashboard button. </td></tr>
<tr><td colspan="1" valign="top"><b>Post Condition:</b> The system returns to the actor’s dashboard. </td></tr>
</table>

**Use case # 11** 



<table><tr><th colspan="1" valign="top"><b>UC ID</b> </th><th colspan="2" valign="top">UC#11 </th></tr>
<tr><td colspan="1"><b>Use case Name</b> </td><td colspan="2" valign="top"><b>invite_applications</b> </td></tr>
<tr><td colspan="1" valign="top"><b>Description</b> </td><td colspan="2">He can invite the applications for the MCM scholarship or awards (if necessary) for all the students satisfied the criteria as mentioned in SPACS manual. </td></tr>
<tr><td colspan="1" valign="top"><b>Actor</b> </td><td colspan="2" valign="top">SPACS Convener </td></tr>
<tr><td colspan="1" valign="top"><b>Precondition</b> </td><td colspan="2" valign="top">Logs into the system </td></tr>
<tr><td colspan="1" rowspan="4" valign="top"><b>Main Flow</b> </td><td colspan="1" valign="top">1 </td><td colspan="1">Select ‘Invite applications’ option and the list of awards or scholarship is displayed for selection </td></tr>
<tr><td colspan="1">2 </td><td colspan="1">Selects one award or MCM scholarship and click NEXT. </td></tr>
<tr><td colspan="1" valign="top">3 </td><td colspan="1">He has to select the Year of Students to which he want to invite the MCM applications or awards and click NEXT. </td></tr>
<tr><td colspan="1" valign="top">4 </td><td colspan="1" valign="top">After successful completion, Clicks INVITE button. </td></tr>
<tr><td colspan="1"><b>Post conditions</b> </td><td colspan="2" valign="top">The notification is pushed to all the recipients on their homepage upon logging in. </td></tr>
<tr><td colspan="1"><b>Alternate Flow</b> </td><td colspan="2" valign="top">NIL </td></tr>
<tr><td colspan="1"><b>Sub Flow</b> </td><td colspan="2">NIL </td></tr>
<tr><td colspan="1" rowspan="2"><b>Global Alternate Flow</b> </td><td colspan="1" rowspan="2" valign="top">GA1 </td><td colspan="1" valign="top">The actor can return to the dashboard at any time by clicking on dashboard button. </td></tr>
<tr><td colspan="1" valign="top"><b>Post Condition:</b> The system returns to the actor’s dashboard. </td></tr>
</table>

4. **Use case diagram and description for SPACS Assistant (extends User) asactor to the system** 

**Use case # 12** 

**UC ID**  UC#12 ![](Aspose.Words.c154b3e5-6f3c-4428-91d6-bcdb87880290.004.png)



<table><tr><th colspan="1"><b>Use case Name</b> </th><th colspan="2" valign="top"><b>process_submitted_applications</b> </th></tr>
<tr><td colspan="1" valign="top"><b>Description</b> </td><td colspan="2"><p>The actor is able to browse the awards/scholarships applications. While browsing he also gets a facility to sort them according to CPI, Income etc. </p><p>This feature provides an indepth statistics about the applicants. </p></td></tr>
<tr><td colspan="1"><b>Actor</b> </td><td colspan="2">SPACS Assistant </td></tr>
<tr><td colspan="1" valign="top"><b>Precondition</b> </td><td colspan="2" valign="top">Actor logs into the system, opens ‘Awards and Scholarships’ portal </td></tr>
<tr><td colspan="1" rowspan="5" valign="top"><b>Main Flow</b> </td><td colspan="1">1 </td><td colspan="1">Click on ‘Browse applications’ </td></tr>
<tr><td colspan="1">2 </td><td colspan="1">Select an award/scholarship </td></tr>
<tr><td colspan="1">3 </td><td colspan="1">All the Submitted applications for the above selected option are displayed </td></tr>
<tr><td colspan="1" valign="top">4 </td><td colspan="1" valign="top">Actor selects one of the applications and checks that application. </td></tr>
<tr><td colspan="1" valign="top">5 </td><td colspan="1" valign="top">Actor checks the hardcopies of submitted files (if required), then he updates the status of the application to the VERIFIED. [A1] </td></tr>
<tr><td colspan="1"><b>Post conditions</b> </td><td colspan="2" valign="top">Actor verifies the application and the respective student is notified regarding the same. </td></tr>
<tr><td colspan="1" rowspan="2" valign="top"><b>Alternate Flow</b> </td><td colspan="1" valign="top">A1 </td><td colspan="1">If actor finds any false information, he REJECTS the application by clicking the REJECTbutton corresponding to that application. </td></tr>
<tr><td colspan="1"></td><td colspan="1"><b>Post Condition</b>: The corresponding application gets rejected and the applicant (student) is notified regarding the same. </td></tr>
<tr><td colspan="1" valign="top"><b>Sub Flow</b> </td><td colspan="2" valign="top">NIL </td></tr>
<tr><td colspan="1" rowspan="2"><b>Global Alternate Flow</b> </td><td colspan="1" rowspan="2" valign="top">GA1 </td><td colspan="1" valign="top">The actor can return to the dashboard at any time by clicking on dashboard button. </td></tr>
<tr><td colspan="1" valign="top"><b>Post Condition:</b> The system returns to the actor’s dashboard. </td></tr>
</table>

**Use case # 13** 



<table><tr><th colspan="1" valign="top"><b>UC ID</b> </th><th colspan="2" valign="top">UC#13 </th></tr>
<tr><td colspan="1"><b>Use case Name</b> </td><td colspan="2" valign="top"><b>Notify_Students</b> </td></tr>
<tr><td colspan="1" valign="top"><b>Description</b> </td><td colspan="2">The "Notify_Students" use case enables an administrator to send notifications to targeted students through the Notification System. The primary actor for this use case is the Administrator, and secondary actors include the Notification System and Students. This use case facilitates communication from the administrator to students for various purposes, such as important announcements or updates. </td></tr>
<tr><td colspan="1" valign="top"><b>Actor</b> </td><td colspan="2" valign="top">Students, SPACS Convener, SPACS Assistant </td></tr>
<tr><td colspan="1" valign="top"><b>Precondition</b> </td><td colspan="2"><p>- Administrator is logged into the system.                                                       </p><p>- Notification System is operational.                                                             </p><p>- Students are registered in the system.   </p></td></tr>
<tr><td colspan="1" rowspan="5" valign="top"><b>Main Flow ![](Aspose.Words.c154b3e5-6f3c-4428-91d6-bcdb87880290.005.png)![](Aspose.Words.c154b3e5-6f3c-4428-91d6-bcdb87880290.006.png)![](Aspose.Words.c154b3e5-6f3c-4428-91d6-bcdb87880290.007.png)</b></td><td colspan="1" valign="top">1 </td><td colspan="1" valign="top">Administrator initiates the notification process through the User Interface. </td></tr>
<tr><td colspan="1" valign="top">2 </td><td colspan="1" valign="top">` `Administrator provides details for the notification (e.g., message, recipients).             </td></tr>
<tr><td colspan="1" valign="top">3 </td><td colspan="1" valign="top">Notification System generates notifications based on the provided details. </td></tr>
<tr><td colspan="1" valign="top">4 </td><td colspan="1" valign="top">Notification System sends notifications to the targeted Students.    </td></tr>
<tr><td colspan="1" valign="top">5 </td><td colspan="1" valign="top">Students receive and view the notifications through the User Interface </td></tr>
<tr><td colspan="1"><b>Post conditions</b> </td><td colspan="2" valign="top">Students successfully receive notifications.   </td></tr>
<tr><td colspan="1"><b>Alternate Flow</b> </td><td colspan="2" valign="top">Delayed Notification Delivery </td></tr>
<tr><td colspan="1" valign="top"><b>Sub Flow</b> </td><td colspan="2" valign="top">NIL </td></tr>
<tr><td colspan="1" valign="top"><b>Global</b> </td><td colspan="1" valign="top">GA1 </td><td colspan="1" valign="top">Notification System Failure. </td></tr>
</table>

![](Aspose.Words.c154b3e5-6f3c-4428-91d6-bcdb87880290.008.png)

**Alternate  Post Condition:** The system returns to the actor’s dashboard. ![](Aspose.Words.c154b3e5-6f3c-4428-91d6-bcdb87880290.009.png)![](Aspose.Words.c154b3e5-6f3c-4428-91d6-bcdb87880290.010.png)**Flow** 

3. Other Constraints 
1. User Interface 

`   `The user interface should comply with the colour scheming and dashboard design of the FUSIONIIT. Users should be able to navigate from one functionality to  other.  Inter  module  navigation  should  be  smooth.  All  the  functionalities should be easy to use and no specific training should be required for the usage of the module. 

2. Tech Stack Used 

For developing the mobile app, dart language is used with the flutter framework. For web Javascript, HTML, CSS are used with Django framework. Postresql database is used for storing all fusion data. 

- 4. Non- Functional Requirements
1. Performance: 

` `The system should respond to user interactions quickly. Response time for booking actions, inventory updates, and notifications should be less. 

2. Scalability:

The system should handle a mass of concurrent users. System performance should be evaluated under increasing load conditions. 

3. Availability:

The system should be available 99.9% of the time. 

4. Security:

Ensure data confidentiality and integrity. Role-based authorization ensures that users can only perform actions relevant to their designated roles. 

- 5. Module dependencies with other fusion modules 
- Integration at the UI Level: 

`       `Users log into the Fusion application and land on the main dashboard.         Navigation should include direct links or buttons in Fusion’s menu, ensuring a clear path for each actor (student, spacs convener, spacs assistant) to access their specific functionalities withing the awards and scholarships module. 

- Module Level: 

  Awards and Scholarships Module interact with Notification, Dashboard, and file transfering system. 
