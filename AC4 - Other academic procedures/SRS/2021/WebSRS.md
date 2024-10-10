# Software Requirements Specification for AC-4-OTHER ACADEMIC PROCEDURES (WEB)

## PREPARED BY:
1) KUSHAL SHIVHARE (21BCS122)  
2) KAUSHAL KUMAR SAHANI (21BCS112)  
3) GAURAV YADAV (21BCS087)  
4) JATIN SINGH (21BCS105)  
5) KARAN (21BCS108)  

**LEAD:** Rameshwar Jagdish Paryani (21BCS171)

**MENTOR:** Dr. Ayan Seal

---

## 1. Introduction

#### 1.1 Introduction about the Fusion – A brief Description
FusionIIIT stands as a testament to the seamless integration and automation of diverse functions within PDPM Indian Institute of Information Technology, Design and Manufacturing, Jabalpur. Crafted with precision using Python 3.8 and powered by the Django Web framework, this initiative is a student-driven endeavor designed to elevate the institute's operational landscape. Encompassing everything from efficient administration management to academic prowess and miscellaneous departmental tasks, FusionIIIT is a holistic solution that harmonizes the intricacies of campus life.  
Imagine it as a digital wizard that takes care of everything, from organizing the administrative stuff to making academics smoother. It's not just limited to the usual tasks; FusionIIIT jumps into various departments and sections, making sure every corner of campus life runs smoothly.  
In the admin side, it handles the complicated paperwork and processes. For academics, it brings a digital touch, making learning and managing courses easier. But it doesn't stop there; FusionIIIT is like a friendly companion for all the different parts of the campus, making sure everything works well.  
In simpler terms, FusionIIIT is not just a tool – it's a helpful friend, making life at PDPM IIITDM Jabalpur more organized and enjoyable for everyone.

#### 1.2 Purpose of the module
The aim of the document is to gather and analyse and give an in-depth insight of the Academic Procedures of IIITDM Jabalpur which includes Leave Bonafide, and No-dues. It will define the users and functionality of the Software.  
Also, we shall predict and sort out how we hope this product will be used in order to gain a better understanding of the Software, outline concepts that may be developed later, and document ideas that are being considered, but may be discarded as the product develops. This document describes the project's target audience and its user interface, hardware and software requirements. It defines how our client, team and audience see the product and its functionality. Nonetheless, it helps any designer and developer to assist in Software Development Lifecycle (SDLC) processes.

#### 1.3 Scope of the module
The Software System will be Academic Procedures Web Services Portal to make various activities of the academic office easy to process and fast. Accessing the information and performing the activities will be easy using the Software.  
Software will facilitate various activities of the academic procedures at one place.

---

## 2. User/Actor Characteristics

#### 2.1 STUDENT
Represents individuals who intend to do their academic procedures such as filling of leave form, filling of bonafide form, checking the status of their no dues etc.  
**Role:** student (UG + PG) role is to make use of this portal to fulfil his academic procedures through this platform.  
**Specific Functionalities:**
- Checking of no_dues_status.
- Filling the leave_form.
- Filling the bonafide_form.
<br>

#### 2.2 PG STUDENTS
PG Students can access all the functionalities of Student but they also come through some special features such as looking for their status of graduate seminar and assistantship claim status.  
**Role:** PG students role is to make sure that they effectively make use of this portal to check their graduate_seminar_status and check their assistantship_claim_status.  
**Specific Functionalities:**
- Check_graduate_seminar_status.
- Check_Assistantship_claim_status.
<br>

#### 2.3 HOD
HOD is the head of the department of all the students (UG + PG) and faculty of that same department.  
**Role:** The role of HOD is to make sure that he checks all the leave requests and then grants or rejects them and to sign the assistantship claim form.  
**Specific Functionalities:**
- To check all the leave requests.
- To approve or rejects the leave requests.
- To sign assistantship claim form of PG students.
<br>

