# Software Requirements Specification for AC4 - Other Academic Procedures(App)

### Prepared by:
- Ashish kol (21BCS041)
- Bikash Sabar (21BCS060)
- Gadam Omkar (21BCS083)
- Gaurav Singh (21BCS086)
- Shivam Kumar (21BCS191)

**LEAD:** Prakash Dwivedi (21BCS159)

**MENTOR:** Dr. Ayan Seal

---

## 1. Introduction

### 1.1 Introduction about the Fusion – A brief Description

FusionIIIT stands as a testament to the seamless integration and automation of diverse functions within PDPM Indian Institute of Information Technology, Design and Manufacturing, Jabalpur. Crafted with precision using Python 3.8 and powered by the Django Web framework, this initiative is a student-driven endeavor designed to elevate the institute's operational landscape. Encompassing everything from efficient administration management to academic prowess and miscellaneous departmental tasks, FusionIIIT is a holistic solution that harmonizes the intricacies of campus life.

Imagine it as a digital wizard that takes care of everything, from organizing the administrative stuff to making academics smoother. It's not just limited to the usual tasks; FusionIIIT jumps into various departments and sections, making sure every corner of campus life runs smoothly.

In the admin side, it handles the complicated paperwork and processes. For academics, it brings a digital touch, making learning and managing courses easier. But it doesn't stop there; FusionIIIT is like a friendly companion for all the different parts of the campus, making sure everything works well.

In simpler terms, FusionIIIT is not just a tool – it's a helpful friend, making life at PDPM IIITDM Jabalpur more organized and enjoyable for everyone.

### 1.2 Purpose of the module:

This document aims to comprehensively gather, analyze, and provide insight into the Academic Procedures of IIITDM Jabalpur. These procedures encompass the processing of Leave forms, Bonafide forms, Graduate seminar status, Assistantship claim status, and No-dues. The document will define the users and functionality of the Software.

Furthermore, it seeks to predict and address how we anticipate the product's utilization, aiming to gain a better understanding of the Software's intended use. The document will outline concepts that may be developed later and document ideas that are under consideration but may be discarded as the product evolves.

This comprehensive document not only describes the project's target audience, user interface, and hardware/software requirements but also defines how our clients, team, and audience perceive the product and its functionality. It serves as a valuable guide for designers and developers, assisting in the Software Development Lifecycle (SDLC) processes.

### 1.3 Scope of the module:

The Academic Procedures system is an integral subsystem within the broader College System. The software is designed to retrieve input from the College Database, which stores information about both students and faculty. The system involves four distinct actors: Students, Heads of Department (HODs), Assistant, and Department admin. Each actor is assigned specific activities within the system, ensuring a distributed and specialized approach to task execution. This delineation of responsibilities contributes to the system's efficiency and effectiveness in managing academic procedures.

---

## 2. User/Actor Characteristics

#### 2.1 STUDENT
Represents individuals who intend to do their academic procedures such as filling of leave form, filling of bonafide form, checking the status of their no dues, etc.  
**Role:** The student's (UG + PG) role is to make use of this portal to fulfill his academic procedures through this platform.  
**Specific Functionalities:**
- Checking of no_dues_status.
- Filling the leave_form.
- Filling the bonafide_form.
<br>

#### 2.2 PG STUDENTS:
PG Students can access all the functionalities of Student but they also come through some special features such as looking for their status of graduate seminar and assistantship claim status.  
**Role:** PG students' role is to make sure that they effectively make use of this portal to check their graduate_seminar_status and check their assistantship_claim_status.  
**Specific Functionalities:**
- Check_graduate_seminar_status.
- Check_Assistantship_claim_status.
<br>

#### 2.3 HOD

HOD is the head of the department of all the students (UG + PG) and faculty of that same department.  
**Role:** The role of the HOD is to make sure that he checks all the leave requests and then grants or rejects them and to sign the assistantship claim form.  
**Specific Functionalities:**
- To check all the leave requests.
- To approve or reject the leave requests.
- To sign the assistantship claim form of PG students.
<br>

#### 2.4 ACAD ADMIN

Acad Admin is the administrative personnel and is responsible for managing all the academic affairs.  
**Role:** The role of Acad Admin is to verify the bonafide application and give assistantship to PG students and to make sure to update the no_dues status.  
**Specific Functionalities:**
- To verify the bonafide applications of students.
- To give assistantship to PHD and PG students.
- To update the no_dues status.
<br>

#### 2.5 Dept-Admin

