**Fusion ERP**

**Software Requirements Specification**

**OS-2-PRIMARYHEALTHCENTER MOBILEAPP**

Faculty Mentor:

Dr. Sraban Kumar Mohanty

Prepared by :

21bcs163 Pratham (**Team Lead**) 21bcs241 Vikas

21bcs243 Vishal Bairagi 21bcs245 Vishnu J Nair 21bcs246 Vishwajeet Toppo 21bcs247 Yadav Pritesh

1  **Introduction**
1. **Introduction about the Fusion – A brief Description**

FusionIIIT stands as a testament to the seamless integration and automation of diverse functions within PDPM Indian Institute of Information Technology, Design and Manufacturing, Jabalpur. Crafted with precision using Python 3.8 and powered by the Django Web framework, this initiative is a student-driven endeavor designed to elevate the institute's operational landscape. Encompassing everything from efficient administration management to academic prowess and miscellaneous departmental tasks, FusionIIIT is a holistic solution that harmonizes the intricacies of campus life.

Imagine it as a digital wizard that takes care of everything, from organizing the administrative stuff to making academics smoother. It's not just limited to the usual tasks; FusionIIIT jumps into various departments and sections, making sure every corner of campus life runs smoothly.

In the admin side, it handles the complicated paperwork and processes. For academics, it brings a digital touch, making learning and managing courses easier. But it doesn't stop there; FusionIIIT is like a friendly companion for all the different parts of the campus, making sure everything works well.

In simpler terms, FusionIIIT is not just a tool – it's a helpful friend, making life at PDPM IIITDM Jabalpur more organized and enjoyable for everyone.

2. **Purpose of the module:**

The purpose of the project entitled as PRIMARY HEALTH CENTRE MANAGEMENT SYSTEM is to computerize the Office Management and to manage different activities related to Primary Health Centre of PDPM IIITDM Jabalpur.

- Patient Registration and Record Management.
- Appointment and Prescription Record Keeping
- Doctor Availability and Scheduling
- Implementing measures to ensure the security and privacy of patient data
3. **Scope of the module**

The users of this module will be the registered students of the Institute (PDPM IIITDM Jabalpur), Faculty Members and their dependencies(family members).

This software system will be a Mobile application based Health Care Management System to be used by the above-mentioned people. Interface will enable the actors to view schedules for consulting doctors, to keep a track of their health records.

The compounder will be able to update the Doctor's schedule and patient log, manage the inventory, and make announcements of updates.

2  **User/Actor characteristics**

There are two types of users that interact with the system.

- Patient (Students &Employees)
- Compounder

**UserRoles and Permissions**:

Patients should have access to the following features:

- **View doctorschedule:** Patients should be able to see the schedule of doctors and their availability.
- **View announcements:** Patients should be able to view important announcements from the health center.
- **View health record**: Patients should have access to their own health records.
- **Request ambulance:** Patients should be able to request an ambulance in case of emergencies.
- **Provide feedback:** Patients should be able to provide feedback on their experiences.
- **View pathologist schedule**: Patients would have access to the schedule of pathologists visiting the health center.

Patients who are employees should have additional access to:

- **Dependency health record:** Staff members should be able to manage health records of their dependents.
- **Apply formedical relief:** Patients(specifically employees) should be able to apply for medical relief if needed.

Compounder (admin) should have access to the following features:

- **Update doctorschedule:** Compounder should be able to update the schedule of doctors.
- **Update patient log:** Compounder should be able to update patient logs and records.
- **Make announcements:** Compounders should be able to create and publish announcements.
- **Generate reports:** Compounder should be able to generate reports based on various parameters.
- **Forward medical relief:** Compounder should be able to process and forward medical relief requests.
- **Manage inventory:** Compounder should be able to manage the inventory of medicines and medical supplies.
- **Update pathologist schedule**: Compounder will be able to update the schedule of the pathologist
3  **Functional Requirements**
1. **UserAuthentication:** The system should have a secure user authentication mechanism to ensure that only registered students, faculty members, dependents, and compounders can access the application.
1. **UserRoles and Permissions:** Different user roles (students, faculty, dependents, compounders) with specific permissions should be defined to regulate access to various features and data within the application.
1. **Doctor's Schedule:** The system should display the schedule of consulting doctors, including their availability, timings, and consultation slots.Users should be able to request, book, or cancel appointments through the application.
1. **Health Records Management:** Users should have the ability to view and update their health records, including medical history, prescriptions, and appointments.The system should allow users to upload relevant health documents or reports.
1. **Compounder's Features:** Compounders should be able to update doctor schedules, including adding or modifying consultation slots. Inventory management functionalities for tracking medical supplies, updating stock levels, and generating alerts for low inventory.

