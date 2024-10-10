# FUSION ERP Software Requirements Specification for GAD-3-COMPLAINT MANAGEMENT (APP) 

**Prepared by:** Ananya Sharma (21BCS020), Armin Patel (21BCS031), Chahit Kolte (21BCS062), Harsh Chauhan (21BCS094), Harshith Sudar (21BCS097) 

**Student Mentor:** Hardik Pratap Singh (21BCS090) 
**Faculty Mentor:** Dr. Avinash Chandra Pandey 

## Table of Contents
1. [Introduction](#introduction)
   - [Introduction about the Fusion – A brief Description](#introduction-about-the-fusion-a-brief-description)
   - [Purpose of module](#purpose-of-module)
   - [Scope of module](#scope-of-module)
2. [User/Actor Characteristics](#useractor-characteristics)
3. [System Features (Functional Requirements)](#system-features-functional-requirements)
   - [Use Case Diagram](#use-case-diagram)
   - [Use Case Descriptions](#use-case-descriptions)
4. [Non-Functional Requirements](#non-functional-requirements)
5. [Dependencies](#dependencies)

## 1. Introduction 

### 1.1 Introduction about the Fusion – A brief Description 
FusionIIIT at PDPM Indian Institute of Information Technology, Design, and Manufacturing, Jabalpur, exemplifies the seamless integration and automation of diverse functions. Developed by students using Python 3.8 and powered by the Django Web framework, this initiative is a testament to the institute's commitment to improving operational efficiency and enriching campus life. In the administrative domain, FusionIIIT manages intricate paperwork and processes, simplifying administrative tasks for a more streamlined approach. On the academic side, it introduces a digital facet to learning and course management, enhancing the educational experience. However, its impact extends beyond the conventional, reaching various departments and sections to ensure the smooth operation of every aspect of campus life.

Visualize FusionIIIT as a digital wizard that not only organizes administrative processes and elevates academic experiences but also lends support to miscellaneous departmental tasks. It acts as a supportive companion, overseeing the seamless functioning of every facet of campus life.

Beyond being a mere tool, FusionIIIT emerges as a reliable friend dedicated to enhancing organization and enjoyment in the lives of everyone at PDPM IIITDM Jabalpur. 

### 1.2 Purpose of the module: 
The central complaint system is designed to efficiently manage and resolve issues pertaining to electricity, hostels, and cleanliness in each campus building. The primary goal of this software is to provide a swift and effective mechanism for addressing concerns raised by individuals within the campus community, ensuring a seamless resolution process. Additionally, it serves as a communication platform, facilitating a direct connection between users and the relevant Caretaker/Supervisor for each department.

### 1.3 Scope of the module: 
The complaint management system by offering a comprehensive and efficient platform for students to register their concerns. Beyond simple registration, the system facilitates real-time tracking and visibility of complaints for respective authorities.

## 2. User/Actor Characteristics 
### 2.1 Student / Faculty / Staff 
Individuals who would lodge the complaints. 
**Role:** Creation of complaint 

**Specific Functionalities:**  
- Lodge complaint through the Fusion portal 
- Specify details of the complaint 
- Choose the complaint category 
- Track Complaint status 
- Provide Feedback 

### 2.2 Admin / Section In-Charge 
Admin or Section In-Charge of the service. 
**Role:** Oversee the complaints, able to respond and change the status of complaints 

**Specific Functionalities:** 
- View Complaints 
- Respond to complaints 
- Change the status of complaints 
- Manage worker/caretaker 

### 2.3 Caretaker 
Caretaker of the particular service like internet, electricity. 
**Role:** View and resolve complaints, manage worker 

**Specific Functionalities:** 
- View Complaints 
- Respond to complaints 
- Assign worker 

## 3. System Features (Functional Requirements) 
### 3.1 Use Case Diagram 
![Use Case Diagram](images/Aspose.Words.1989d50c-b992-4d37-bf89-c72de2f30f4e.001.png)

### 3.2 Use Case Description 

#### **Use Case #1** 
| UC ID | UC #1 |
|-------|-------|
| Use Case Name | lodge_complaint |
| Description | Report issues to the concerning administration |
| Actor(s) | Staff, Student, Faculty |
| Pre-Condition | User must be logged in |
| Main Flow | 1) The user fills all the necessary columns and clicks on the submit button.<br>2) System Displays the message of the complaint being successfully received. |
| Post-Condition | The complaint is successfully received by the system and stored in the database. |
| Alternate Flow | If the User is not logged in, the system prompts them to log in. |
| Sub Flow | none |
| Global Alternate Flow | none |

#### **Use Case #2** 
| UC ID | UC #2 |
|-------|-------|
| Use Case Name | track_status |
| Description | Check the status of the complaint |
| Actor(s) | Staff, Student, Faculty |
| Pre-Condition | The user must have a complaint registered. |
| Main Flow | 1) User checks the complaint history for the status.<br>2) User checks his complaint whether it has been overlooked/resolved by the caretaker within a given timestamp or not. |
| Post-Condition | none |
| Alternate Flow | none |
| Sub Flow | none |
| Global Alternate Flow | none |

#### **Use Case #3** 
| UC ID | UC #3 |
|-------|-------|
| Use Case Name | give_feedback |
| Description | Rate resolution of the complaint |
| Actor(s) | Staff, Student, Faculty |
| Pre-Condition | User must have a complaint lodged |
| Main Flow | 1) The user selects the complaint they want to provide feedback on.<br>2) The user enters their feedback.<br>3) The system stores the feedback. |
| Post-Condition | none |
| Alternate Flow | none |
| Sub Flow | none |
| Global Alternate Flow | none |

#### **Use Case #4** 
| UC ID | UC #4 |
|-------|-------|
| Use Case Name | view_complaint |
| Description | View complaint details |
| Actor(s) | Caretaker |
| Pre-Condition | Caretaker must be logged in. |
| Main Flow | 1) Caretaker clicks on view complaints.<br>2) New page with all complaints and their complainter appears. |
| Post-Condition | Caretaker chooses a complaint to assign worker to it. |
| Alternate Flow | none |
| Sub Flow | none |
| Global Alternate Flow | none |

#### **Use Case #5** 
| UC ID | UC #5 |
|-------|-------|
| Use Case Name | forward/respond |
| Description | Forward the complaint to admin/section in charge. |
| Actor(s) | Caretaker |
| Pre-Condition | Caretaker cannot handle problem by himself. |
| Main Flow | 1) Caretaker forwards the complaint. |
| Post-Condition | Problem is to be managed by admin/section in charge. |
| Alternate Flow | none |
| Sub Flow | none |
| Global Alternate Flow | none |

