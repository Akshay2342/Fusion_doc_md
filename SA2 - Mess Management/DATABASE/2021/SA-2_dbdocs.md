# Module Name: Mess Management (Web) SA2  

**Faculty Mentor:** Vijaypal Singh Rathor  
**Student Mentor:** Himanshu Ranjan  

---

## Database Documentation of SA-2 - Mess Management (Web) 4.0  

### Overview of the Module
The users of this module will be:
- Registered students of the Institute (PDPM IIITDM Jabalpur)
- Mess Warden
- Mess Caretaker of the Mess Committee

This software system will be a web and app-based mess management system utilized by the aforementioned stakeholders.

**Core Features:**
- Student registration for mess
- User login
- View mess menu
- Respond to vacation food requests
- Apply for rebates
- Request special food
- Make payments
- Provide feedback
- View announcements
- Request for deregistration

**Management Features:**
- Mess Caretaker: Manage registrations, make announcements, create and respond to vacation food requests, view feedback, manage bills, and update the mess menu.
- Mess Warden: Make and view announcements, search, and generate reports.

This interface aids the mess caretaker and warden in coordinating, controlling, and allowing users to view past records and access all functionalities without needing to visit the mess physically.

---

## Document Links
- **SRS:** [Mess Management](https://docs.google.com/document/d/1B4MA1wB-32SvVVdqodzp35uOrVuWT9Qn1BXngnYD7l4/edit)
- **A. ER Diagram:** [ER SCHEMA DRAW IO](https://drive.google.com/file/d/1dxd6W0Q-O4swUod2w-78Z952v5b1EImY/view?usp=sharing)
- **B. Database Schema Info:** [Mess Management Schema](https://docs.google.com/spreadsheets/d/138oEhraWrHpdLGhLxSzCkrRYkq4E7m8w-X2yN8EtL8M/edit)

---

## Changes Required in the Currently Implemented Tables
*(These changes will be implemented in version 4.0)*

### 1. Table: `central_mess_registration`
- **Attribute Changes:**
  - **student_id**
    - Change: Added as a foreign key reference from `academic_information_student` table.
    - Justification: New Added Table.
  - **registered**
    - Change: New attribute.
    - Justification: New Added Table.
  - **registered_start_date**
    - Change: New attribute.
    - Justification: Start date of registration is needed.
  - **registered_end_date**
    - Change: New attribute.
    - Justification: Required for deregistration from mess.
  - **balance_status**
    - Change: New attribute.
    - Justification: Current balance of the registered student is required.
  - **mess_number**
    - Change: New attribute.
    - Justification: Mess number is required for a registered student.

### 2. Table: `central_mess_announcements`
- **Attribute Changes:**
  - **id**
    - Change: Created new attribute (Primary Key).
    - Justification: Needed a unique key.
  - **subject**
    - Change: Created new attribute.
    - Justification: Subject description is required.
  - **content**
    - Change: Created new attribute.
    - Justification: Announcement content is required.
  - **date**
    - Change: Created new attribute.
    - Justification: Date is required.
  - **created_by**
    - Change: Created new attribute.
    - Justification: User needed to identify who generated the announcement.

### 3. Table: `central_mess_vacation_food`
- **Attribute Changes:**
  - **student_id**
    - Change: Made primary key.
    - Justification: Unique key required for PK.
  - **balance_status**
    - Change: Positive balance required for registration during the applied duration.
    - Justification: To check if payment is needed if account balance is lower.
  - **status**
    - Change: Removed.
    - Justification: Not required according to the current use case diagram.

### 4. Table: `central_mess_payment`
- **Attribute Changes:**
  - **student_id**
    - Change: Made primary key.
    - Justification: Unique key required for PK.
  - **balance_status**
    - Change: Positive balance required for registration during the applied duration.
    - Justification: To check if payment is needed if account balance is lower.
  - **status**
    - Change: Removed.
    - Justification: Not required according to the current use case diagram.

### 5. Table: `central_mess_change_request`
- **Change:** Table removed.
- **Justification:** No need for the table as per the current use case diagram.

### 6. Table: `central_mess_mess_meetings`
- **Change:** Table removed.
- **Justification:** No need for the table as per the current use case diagram.

### 7. Table: `central_mess_mess_minutes`
- **Change:** Table removed.
- **Justification:** No need for the table as per the current use case diagram.

### 8. Table: `central_mess_messinfos`
- **Change:** Table removed.
- **Justification:** No need for the table as per the current use case diagram.

---

## Data Availability for API and Functional Testing

### D.1 Populated Tables
- `central_mess_menu`
- `central_mess_monthly_bill`
- `central_mess_rebate`
- `central_mess_special_request`
- `central_mess_feedback`

### D.2 Tables Required to be Populated
- `central_mess_announcements`
- `central_mess_mess_reg`
- `central_mess_vacation_food`
- `central_mess_payment`

### D.3 Difficulties Faced in Populating Tables
Some tables are missing proper attributes, necessitating updates before they can be populated.