Use Case Diagram

![](images/Aspose.Words.81cc532b-5eb8-45cf-b714-16287de7997c.001.png)

Use case Description



<table><tr><th colspan="1" valign="top"><b>UCID</b></th><th colspan="4" valign="top">UC#1</th></tr>
<tr><td colspan="1"><b>Use case Name</b></td><td colspan="4" valign="top">view_health_record</td></tr>
<tr><td colspan="1" valign="top"><b>Description</b></td><td colspan="4">Our system empowers patients to effortlessly track real-time health updates and access historical records for themselves and dependents. User-friendly and secure, it transforms health management into a personalized, proactive experience.</td></tr>
<tr><td colspan="1" valign="top"><b>Actor</b></td><td colspan="4" valign="top"><b>Patient</b></td></tr>
<tr><td colspan="1" valign="top"><b>Precondition</b></td><td colspan="4" valign="top">The Patient is logged in into the system.</td></tr>
<tr><td colspan="1" rowspan="2" valign="top"><b>Main Flow</b></td><td colspan="1" valign="top">1</td><td colspan="3" valign="top">The patient opens the "View Health Record"section.</td></tr>
<tr><td colspan="1" valign="top">2</td><td colspan="3" valign="top">The system displays a list of health records along with their latest statues[A1]</td></tr>
<tr><td colspan="1"><b>Post conditions</b></td><td colspan="4" valign="top">The health records are reflected in the database.</td></tr>
<tr><td colspan="1" valign="top"><b>Alternate Flow</b></td><td colspan="1" valign="top">A1</td><td colspan="2" valign="top">1</td><td colspan="1">If a newly registered patient has no existing health records to view.</td></tr>
<tr><td colspan="1" rowspan="2" valign="top"><b>Sub Flow</b></td><td colspan="2" valign="top">1</td><td colspan="2" valign="top">The patient goes to manage dependencies.</td></tr>
<tr><td colspan="2" valign="top">2</td><td colspan="2" valign="top">The patient also view health records of their dependencies[SA1]</td></tr>
<tr><td colspan="1"></td><td colspan="2" valign="top">3</td><td colspan="2" valign="top">The patient can add/delete a dependency.</td></tr>
<tr><td colspan="1" valign="top"><b>Alternate Sub Flow</b></td><td colspan="2" valign="top">SA1</td><td colspan="2" valign="top">If no dependencies exist, the system notifies the patient that no dependent health records are currently available.</td></tr>
<tr><td colspan="1" rowspan="2" valign="top"><b>Global Alternate Flow</b></td><td colspan="1" valign="top">GA1</td><td colspan="3">Due to high traffic, logging in may be temporarily affected. We apologize for the inconvenience</td></tr>
<tr><td colspan="1" valign="top">GA2</td><td colspan="3" valign="top">If a technical error occurs during the execution of any action (e.g., database failure, server issues), the system displays an error message and logs the incident.</td></tr>
</table>



<table><tr><th colspan="1"><b>UCID</b></th><th colspan="2">UC#2</th></tr>
<tr><td colspan="1"><b>Use case Name</b></td><td colspan="2">apply_for_medical_reimbursement</td></tr>
<tr><td colspan="1" valign="top"><b>Description</b></td><td colspan="2">The "apply_for_medical_reimbursement"use case allows employees to apply for medical relief by requesting a medical certificate. This certificate is official documentation to support their need for medical assistance or leave due to health reasons.</td></tr>
<tr><td colspan="1"><b>Actor</b></td><td colspan="2"><b>Patient(employee)</b></td></tr>
<tr><td colspan="1" valign="top"><b>Precondition</b></td><td colspan="2" valign="top">The employee logged in to the system.</td></tr>
<tr><td colspan="1" rowspan="3" valign="top"><b>Main Flow</b></td><td colspan="1" valign="top">1</td><td colspan="1" valign="top">The employee navigates to the "medical relief"section.</td></tr>
<tr><td colspan="1" valign="top">2</td><td colspan="1" valign="top">The system displays a form.</td></tr>
<tr><td colspan="1">3</td><td colspan="1">The employee fills out the form.[A1]</td></tr>
<tr><td colspan="1"></td><td colspan="1">4</td><td colspan="1">The system asks for a confirmation</td></tr>
<tr><td colspan="1"></td><td colspan="1" valign="top">5</td><td colspan="1" valign="top">The employee confirms the submission[A2]</td></tr>
<tr><td colspan="1"></td><td colspan="1" valign="top">6</td><td colspan="1" valign="top">The system returns to the employee ‘Dashboard’</td></tr>
<tr><td colspan="1" valign="top"><b>Postconditions</b></td><td colspan="2" valign="top">The form was successfully submitted and stored in the database.</td></tr>
</table>