Department Admin refers to the administrative personnel responsible for managing the day-to-day operations of a specific department in an organization or institution.  
**Role:** The role of Dept-Admin is to log assistantship and seminar status of PG students.  
**Specific Functionalities:**
- Log_graduate_seminar_data.
- Log_Assistantship_claim_data.
<br>

#### 2.6 LIBRARIAN

The Librarian is the in-charge of the library and manages all the records and data of the library.  
**Role:** The role of the library is to make sure that it releases the no_dues form of all the applicable students.  
**Specific Functionalities:**
- To generate the no_dues form.
<br>

#### 2.7 HOSTEL WARDEN

The Hostel Warden (or hostel caretaker) is the in-charge of the hostel and is responsible for all the students staying in that particular hostel and for maintaining the record of every student in the hostel.  
**Role:** The role of the hostel is to make sure that it releases the no_dues form of all the applicable students.  
**Specific Functionalities:**
- To generate the no_dues form.
<br>

#### 2.8 TA SUPERVISOR

The TA Supervisor is the one who manages all the TA's and is responsible for distributing work to the TA's.  
**Role:** The role of the TA Supervisor is to approve or reject the assistantship claim form of the PG students.  
**Specific Functionalities:**
- To approve assistantship_claim_form.
<br>

#### 2.9 THESIS SUPERVISOR

The Thesis Supervisor is the one who supervises the thesis of PG students.  
**Role:** The role of the Thesis Supervisor is to approve or reject the assistantship claim form of the PG students.  
**Specific Functionalities:**
- To approve assistantship_claim_form.
<br>

#### 2.10 LAB INCHARGE

Lab Incharge includes all the lab in-charge actors (VLSI, ECE, signal processing lab, workshop, CC, mechatronics lab, physics lab) that will verify the no dues of students in their specific lab.  
**Role:** The role of the lab in-charge is to verify the no dues of students in their specific lab.  
**Specific Functionalities:**
- To verify no dues.
<br>

#### 2.11 DESIGN INCHARGE

Design In-charge includes the Design studio and Design Project actors, who will verify the no dues of students.  
**Role:** The role of the Design In-charge is to verify the no dues of students related to the specific design discipline.  
**Specific Functionalities:**
- To release and update no dues form.
<br>

#### 2.12 OFFICE INCHARGE

The Office In-charge is responsible for managing all the offices like Gymkhana, placement cell, Alumni, Discipline office, BTP supervisor, Bank, Account, and managing all the records and data of the offices.  
**Role:** The role of the Office In-charge is to verify the no_dues form of all the students and proceed with other work.  
**Specific Functionalities:**
- To verify no dues form.
<br>

#### 2.13 MESS INCHARGE

The Mess In-charge deals with mess-related work, including accounting for the Mess.  
**Role:** The Mess In-charge will check the database of each student and verify the no dues of students in the mess.  
**Specific Functionalities:**
- To verify no dues form.

---

## 3. Functional Requirements

### 3.1 Use Case Diagram
![Diagram Image](../../Diagrams/OAD%20V2.png)


### 3.2 Use Case 

| UC ID  | UC#1 |
|--------|------|
| **Use Case Name** | fill_leave_form |
| **Description** | Filling leave application form |
| **Actor** | Students |
| **Precondition** | Balance leaves left or Medical certificate or any supporting document. |
| **Main Flow** | 1. Application should be filled with appropriate document if any (optional). <br> 2. Application is forwarded to the HOD. |
| **Postcondition** | Application is submitted and forwarded to the HOD. |

---

| UC ID  | UC#2 |
|--------|------|
| **Use Case Name** | approve/reject_leave_request |
| **Description** | Permit leave or reject leave to the student |
| **Actor** | HOD |
| **Precondition** | HOD should be logged in on the website |
| **Main Flow** | 1. Approve the leave request. <br> 2. Status of leave application gets updated. |
| **Postcondition** | Leave is granted to the student. |
| **Alternate Flow** | Leave is not granted to the student. |

---
| UC ID  | UC#3 |
|--------|------|
| **Use Case Name** | upload_document |
| **Description** | It is optional to upload a document during filling the leave form. |
| **Actor** | Students |
| **Main Flow** | 1. Student can upload a supporting document during form filling. |
| **Postcondition** | HOD will check the reason and either grant or not grant the leave. |
---
| UC ID  | UC#4 |
|--------|------|
| **Use Case Name** | fill_bonafide_form |
| **Description** | Filling the Bonafide form |
| **Actor** | Students |
| **Precondition** | Purpose for bonafide |
| **Main Flow** | 1. Fill the form <br> 2. Submit the form <br> 3. Forward to the Acad Admin. |
| **Postcondition** | Received by the Acad Admin. |