#### 2.4 ACAD ADMIN
Acad Admin is the administrative personnel and is responsible for managing all the academic affairs.  
**Role:** The role of Acad Admin is to verify the bonafide application and give assistantship to PG students and to make sure to update the no_dues status.  
**Specific Functionalities:**
- To verify the bonafide applications of students.
- To give assistantship to PhD and PG students.
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
Library (Librarian) is the incharge of the library and manages all the records and data of the library.  
**Role:** The role of library is to make sure that it releases the no_dues form of all the applicable students.  
**Specific Functionalities:**
- To generate the no_dues form.
<br>

#### 2.7 HOSTEL WARDEN
Hostel (Hostel warden or hostel caretaker) is the incharge of the hostel and is responsible for all the students staying in that particular hostel and to keep and maintain the record of every students of that hostel.  
**Role:** The role of hostel is to make sure that it releases the no_dues form of all the applicable students.  
**Specific Functionalities:**
- To generate the no_dues form.
<br>

#### 2.8 TA SUPERVISOR
TA Supervisor is the one who manages all the TA’s and is responsible to distribute works to the TA’s.  
**Role:** The role of TA Supervisor is to approve or reject the assistantship claim form of the PG students.  
**Specific Functionalities:**
- To approve assistantship_claim_form.
<br>

#### 2.9 THESIS SUPERVISOR
Thesis Supervisor is the one who supervises the thesis of PG students.  
**Role:** The role of Thesis Supervisor is to approve or reject the assistantship claim form of the PG students.  
**Specific Functionalities:**
- To approve assistantship_claim_form.
<br>

#### 2.10 LAB INCHARGE
Lab incharge includes all the labs incharge actors (VLSI, ECE, signal processing lab, workshop, CC, mechatronics lab, physics lab), that will verify no dues of student in their specific lab.  
**Role:** The role of the lab incharge is to verify the no dues of student of specific lab.  
**Specific Functionalities:**
- To verify no dues.
<br>

#### 2.11 DESIGN INCHARGE
Design incharge includes Design studio and Design Project actor in it, who will verify the no dues of students.  
**Role:** The role of the Design incharge is to verify the no dues of student of specific design discipline related no dues.  
**Specific Functionalities:**
- To release and update no dues form.
<br>

#### 2.12 OFFICE INCHARGE
Office incharge is the incharge of all the offices like Gymkhana, placement cell, alumni, discipline office, BTP supervisor, bank, account, and manages all the records and data of the all the offices.  
**Role:** The role of the Office incharge is to verify the no_dues form of all the students and proceed it for other work.  
**Specific Functionalities:**
- To verify no dues form.
<br>

#### 2.13 MESS INCHARGE
Mess incharge is the incharge of dealing with the mess-related work that includes accounting of Mess.  
**Role:** Mess incharge will check the database of each student and verify the no dues of student of mess.  
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

---


### 3.3. Other Functional Requirements  
we can send notifications or email to the respective students when his/her request had been accepted.

### 3.4 Other constraints  
#### 3.4.1 User Interfaces  
The user interface should comply with the colour scheming and dashboard design of the FUSIONIIT. Users should be able to navigate from one functionality to other. Inter module navigation should be smooth. All the functionalities should be easy to use and no specific training should be required for the usage of the module.

#### 3.4.2 Tech Stack Used  
we are using:  
- Django  
- Postgresql DB.

---

### 4. Non- Functional Requirements  
#### 4.1 Performance:  
The system should respond to user interactions quickly. Response time for booking actions, inventory updates, and notifications should be less.

#### 4.2 Scalability:  
The system should handle a mass of concurrent users. System performance should be evaluated under increasing load conditions.

#### 4.3 Availability:  
The system should be available 99.9% of the time.

#### 4.4 Security:  
Ensure data confidentiality and integrity. Role-based authorization ensures that users can only perform actions relevant to their designated roles.

---

### 5. Module dependencies with other fusion modules  
#### 5.1. UI Level  
when the students will submit any application regarding leave or affidavait or assistantship status etc then the HOD or dept admin and acad admin can view them through their logging in with their credentials and can approve or reject their requests. And after that the students go to their portal and see if their requests had been approved or not.

#### 5.2 DB Level Dependencies  
DB tables that other academic procedures module depends on is:  
- Students  
- HOD  
- Acad Admin  
- Dept Admin.