<table><tr><th colspan="1" valign="top"><b>Alternate Flow</b></th><th colspan="1" valign="top">A1</th><th colspan="1" valign="top">1</th><th colspan="1">The employee chooses not to confirm but rather chooses to cancel.</th></tr>
<tr><td colspan="1" valign="top"><b>Sub Flow</b></td><td colspan="3" valign="top">NIL</td></tr>
<tr><td colspan="1" rowspan="2" valign="top"><b>Global Alternate Flow</b></td><td colspan="1" valign="top">GA1</td><td colspan="2" valign="top">The employee can ‘cancel’the procedure at any time by exercising such an option and will be directed to the dashboard.</td></tr>
<tr><td colspan="1" valign="top">GA2</td><td colspan="2" valign="top">If a technical error occurs during the execution of any action (e.g., database failure, server issues), the system displays an error message and logs the incident.</td></tr>
</table>



<table><tr><th colspan="1" valign="top"><b>UCID</b></th><th colspan="2" valign="top">UC#3</th></tr>
<tr><td colspan="1" valign="top"><b>Use case Name</b></td><td colspan="2" valign="top">view_doctor_schedule</td></tr>
<tr><td colspan="1" valign="top"><b>Description</b></td><td colspan="2">The "View Doctor Schedule"use case allows patients to view doctor schedules in PHC through the Fusion portal.</td></tr>
<tr><td colspan="1" valign="top"><b>Actor</b></td><td colspan="2" valign="top"><b>Patient</b></td></tr>
<tr><td colspan="1"><b>Precondition</b></td><td colspan="2">The patient is logged in into the system.</td></tr>
<tr><td colspan="1" rowspan="3" valign="top"><b>Main Flow</b></td><td colspan="1">1</td><td colspan="1">The patient navigates to the "View Doctor Schedule"section.</td></tr>
<tr><td colspan="1">2</td><td colspan="1">The system displays doctor schedules.</td></tr>
<tr><td colspan="1" valign="top">3</td><td colspan="1" valign="top">The patient view doctor schedule and book appointment accordingly</td></tr>
<tr><td colspan="1" valign="top"><b>Post conditions</b></td><td colspan="2" valign="top">The patient viewed the doctor schedule</td></tr>
<tr><td colspan="1" valign="top"><b>Global Alternate Flow</b></td><td colspan="1" valign="top">GA1</td><td colspan="1" valign="top">If a technical error occurs during the execution of any action (e.g., database failure, server issues), the system displays an error message and logs the incident.</td></tr>
</table>



<table><tr><th colspan="1"><b>UCID</b></th><th colspan="2">UC#4</th></tr>
<tr><td colspan="1" valign="top"><b>Use case Name</b></td><td colspan="2" valign="top">view_pathologist_schedule</td></tr>
<tr><td colspan="1" valign="top"><b>Description</b></td><td colspan="2" valign="top">The "View Pathologist Schedule"use case allows patients to view pathologist schedules in PHC through the Fusion portal.</td></tr>
<tr><td colspan="1" valign="top"><b>Actor</b></td><td colspan="2" valign="top"><b>Patient</b></td></tr>
<tr><td colspan="1" valign="top"><b>Precondition</b></td><td colspan="2" valign="top">The patient is logged in into the system.</td></tr>
<tr><td colspan="1" rowspan="2" valign="top"><b>Main Flow</b></td><td colspan="1">1</td><td colspan="1">The patient navigates to the "View Pathologist Schedule"section.</td></tr>
<tr><td colspan="1">2</td><td colspan="1">The system displays a pathologist schedule.</td></tr>
</table>



