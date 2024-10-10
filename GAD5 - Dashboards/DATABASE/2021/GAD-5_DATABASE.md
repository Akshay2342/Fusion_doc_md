# Module Name – GAD 5 (Dashboard)
**Faculty Mentor** – Prof. Neelam Dayal  
**Student Mentor** – Pranjal Jha  

## Database Documentation of [GAD 5 – Dashboard (mobile and web)] 4.0

### Overview of the Module

The primary purpose of the FusionIIIT Dashboard Module is to provide an intuitive and efficient platform for different user roles to access and manage their profiles, navigate to specific modules, and receive notifications from various departments. It aims to streamline administrative processes, enhance academic management, and foster communication across different levels within the institute. 

The Dashboard Module encompasses profile management for users such as Students, Head of Department, Dean Academics, Dr Acad, Chairperson, Director, and Faculty. It allows users to view and manage their profiles, access specific modules based on their roles, and receive notifications from different departments. Administrative profiles are accessible for all roles except students.

### SRS

#### A. ER Diagram (to be using draw.io)
[Gad-5 ER-Diagram](https://drive.google.com/file/d/1Sxtx5wRC04rpED-tkIBq6QEt3lGYyMJH/view?usp=sharing)

#### B. Database Schema Info (in the Google Sheet)
[Dashboard Database Schema Info](https://docs.google.com/spreadsheets/d/1hHYEP9QZEXUS0MWdLNA1US_2Ptxrod95LNrkszavuN0/edit#gid=0)

#### C. Mention All the Changes Required in the Currently Implemented Tables
*(These changes will be done in the current version 4.0)*

1. **auth_user**

   - **last_login**
     - **Change**: last login needs to be removed  
     - **Justification**: not using this field anywhere  

2. **globals_holdsdesignation**

   - **user_id**
     - **Change**: remove user_id  
     - **Justification**: working_id and user_id have the same reference  

3. **globals_feedback**

   - **Remove Feedback table**

#### D. Data Availability for API and Functional Testing

##### D1. Mention the Tables That Are Already Populated

- auth_user  
- globals_departmentinfo  
- globals_extrainfo  
- globals_designation  
- globals_staff  
- globals_holdsdesignation  
- globals_faculty  
- academic_information_student  
- notifications_notification  

##### D2. Mention the Tables Required to Be Populated

##### D3. Mention Any Difficulties Faced by Your Team Regarding Populating Any Table
