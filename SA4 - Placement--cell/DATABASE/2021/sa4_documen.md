# Module Name - SA-4 Placement Cell

**Faculty Mentor** - Preeti Khanna

**Student Mentor** - Rahul Sankhla

## Database Documentation of [SA4 - Placement Cell] 4.0

### Overview of the Module:

**SRS:** [(Link)](https://docs.google.com/document/d/1cs_w4cuAT9zMYUUfz46w3Cjut7ZG2MnzWW_gWPBkLCM/edit?usp=sharing)

**A. ER Diagram** [![ER Diagram](https://drive.google.com/file/d/1NmkmFLymTUPb0neaSGHfXbTgiYFYKVjQ/view?usp=sharing)](https://drive.google.com/file/d/1NmkmFLymTUPb0neaSGHfXbTgiYFYKVjQ/view?usp=sharing)

**B. Database Schema Info (in the Google sheet):** [Database Schema](https://docs.google.com/spreadsheets/d/1USqb7-jJr2A5nFAIO6F_g17_xRNxdqdYHuFaZ3oYrUc/edit#gid=0)

### C. Changes Required in Currently Implemented Tables
*(These changes will be done in this current version 4.0)*

1. **placement_cell_education**
   - **institute:**
     - Change: Need to be removed 
     - Justification: No need for institute name

2. **Placement_cell_companydetails**
   - **role:**
     - Change: Needs to be implemented
     - Justification: Students need information about the role the company is providing
   - **placementType:**
     - Change: Needs to be implemented
   - **stipend:**
     - Change: Needs to be implemented
     - Justification: Students need information about the package the company is providing
   - **year:**
     - Change: Needs to be implemented
     - Justification: Companies provide offers to a select group of students.

4. **Placement_cell_placementrecord:**
   - **test_score:**
     - Change: Needs to be removed
     - Justification: Companies don’t reveal test results
   - **test_type:**
     - Change: Needs to be removed
     - Justification: Companies don’t reveal test details.

### Tables that Need to be Implemented

1. **Placement_cell_alumni**
   - **Attributes:**
     1. Name
     2. company_name
     3. Graduation_year
     4. Purpose

2. **Placement_cell_documents**
   - **Attributes:**
     1. type
     2. student_id
     3. Content

3. **Placement_cell_resume**
   - **Attributes:**
     1. student_id
     2. content

### Tables that Need to be Removed

- placement_cell_coinventor
- placement_cell_conference
- placement_cell_experience
- placement_cell_extracurricular
- placement_cell_has*
- placement_cell_interest
- placement_cell_messageOfficer
- placement_cell_patent
- placement_cell_placementstatus
- placement_cell_project*
- placement_cell_publication
- placement_cell_role
- placement_cell_skill

### D. Data Availability for API and Functional Testing

#### D.1 Tables that are Already Populated

- Placement_cell_course
- Placement_cell_education
- Placement_cell_experience
- Placement_cell_has
- Placement_cell_project
- Placement_cell_skill

#### D.2 Tables Required to be Populated

- placement_cell_chairmanvisit
- placement_cell_coauthor
- placement_cell_coinventor
- placement_cell_companydetails
- placement_cell_conference
- placement_cell_extracurricular
- placement_cell_interest
- placement_cell_messageofficer
- placement_cell_notifystudent
- placement_cell_patent
- placement_cell_placementrecord
- placement_cell_placementschedule
- placement_cell_placementstatus
- placement_cell_publication
- placement_cell_reference
- placement_cell_role
- placement_cell_studentrecord
- placement_cell_studentplacement

#### D.3 Difficulties Faced by Your Team Regarding Populating Any Table

Most of the tables were not populated, and the attributes of most of the tables were not linking with the current use case that has been provided. 

As a result, several previous tables have to be deleted, and in their place, new tables have to be added.