||3|The patient views the schedule.|
| :- | - | - |
|**Post conditions**||The updated pathologist schedule information is reflected in the database.|
|**Global Alternate Flow**|GA1|If a technical error occurs during the execution of any action (e.g., database failure, server issues), the system displays an error message and logs the incident.|



<table><tr><th colspan="1"><b>UCID</b></th><th colspan="2">UC#5</th></tr>
<tr><td colspan="1"><b>Use case Name</b></td><td colspan="2">view_announcements</td></tr>
<tr><td colspan="1" valign="top"><b>Description</b></td><td colspan="2">The "view_announcement"use case allows patient to see the latest announcement made on the Fusion portal by the compounder.</td></tr>
<tr><td colspan="1"><b>Actor</b></td><td colspan="2"><b>Patient</b></td></tr>
<tr><td colspan="1"><b>Precondition</b></td><td colspan="2">The patient is logged in into the system.</td></tr>
<tr><td colspan="1" rowspan="2" valign="top"><b>Main Flow</b></td><td colspan="1">1</td><td colspan="1">The patient navigates to the "Announcement"section.</td></tr>
<tr><td colspan="1">2</td><td colspan="1">The patient sees the latest announcements.</td></tr>
<tr><td colspan="1" valign="top"><b>Global Alternate Flow</b></td><td colspan="1" valign="top">GA1</td><td colspan="1">If a technical error occurs during the execution of any action (e.g., database failure, server issues), the system displays an error message and logs the incident.</td></tr>
</table>



<table><tr><th colspan="1"><b>UCID</b></th><th colspan="2">UC#6</th></tr>
<tr><td colspan="1"><b>Use case Name</b></td><td colspan="2">give_feedback</td></tr>
<tr><td colspan="1" valign="top"><b>Description</b></td><td colspan="2" valign="top">The "give_feedback"use case allows a patient to provide his/her feedback on the Fusion portal by the compounder.</td></tr>
<tr><td colspan="1" valign="top"><b>Actor</b></td><td colspan="2" valign="top"><b>Patient</b></td></tr>
<tr><td colspan="1"><b>Precondition</b></td><td colspan="2">The patient is logged in into the system.</td></tr>
<tr><td colspan="1" rowspan="2" valign="top"><b>Main Flow</b></td><td colspan="1">1</td><td colspan="1">The patient navigates to the "Feedback"section.</td></tr>
<tr><td colspan="1" valign="top">2</td><td colspan="1" valign="top">The patient fills the feedback form.</td></tr>
<tr><td colspan="1"></td><td colspan="1" valign="top">3</td><td colspan="1" valign="top">The patient submits the form.</td></tr>
<tr><td colspan="1" valign="top"><b>Global Alternate Flow</b></td><td colspan="1" valign="top">GA1</td><td colspan="1" valign="top">If a technical error occurs during the execution of any action (e.g., database failure, server issues), the system displays an error message and logs the incident.</td></tr>
</table>



|**UCID**|UC#7|
| - | - |
|**Use case Name**|update\_patient\_health\_record|
|**Description**|Compounder have the capability to diligently update patient logs, ensuring they accurately reflect the latest treatments and any changes in the health record, promoting comprehensive and up-to-date patient information|
|**Actor**|**Compounder**|
|**Precondition**|The Compounder is logged in into the system.|



<table><tr><th colspan="1" rowspan="2" valign="top"><b>Main Flow</b></th><th colspan="1">1</th><th colspan="3">The compounder opens the "update Health Record"section of a specific patient.</th></tr>
<tr><td colspan="1">2</td><td colspan="3">The system displays previous list of health records.[A1]</td></tr>
<tr><td colspan="1"></td><td colspan="1">3</td><td colspan="3">Compounder enter new records of latest appointment happened.[A2]</td></tr>
<tr><td colspan="1"><b>Post conditions</b></td><td colspan="4" valign="top">The health records changes/updates are reflected in the database.</td></tr>
<tr><td colspan="1" valign="top"><b>Alternate Flow</b></td><td colspan="1" valign="top">A1</td><td colspan="2" valign="top">1</td><td colspan="1" valign="top">If a newly registered patient has no existing health records to view.</td></tr>
<tr><td colspan="1"></td><td colspan="1" valign="top">A2</td><td colspan="2" valign="top">1</td><td colspan="1" valign="top">If the appointment was canceled, nothing new happened in the health record.</td></tr>
<tr><td colspan="1" valign="top"><b>Sub Flow</b></td><td colspan="4" valign="top">The compounder also update health records of their dependencies[SA1]</td></tr>
<tr><td colspan="1" valign="top"><b>Alternate Sub Flow</b></td><td colspan="2" valign="top">SA1</td><td colspan="2">If no dependencies exist, the system notifies the compounder that no dependent health records are currently available.</td></tr>
<tr><td colspan="1" rowspan="2" valign="top"><b>Global Alternate Flow</b></td><td colspan="1" valign="top">GA1</td><td colspan="3">Due to high traffic, logging in may be temporarily affected. We apologize for the inconvenience</td></tr>
<tr><td colspan="1" valign="top">GA2</td><td colspan="3">If a technical error occurs during the execution of any action (e.g., database failure, server issues), the system displays an error message and logs the incident.</td></tr>
</table>



