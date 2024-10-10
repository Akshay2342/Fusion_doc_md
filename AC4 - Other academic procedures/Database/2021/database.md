# Database Documentation 4.0 of AC-4 (App Application) Other Academic Procedures  

**Prepared by:**  

- 21BCS041-Ashish Kol  
- 21BCS060-Bikash Sabar  
- 21BCS083-Gadam Omkar  
- 21BCS086-Gaurav Singh  
- 21BCS192-Shivam Kumar  
- 21BCS159-Prakash Dwivedi (Student mentor)  

### Overview of the Module:  
The aim of the document is to gather and analyse and give an in-depth insight of the Academic Procedures of IIITDM Jabalpur which includes Leave Bonafide, and No-dues. It will define the users and functionality of the Software. Also, we shall predict and sort out how we hope this product will be used in order to gain a better understanding of the Software, outline concepts that may be developed later, and document ideas that are being considered, but may be discarded as the product develops. This document describes the project's target audience and its user interface, hardware and software requirements. It defines how our client, team and audience see the product and its functionality. Nonetheless, it helps any designer and developer to assist in Software Development Lifecycle (SDLC) processes.  

#### A. ER Diagram
[ER Diagram to be created using draw.io]([ER Diagram](https://drive.google.com/file/d/1lxXeMek8ibTMMvtHJKCSpptVEHGr1BIg/view))  

#### B. Database Schema Info
[Database Schema Info in the Google sheet]([Database Schema of Other Academic Procedure (AC4)](https://docs.google.com/spreadsheets/d/11HrMJ3QjjfIl7Uxs6Lqfq320iUq7sX4vzcTUiKmkiAw/edit?gid=0#gid=0))  

#### C. Changes required in the currently implemented Tables:  

- **No_Dues**  
  - **Physics_lab**  
    - Change: Yet to be added  
    - Justification: Physics lab incharge has to clear the dues  
  - **Computer_center**  
    - Change: Yet to be added  
    - Justification: Computer_center has to clear the dues  
  - **I-Card**  
    - Change: Yet to be added  
    - Justification: I-Card dues have to be cleared  
  - **Workshop**  
    - Change: Yet to be added  
    - Justification: Workshop has to clear the dues  
  - **Mechatronics_lab**  
    - Change: Yet to be added  
    - Justification: Mechatronics_lab incharge has to clear the dues  
  - **Signal_Processing**  
    - Change: Yet to be added  
    - Justification: Signal_Processing incharge has to clear the dues  
  - **VLSI**  
    - Change: Yet to be added  
    - Justification: VLSI incharge has to clear the dues  
  - **ECE**  
    - Change: Yet to be added  
    - Justification: ECE incharge has to clear the dues  
  - **Design_project**  
    - Change: Yet to be added  
    - Justification: Design_project incharge has to clear the dues  
  - **Design_studio**  
    - Change: Yet to be added  
    - Justification: Design_studio incharge has to clear the dues  
  - **PBI_Supervisor**  
    - Change: Yet to be added  
    - Justification: PBI_Supervisor has to clear the dues  
  - **Discipline_office**  
    - Change: Yet to be added  
    - Justification: Discipline_office has to clear the dues  
  - **Student_Gymkhana**  
    - Change: Yet to be added  
    - Justification: Student_Gymkhana has to clear the dues  
  - **Alumni_office**  
    - Change: Yet to be added  
    - Justification: Alumni_office has to clear the dues  
  - **Account_section**  
    - Change: Yet to be added  
    - Justification: Account_section has to clear the dues  
  - **Allahabad_bank**  
    - Change: Yet to be added  
    - Justification: Allahabad_bank has to clear the dues  
<br>
<br>

- **Assistantship_claim_status**  
  - **Discipline**  
    - Change: Yet to be added  
    - Justification: To Know the discipline of the student  
  - **HOD**  
    - Change: Yet to be added  
    - Justification: To check if HOD approved or not  
  - **Date**  
    - Change: Yet to be added  
    - Justification: Date of applying  
  - **Month**  
    - Change: Yet to be added  
    - Justification: The month for which he/she is applying for assistantship  
  - **Account_No**  
    - Change: Yet to be added  
    - Justification: For money transactions  
  - **TA_Supervisor**  
    - Change: Yet to be added  
    - Justification: To check if TA supervisor has approved or not  
  - **Thesis_Supervisor**  
    - Change: Yet to be added  
    - Justification: To check if Thesis Supervisor has approved or not  
<br>
<br>

- **Graduate Seminar Data (Not Implemented)**  
  - **Roll_No.**  
    - Change: Yet to be added  
    - Justification: To get Student information  
  - **Seminar_Schedule**  
    - Change: Yet to be added  
    - Justification: To check schedule of seminar  
  - **Semester**  
    - Change: Yet to be added  
    - Justification: To know student semester  
  - **Discipline**  
    - Change: Yet to be added  
    - Justification: To Know the discipline of the student  
<br>
<br>

- **Bonafide (Not Implemented)**  
  - **Roll_No.**  
    - Change: Yet to be added  
    - Justification: To get student information  
  - **Purpose**  
    - Change: Yet to be added  
    - Justification: For which purpose student is applying  
  - **Document**  
    - Change: Yet to be added  
    - Justification: Bonafide Form uploaded by Acad. Admin  
<br>
<br>

- **Leave**  
  - **Department**  
    - Change: Yet to be added  
    - Justification: HOD will approve leave of respective departments  
  - **To**  
    - Change: Yet to be added  
    - Justification: Duration of leave  
  - **From**  
    - Change: Yet to be added  
    - Justification: Duration of leave  

---
### D. Data Availability for API and Functional Testing:  

##### D.1 Mention the tables that are already populated  
- leave  
- No Dues  

##### D.2 Mention the tables required to be populated  
- Bonafide (Need to be implemented)  
- Graduate Seminar (Need to be implemented)  
- Assistantship Claim status (Need to implemented)  

##### D.3 Mention any difficulties faced by your team regarding populating any table (if any)  
- There is changes in No Dues procedures so we required to change the attributes of table.  

- Bonafide, Graduate Seminar, Assistantship Claim Status need to implement from scratch.  