---
| UC ID  | UC#5 |
|--------|------|
| **Use Case Name** | verify_bonafide |
| **Description** | Approve the bonafide request |
| **Actor** | Acad Admin |
| **Precondition** | Bonafide request |
| **Main Flow** | 1. The Acad admin checks the bonafide request. <br> 2. Acad admin can approve or reject the request. |
| **Postcondition** | Students can check the status of their request. |

---
| UC ID  | UC#6 |
|--------|------|
| **Use Case Name** | check_graduate_seminar_status |
| **Description** | To check the graduate seminar schedule |
| **Actor** | PG students |
| **Precondition** | Graduate seminar status must be logged or updated. |
| **Main Flow** | 1. Students can view the schedule of their seminar. |
| **Postcondition** | N/A |

---
| UC ID  | UC#7 |
|--------|------|
| **Use Case Name** | check_assistantship_claim_status |
| **Description** | For getting the stipend |
| **Actor** | PG Student |
| **Precondition** | Must be a PG Student |
| **Main Flow** | 1. Fill the form <br> 2. Submit to the department admin office. |
| **Postcondition** | 1. Accepted by Department Admin office <br> 2. Notified to PG student. |

---
| UC ID  | UC#8 |
|--------|------|
| **Use Case Name** | log_assistantship_claim_data |
| **Description** | Department Admin office generates the form |
| **Actor** | Department Admin |
| **Precondition** | Department Admin should be logged in to the page |
| **Main Flow** | 1. Generate the Assistant Claim Form. <br> 2. Allot student to their TA supervisor and Thesis supervisor. |
| **Postcondition** | Form gets to TA supervisor and Thesis Supervisor for approval. |
| **Alternate Flow** | In case of incomplete details, notify the student. |

---
| UC ID  | UC#9 |
|--------|------|
| **Use Case Name** | update_no_dues_status |
| **Description** | Acad Admin will update the no dues of the student. |
| **Actor** | Acad Admin |
| **Precondition** | NoDues status of student must be present. |
| **Main Flow** | 1. Acad Admin will check the no dues of the student. <br> 2. Update no dues after the student clears it. |
| **Postcondition** | Student will be able to see NoDues Status. |

---
| UC ID  | UC#10 |
|--------|------|
| **Use Case Name** | check_no_dues_status |
| **Description** | Check NoDues Status |
| **Actor** | Student |
| **Precondition** | NoDues status should be present. |
| **Main Flow** | 1. Students can check their status of NoDues. <br> 2. Once all dues are cleared, the student can download the NoDues approval. |
| **Postcondition** | 1. Student will be able to see NoDues Status. <br> 2. Student will be able to download the NoDues approval. |
| **Alternate Flow** | If not all dues are cleared, students can’t download NoDues approval. |

---
| UC ID  | UC#11 |
|--------|------|
| **Use Case Name** | log_graduate_seminar_data |
| **Description** | Dept admin updates or logs the schedule of the graduate seminar. |
| **Actor** | Department Admin |
| **Main Flow** | 1. Department Admin updates or logs the schedule for the seminar. |
| **Postcondition** | Students can view the graduate seminar schedule. |

---
| UC ID  | UC#12 |
|--------|------|
| **Use Case Name** | Assistant Claim Form (TA Supervisor) |
| **Description** | TA supervisor approves the assistant claim of the student. |
| **Actor** | TA supervisor |
| **Precondition** | 1. TA supervisor should be logged in to the website. <br> 2. Form should be filled by the student. |
| **Main Flow** | a) Check the assistantship form of the student. <br> b) Verify the details provided by the student. <br> c) Approve/Reject the assistant claim form of the student. |
| **Postcondition** | After approval, the form will go to the Thesis Supervisor for approval. |
| **Alternate Flow** | In case of incomplete details, notify the student. |

---
| UC ID  | UC#13 |
|--------|------|
| **Use Case Name** | Assistant Claim Form (Thesis Supervisor) |
| **Description** | Thesis supervisor approves the assistant claim of the student. |
| **Actor** | Thesis supervisor |
| **Precondition** | 1. Thesis supervisor should be logged in to the website. <br> 2. Form should be approved by the TA Supervisor. |
| **Main Flow** | a) Check the assistantship form of the student. <br> b) Verify the details provided by the student. <br> c) Approve/Reject the assistant claim form of the student. |
| **Postcondition** | After approval, the form will go to the HoD for signature. |
| **Alternate Flow** | In case of incomplete details, notify the student. |