<table><tr><th colspan="1"><b>UCID</b></th><th colspan="2">UC#8</th></tr>
<tr><td colspan="1"><b>Use case Name</b></td><td colspan="2">manage_inventory</td></tr>
<tr><td colspan="1" valign="top"><b>Description</b></td><td colspan="2">The "manage_inventory"use case allows the compounder to check the available stocks of medicines, blood and beds available and update accordingly through the Fusion portal.</td></tr>
<tr><td colspan="1"><b>Actor</b></td><td colspan="2"><b>Compounder</b></td></tr>
<tr><td colspan="1"><b>Precondition</b></td><td colspan="2">The compounder is logged in into the system.</td></tr>
<tr><td colspan="1" rowspan="3" valign="top"><b>Main Flow</b></td><td colspan="1">1</td><td colspan="1">The compounder navigates to the "Inventory"section.</td></tr>
<tr><td colspan="1">2</td><td colspan="1">The compounder goes to the medicines section.</td></tr>
<tr><td colspan="1">3</td><td colspan="1">The compounder selects a medicine to update if required.</td></tr>
<tr><td colspan="1"></td><td colspan="1">4</td><td colspan="1">The compounder goes to the blood bank section and updates if required.</td></tr>
<tr><td colspan="1"></td><td colspan="1" valign="top">5</td><td colspan="1" valign="top">The compounder goes to the bed section and updates if required.</td></tr>
<tr><td colspan="1" valign="top"><b>Post conditions</b></td><td colspan="2" valign="top">The updated information is reflected in the database.</td></tr>
<tr><td colspan="1" valign="top"><b>Global Alternate Flow</b></td><td colspan="1" valign="top">GA1</td><td colspan="1">If a technical error occurs during the execution of any action (e.g., database failure, server issues), the system displays an error message and logs the incident.</td></tr>
</table>



|**UC ID**|UC#9|
| - | - |
|**Use case Name**|forward\_medical\_reimbursement|