#### **Use Case #6** 
| UC ID | UC #6 |
|-------|-------|
| Use Case Name | respond_to_complaint |
| Description | Respond/comment on the complaint by the administration |
| Actor(s) | Caretaker, admin |
| Pre-Condition | User is authorized to view the complaint |
| Main Flow | 1) Caretaker views the complaint.<br>2) Caretaker takes necessary action to resolve the complaint and responds accordingly. |
| Post-Condition | none |
| Alternate Flow | none |
| Sub Flow | none |
| Global Alternate Flow | none |

#### **Use Case #7** 
| UC ID | UC #7 |
|-------|-------|
| Use Case Name | change_status |
| Description | Update complaint status as needed |
| Actor(s) | Admin, caretaker |
| Pre-Condition | User is logged in with the role of admin or caretaker |
| Main Flow | 1) Selects a complaint.<br>2) Selects a new status for the complaint. |
| Post-Condition | System updates the complaint status. |
| Alternate Flow | none |
| Sub Flow | none |
| Global Alternate Flow | none |

## 4. Non-Functional Requirements 

1. **Performance:** 
   The system should respond to user interactions quickly. Response time for booking actions, inventory updates, and notifications should be less.

2. **Scalability:** 
   The system should handle a mass of concurrent users. System performance should be evaluated under increasing load conditions.

3. **Availability:** 
   The system should be available 99.9% of the time.

4. **Security:** 
   Ensure data confidentiality and integrity. Role-based authorization ensures users can only perform actions relevant to their designated roles.

## 5. Dependencies 

### 5.1 Integration at the UI Level: 
Users log into the Fusion application and land on the main dashboard. The user (student, staff, faculty, and other community members of IIITDMJ) can add a complaint by filling in the required input fields. Lodgers can also see the complaint status and history.

### 5.2 Integration at the Back-end Level: 
The API endpoints should manage user authentication and serve data regarding complaints. Data should be stored in a robust and efficient database system, ensuring that information retrieval is optimized.
Data dependencies of the Complaint registration module:

| S.no | Table Name                         | Foreign Key       | Referenced Table       |
|------|------------------------------------|-------------------|------------------------|
| 1    | complaint_system_caretaker         | staff_Id_Id       | globals_extrainfo      |
| 2    | complaint_system_hall              | staff_id_id       | globals_extrainfo      |
| 3    | complaint_system_student_complaint | complainer_id     | globals_extrainfo      |
| 4    | complaint_system_supervisor        | sup_id_id         | globals_extrainfo      |
| 5    | complaint_system_workers           | caretaker_id_id   | complaint_system_caretaker |

### 5.3 Module Level
The Complaint registration module interacts with the Notification, Dashboard, and File Transfering system.