---
| UC ID  | UC#14 |
|--------|------|
| **Use Case Name** | Sign Assistant Claim Form |
| **Description** | HOD will sign the Assistant claim Form. |
| **Actor** | HOD |
| **Precondition** | 1. HOD should be logged in to the page. <br> 2. Assistant claim should be approved by the TA and Thesis supervisors. |
| **Main Flow** | 1. HOD will check the Assistant claim Form. <br> 2. Sign the Assistant Claim Form. |
| **Postcondition** | Details of the student get shared with Acad Admin for stipend processing. |
| **Alternate Flow** | In case of incomplete details, notify the student. |

---
| UC ID  | UC#15 |
|--------|------|
| **Use Case Name** | Give Assistantship |
| **Description** | Acad Admin gives stipend to allotted student. |
| **Actor** | Acad Admin |
| **Precondition** | 1. Acad Admin should be logged in to the website. <br> 2. Assistant claim form should be signed by HOD. |
| **Main Flow** | 1. Acad Admin checks the bank details of the student. <br> 2. Acad Admin gives stipend to the allotted student. |
| **Postcondition** | Student will receive the stipend and approval. |
| **Alternate Flow** | In case of incomplete details, notify the student. |

---
| UC ID  | UC#16 |
|--------|------|
| **Use Case Name** | Verify No Dues (Library) |
| **Description** | Verify no dues to the student. |
| **Actor** | Librarian |
| **Precondition** | Librarian should be logged into the portal. |
| **Main Flow** | 1. Check clear if no dues of the student are clear in the library database. <br> 2. Check not clear if no dues of the student are not clear in the library database. |
| **Postcondition** | Student can view their no dues through the website. |
| **Alternate Flow** | If no dues are not clear, the student has to follow the library protocol to clear the dues. |

---
| UC ID  | UC#17 |
|--------|------|
| **Use Case Name** | Verify No Dues (Hostel) |
| **Description** | Verify no dues to the student. |
| **Actor** | Hostel Warden or Hostel Caretaker |
| **Precondition** | Hostel Warden or Hostel Caretaker should be logged into the portal. |
| **Main Flow** | 1. Check clear if no dues of the student are clear in the hostel database. <br> 2. Check not clear if no dues of the student are not clear in the hostel database. |
| **Postcondition** | Student can view their no dues through the website. |
| **Alternate Flow** | If no dues are not clear, the student has to follow the hostel protocol to clear the dues. |

---
| UC ID  | UC#18 |
|--------|------|
| **Use Case Name** | Verify No Dues (Mess) |
| **Description** | Verify no dues to the student. |
| **Actor** | Mess Incharge |
| **Precondition** | Mess Incharge should be logged into the portal. |
| **Main Flow** | 1. Check clear if no dues of the student are clear in the mess database. <br> 2. Check not clear if no dues of the student are not clear in the mess database. |
| **Postcondition** | Student can view their no dues through the website. |
| **Alternate Flow** | If no dues are not clear, the student has to follow the mess protocol to clear the dues. |

---
| UC ID  | UC#19 |
|--------|------|
| **Use Case Name** | Verify No Dues (Lab) |
| **Description** | Verify no dues to the student. |
| **Actor** | Lab Incharge |
| **Precondition** | Lab Incharge should be logged into the portal. |
| **Main Flow** | 1. Check clear if no dues of the student are clear in the specified authority's database. <br> 2. Check not clear if no dues of the student are not clear in the specified authority's database. |
| **Postcondition** | Student can view their no dues through the website. |
| **Alternate Flow** | If no dues are not clear, the student has to follow the lab protocol to clear the dues. |

---
| UC ID  | UC#20 |
|--------|------|
| **Use Case Name** | Verify No Dues (Office) |
| **Description** | Verify no dues to the student. |
| **Actor** | Office Incharge |
| **Precondition** | Office Incharge should be logged into the portal. |
| **Main Flow** | 1. Check clear if no dues of the student are clear in the office database. <br> 2. Check not clear if no dues of the student are not clear in the office database. |
| **Postcondition** | Student can view their no dues through the website. |
| **Alternate Flow** | If no dues are not clear, the student has to follow the office protocol to clear the dues. |