<table><tr><th colspan="1" valign="top"><b>Description</b></th><th colspan="3">The "forward_medical_reimbursement "use case enables the compounder to either approve or deny a patient's request for medical relief.</th></tr>
<tr><td colspan="1" valign="top"><b>Actor</b></td><td colspan="3" valign="top"><b>Compounder</b></td></tr>
<tr><td colspan="1" valign="top"><b>Precondition</b></td><td colspan="3" valign="top">The compounder logged in to the system.</td></tr>
<tr><td colspan="1" rowspan="8" valign="top"><b>Main Flow</b></td><td colspan="1">1</td><td colspan="2">The compounder chose the option to see the pending requests for medical relief.</td></tr>
<tr><td colspan="1" valign="top">2</td><td colspan="2" valign="top">The system presents a list of the pending requests for leave.</td></tr>
<tr><td colspan="1" valign="top">3</td><td colspan="2" valign="top">The compounder selects one of the ’ pending requests for medical relief’ to view details.</td></tr>
<tr><td colspan="1" valign="top">4</td><td colspan="2" valign="top">A form containing the details of the medical relief request gets displayed along with options for actions to be taken</td></tr>
<tr><td colspan="1" valign="top">5</td><td colspan="2" valign="top">The compounder chooses an action [A1]</td></tr>
<tr><td colspan="1" valign="top">6</td><td colspan="2" valign="top">The System asks for a confirmation</td></tr>
<tr><td colspan="1" valign="top">7</td><td colspan="2" valign="top">The compounder confirms for the action [A2]</td></tr>
<tr><td colspan="1">8</td><td colspan="2">The system presents an acknowledgment including all the furnished details of the leave request and action taken</td></tr>
<tr><td colspan="1"></td><td colspan="1">9</td><td colspan="2">The system returns to the compounder ‘Dashboard’</td></tr>
<tr><td colspan="1" valign="top"><b>Postconditions</b> </td><td colspan="3" valign="top">The updated information about medical relief is reflected in the database.</td></tr>
<tr><td colspan="1" rowspan="4" valign="top"><b>Alternate Flow</b></td><td colspan="1" rowspan="2" valign="top">A1</td><td colspan="1" valign="top">1</td><td colspan="1" valign="top">In the case of the ‘reject’ option, the system seeks the reason/comments from the compounder. The compounder provides the comments and confirm</td></tr>
<tr><td colspan="1" valign="top">2</td><td colspan="1"><b>Post-condition</b> – The system returns to the compounder ‘Dashboard’ – initial screen.</td></tr>
<tr><td colspan="1" rowspan="2" valign="top">A2</td><td colspan="1" valign="top">1</td><td colspan="1" valign="top">The compounder chooses not to confirm.</td></tr>
<tr><td colspan="1" valign="top">2</td><td colspan="1"><b>Post-condition</b> – The system displays the form with the data filled in so far.</td></tr>
<tr><td colspan="1" valign="top"><b>Sub Flow</b></td><td colspan="3">The employee is notified of the compounder action as the status update of the application</td></tr>
<tr><td colspan="1" valign="top"><b>Global Alternate Flow</b></td><td colspan="1" valign="top">GA1</td><td colspan="2" valign="top">If a technical error occurs during the execution of any action (e.g., database failure, server issues), the system displays an error message and logs the incident.</td></tr>
</table>



|**UCID**|UC#10|
| - | - |
|**Use case Name**|update\_doctor\_schedule|
|**Description**|The "Update Doctor Schedule"use case allows the compounder to update doctor schedules in PHC through the Fusion portal.|



<table><tr><th colspan="1"><b>Actor</b></th><th colspan="3"><b>Compounder</b></th></tr>
<tr><td colspan="1"><b>Precondition</b></td><td colspan="3">The Compounder is logged in into the system.</td></tr>
<tr><td colspan="1" rowspan="3" valign="top"><b>Main Flow</b></td><td colspan="1">1</td><td colspan="2">The Compounder navigates to the "Update Doctor Schedule" section.</td></tr>
<tr><td colspan="1">2</td><td colspan="2">The system displays a list of doctor schedules</td></tr>
<tr><td colspan="1">3</td><td colspan="2">The compounder update doctor schedules accordingly</td></tr>
<tr><td colspan="1" valign="top"><b>Post conditions</b></td><td colspan="3" valign="top">The updated doctor schedule information is reflected in the database.</td></tr>
<tr><td colspan="1" valign="top"><b>Alternate Flow</b></td><td colspan="1" valign="top">A1</td><td colspan="1" valign="top">1</td><td colspan="1" valign="top">No doctor is available so compounder not update any schedule, Only reviewed it.</td></tr>
<tr><td colspan="1" valign="top"><b>Sub Flow</b></td><td colspan="3" valign="top">NIL</td></tr>
<tr><td colspan="1" valign="top"><b>Global Alternate Flow</b></td><td colspan="1" valign="top">GA1</td><td colspan="2">If a technical error occurs during the execution of any action (e.g., database failure, server issues), the system displays an error message and logs the incident.</td></tr>
</table>



<table><tr><th colspan="1"><b>UCID</b></th><th colspan="3">UC#11</th></tr>
<tr><td colspan="1" valign="top"><b>Use case Name</b></td><td colspan="3" valign="top">update_pathologist_schedule</td></tr>
<tr><td colspan="1" valign="top"><b>Description</b></td><td colspan="3" valign="top">The "Update Pathologist Schedule"use case allows the compounder to update pathologist schedules in PHC through the Fusion portal.</td></tr>
<tr><td colspan="1" valign="top"><b>Actor</b></td><td colspan="3" valign="top"><b>Compounder</b></td></tr>
<tr><td colspan="1" valign="top"><b>Precondition</b></td><td colspan="3" valign="top">The Compounder is logged in into the system.</td></tr>
<tr><td colspan="1" rowspan="3" valign="top"><b>Main Flow</b></td><td colspan="1" valign="top">1</td><td colspan="2" valign="top">The Compounder navigates to the "Update Pathologist Schedule" section.</td></tr>
<tr><td colspan="1" valign="top">2</td><td colspan="2" valign="top">The system displays a list of pathologist schedules.</td></tr>
<tr><td colspan="1" valign="top">3</td><td colspan="2" valign="top">The compounder updates pathologist schedules accordingly.</td></tr>
<tr><td colspan="1" valign="top"><b>Post conditions</b></td><td colspan="3" valign="top">The updated pathologist schedule information is reflected in the database.</td></tr>
<tr><td colspan="1" valign="top"><b>Alternate Flow</b></td><td colspan="1" valign="top">A1</td><td colspan="1" valign="top">1</td><td colspan="1"><p>No pathologist is available so compounder not update any schedule,</p><p>Only reviewed it.</p></td></tr>
<tr><td colspan="1"><b>Sub Flow</b></td><td colspan="3">NIL</td></tr>
<tr><td colspan="1" valign="top"><b>Global Alternate Flow</b></td><td colspan="1" valign="top">GA1</td><td colspan="2">If a technical error occurs during the execution of any action (e.g., database failure, server issues), the system displays an error message and logs the incident.</td></tr>
</table>



<table><tr><th colspan="1"><b>UCID</b></th><th colspan="2">UC#12</th></tr>
<tr><td colspan="1"><b>Use case Name</b></td><td colspan="2">make_announcements</td></tr>
<tr><td colspan="1" valign="top"><b>Description</b></td><td colspan="2">The "make_announcement"use case allows patient to see the latest announcement made on the Fusion portal by the compounder.</td></tr>
<tr><td colspan="1"><b>Actor</b></td><td colspan="2"><b>Compounder</b></td></tr>
<tr><td colspan="1"><b>Precondition</b></td><td colspan="2">The compounder is logged in into the system.</td></tr>
<tr><td colspan="1" rowspan="2" valign="top"><b>Main Flow</b></td><td colspan="1">1</td><td colspan="1">The compounder navigates to the "Announcement"section.</td></tr>
<tr><td colspan="1">2</td><td colspan="1">The patient makes the latest announcements.</td></tr>
<tr><td colspan="1" valign="top"><b>Global Alternate Flow</b></td><td colspan="1" valign="top">GA1</td><td colspan="1">If a technical error occurs during the execution of any action (e.g., database failure, server issues), the system displays an error message and logs the incident.</td></tr>
</table>



<table><tr><th colspan="1"><b>UCID</b></th><th colspan="2">UC#13</th></tr>
<tr><td colspan="1"><b>Use case Name</b></td><td colspan="2">generate_report</td></tr>
<tr><td colspan="1" valign="top"><b>Description</b></td><td colspan="2" valign="top">The "generate_report"use case allows the compounder to generate a medical report of a patient on the Fusion portal by the compounder.</td></tr>
<tr><td colspan="1" valign="top"><b>Actor</b></td><td colspan="2" valign="top"><b>Compounder</b></td></tr>
<tr><td colspan="1"><b>Precondition</b></td><td colspan="2">The compounder is logged in into the system.</td></tr>
<tr><td colspan="1" rowspan="4" valign="top"><b>Main Flow</b></td><td colspan="1">1</td><td colspan="1">The compounder navigates to the health records of a patient.</td></tr>
<tr><td colspan="1" valign="top">2</td><td colspan="1" valign="top">The compounder navigates to generate report.</td></tr>
<tr><td colspan="1" valign="top">3</td><td colspan="1" valign="top">The compounder fills the required details.</td></tr>
<tr><td colspan="1" valign="top">4</td><td colspan="1" valign="top">Submit the form.</td></tr>
<tr><td colspan="1" valign="top"><b>Global Alternate Flow</b></td><td colspan="1" valign="top">GA1</td><td colspan="1" valign="top">If a technical error occurs during the execution of any action (e.g., database failure, server issues), the system displays an error message and logs the incident.</td></tr>
</table>

6. **UserInterfaces**

The user interface should comply with the colour scheming and dashboard design of the FUSION\_IIIT. Users should be able to navigate from one functionality to another. Inter module navigation should be smooth. All the functionalities should be easy to use and no specific training should be required for the usage of the module