---
| UC ID  | UC#21 |
|--------|------|
| **Use Case Name** | Verify No Dues (Design Office) |
| **Description** | Verify no dues to the student. |
| **Actor** | Design Incharge |
| **Precondition** | Design Incharge should be logged into the portal. |
| **Main Flow** | 1. Check clear if no dues of the student are clear in the design office database. <br> 2. Check not clear if no dues of the student are not clear in the design office database. |
| **Postcondition** | Student can view their no dues through the website. |
| **Alternate Flow** | If no dues are not clear, the student has to follow the design office protocol to clear the dues. |


### 3.3 Other Functional Requirements:

• **Notification and Communication:**  
  The module will integrate with the communication system to send notifications and alerts to stakeholders involved in academic procedures. Notifications include updates on form submissions, approvals, and other relevant information. Automated email or SMS notifications will be generated for various academic processes, including Leave form approvals, Bonafide certificate issuances, No-dues clearance status, Graduate seminar participation, and assistantship claim status.

• **Alerts and Updates:**  
  The system will provide alerts for critical events, such as approaching deadlines for form submissions, changes in academic schedules, and important updates related to academic procedures. Notifications will be sent to relevant actors, including students, assistants, HODs, and department administrators.

• **Role Assignment:**  
  The Super admin of the academic system should have the ability to assign roles and permissions for academic administrative roles, such as HODs, assistants, and department administrators.

• **Offline Processes:**  
  The system should be capable of handling offline academic processes, allowing for the submission of physical forms or documentation when necessary.

• **Category Conversion:**  
  The system may allow for the conversion of student categories (e.g., from undergraduate to postgraduate) subject to approval from the competent authority. This functionality ensures flexibility in managing academic transitions.

• **Tariff and Fee Changes:**  
  Changes in academic fees, such as tuition or examination fees, may be possible over time and will be subject to decisions made by the institute authorities. The system should be able to accommodate and reflect these changes accurately.

  These functional requirements contribute to the efficiency, flexibility, and adaptability of the Academic Procedures module, ensuring seamless communication, timely notifications, and the ability to handle various academic scenarios.

### 3.4 Other Constraints:

#### 3.4.1 User Interfaces:
The user interface should align with the established color scheme and dashboard design of the institution's overarching academic management system. Consistency in design elements ensures a cohesive user experience.  
Users should experience smooth navigation between different functionalities within the module. Inter-module navigation should be intuitive and seamless.  
All functionalities within the Academic Procedures module should be user-friendly, requiring minimal training for users to navigate and perform tasks effectively.

#### 3.4.2 Tech Stack Used:
The development tech stack for mobile app components of the Academic Procedures module shall include Flutter, Dart, Android Studio, frameworks, and tools used. This ensures a standardized and efficient development process across platforms.

#### 3.4.3 Business Rules:

• **Academic Form Processing:**  
  The processing of academic forms, such as Leave forms, Bonafide requests, and No-dues clearances, shall adhere to existing rules and guidelines set by the institution. The system will enforce consistency in form processing based on these rules.

• **Graduate Seminar Participation:**  
  Rules for managing and participating in Graduate seminars will be outlined and enforced by the system. This includes guidelines for submission, approval, and documentation associated with seminar participation.

• **Assistantship Claims:**  
  The validation and approval of assistantship claims will follow established business rules, ensuring transparency and adherence to departmental policies.

• **Category-Based Procedures:**  
  Various academic procedures, including those related to student categories (e.g., undergraduate, postgraduate), shall be governed by specific business rules. This may include processes for category conversion and transition.

  These constraints provide guidance for the design, development, and operation of the Academic Procedures module, ensuring alignment with institutional standards and business rules.

---

## 4. Non-Functional Requirements

#### 4.1 Performance:
The system should respond to user interactions quickly. Response time for booking actions, inventory updates, and notifications should be less.

#### 4.2 Scalability:
The system should handle a mass of concurrent users. System performance should be evaluated under increasing load conditions.

#### 4.3 Availability:
The system should be available 99.9% of the time.

#### 4.4 Security:
Ensure data confidentiality and integrity. Role-based authorization ensures that users can only perform actions relevant to their designated roles.

---

## 5. Module dependencies with other fusion modules

#### 5.1. UI Level:
When the students will submit any application regarding leave or affidavit or assistantship status etc., then the HOD or dept admin and acad admin can view them through their logging in with their credentials and can approve or reject their requests. And after that the students go to their portal and see if their requests had been approved or not.

#### 5.2 DB Level Dependencies:
DB tables that other academic procedures module depends on is:

• Students  
• HOD  
• Acad Admin  
• Dept Admin.