7. **Tech Stack Used**
- Flutter
- Dart
- VS Code
- Android Studio
4  **Non- Functional Requirements**
1. **Performance:** The system should respond to user interactions quickly. Response time for booking actions, inventory updates, and notifications should be less.
1. **Scalability:** The system should handle a mass of concurrent users. System performance should be evaluated under increasing load conditions.
1. **Availability:** The system should be available 99.9%of the time.
1. **Security:** Ensure data confidentiality and integrity. Role-based authorization ensures that users can only perform actions relevant to their designated roles.

   5  **Module dependencies with other fusion modules**
1. **UILevel Dependency**

   Users log in to the Fusion application and are presented with the main dashboard. The user (student, employees) can track his/her health records. The employees can also view the health records of their dependencies.

2. **DB Level Dependencies**

   Following are the tables and their respective dependencies.



<table><tr><th colspan="1" valign="top"><b>S.no.</b></th><th colspan="1" valign="top"><b>Table Name</b></th><th colspan="1" valign="top"><b>Foreign Key</b></th><th colspan="1" valign="top"><b>Reference Table</b></th></tr>
<tr><td colspan="1" rowspan="3" valign="top">1</td><td colspan="1" rowspan="3" valign="top">health_center_appointment</td><td colspan="1">user_id</td><td colspan="1">globals_extrainfo</td></tr>
<tr><td colspan="1" valign="top">doctor_id</td><td colspan="1" valign="top">health_center_doctor</td></tr>
<tr><td colspan="1" valign="top">schedule_id</td><td colspan="1" valign="top">health_center_schedule</td></tr>
<tr><td colspan="1" valign="top">2</td><td colspan="1" valign="top">health_center_ambulance_request</td><td colspan="1" valign="top">user_id</td><td colspan="1" valign="top">globals_extrainfo</td></tr>
<tr><td colspan="1" valign="top">3</td><td colspan="1" valign="top">health_center_complaint</td><td colspan="1" valign="top">user_id</td><td colspan="1" valign="top">globals_extrainfo</td></tr>
<tr><td colspan="1">4</td><td colspan="1">health_center_expiry</td><td colspan="1">medicine_id</td><td colspan="1">health_center_medicine</td></tr>
<tr><td colspan="1" rowspan="3" valign="top">5</td><td colspan="1" rowspan="3" valign="top">health_center_hospital_admit</td><td colspan="1">doctor_id</td><td colspan="1">health_center_doctor</td></tr>
<tr><td colspan="1">hospital_name_id</td><td colspan="1">health_center_hospital</td></tr>
<tr><td colspan="1">user_id</td><td colspan="1">globals_extrainfo</td></tr>
</table>



<table><tr><th colspan="1" rowspan="2" valign="top">6</th><th colspan="1" rowspan="2" valign="top">health_center_medicine</th><th colspan="1" valign="top">medicine_id</th><th colspan="1" valign="top">health_center_stock</th></tr>
<tr><td colspan="1">patient_id</td><td colspan="1">globals_extrainfo</td></tr>
<tr><td colspan="1" rowspan="2" valign="top">7</td><td colspan="1" rowspan="2" valign="top">health_center_prescribed_medicine</td><td colspan="1">medicine_id</td><td colspan="1">health_center_stock</td></tr>
<tr><td colspan="1">prescription_id</td><td colspan="1">health_center_prescription</td></tr>
<tr><td colspan="1" rowspan="3" valign="top">8</td><td colspan="1" rowspan="3" valign="top">health_center_prescription</td><td colspan="1" valign="top">appointment_id</td><td colspan="1" valign="top">health_center_appointment</td></tr>
<tr><td colspan="1" valign="top">doctor_id</td><td colspan="1" valign="top">health_center_doctor</td></tr>
<tr><td colspan="1" valign="top">user_id</td><td colspan="1" valign="top">globals_extrainfo</td></tr>
<tr><td colspan="1" valign="top">9</td><td colspan="1" valign="top">health_center_schedule</td><td colspan="1" valign="top">doctor_id</td><td colspan="1" valign="top">health_center_doctor</td></tr>
</table>

3. **Module Level Dependencies**
- FTS (File Tracking System)
  - To keep track of the files/documents under process when a compounder forwards a medical reimbursement form.
- HR
  - To get the data of students and employees.
- Notifications
  - To trigger notification to the patient for any new announcement.
- Dashboard

○ To provide a unified and real-time interface for monitoring and tracking

health records.
