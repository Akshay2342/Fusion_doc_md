# PHC_OS2 (Web) Module Documentation

**Faculty Mentor:** Dr. Sraban Kumar Mohanty  
**Student Mentor:** Prabhat Suman (21BCS157)  

---

## Database Documentation of PHC_OS2 Module 4.0

### Purpose of the Module

The purpose of the project entitled **PRIMARY HEALTH CENTRE MANAGEMENT SYSTEM** is to computerize the Office Management and manage various activities related to the Primary Health Centre of PDPM IIITDM Jabalpur.

**Key Features:**
- Patient Registration and Record Management
- Prescription Record Keeping
- Doctor Availability and Scheduling
- Implementing measures to ensure the security and privacy of patient data

The users of this module will include registered students of the Institute (PDPM IIITDM Jabalpur), faculty members, and their dependents (family members). This software system will be a mobile application-based Health Care Management System enabling users to view schedules for consulting doctors and track their health records.

### References
- **SRS:** [SRS_PHC_WEB_FINAL1.pdf](https://drive.google.com/file/d/13ejGaBRrsafzDtfKfWQgFNYndwlCXJTS/view?usp=drive_link)
- **ER Diagram:** [ER_diagram.pdf](https://drive.google.com/file/d/1dIrDk7uLQUEB6ll_9nJNCubThZEU7HAg/view?usp=drive_link)
- **Database Schema Info:** [PHC_OS2 Database Schema Info](https://docs.google.com/spreadsheets/d/1oIbkOaGccI2lvZD6w31BYY260ykXHN-Fgh6bs8EjXr4/edit?usp=sharing)

---

### Changes Required in Currently Implemented Tables
*(These changes will be made in the current version 4.0)*

1. **health_center_stock (UC#8)**
   - **Field:** Supplier
   - **Change:** To be added
   - **Justification:** The name of the supplier should be attached to the stocks ordered.

2. **health_center_complaint (UC#6)**
   - **Field:** Complaint
   - **Change:** To be deleted
   - **Justification:** Feedback is a superset containing both positive and negative reviews.

---

### Tables to be Removed
*(These tables will be removed as their functionalities are not present in the new use case diagram.)*
- **health_center_ambulance_request**
- **health_center_appointment**
- **health_center_hospital**
- **health_center_hospital_admit**
- **health_center_counter**

### Tables to be Added
*(These tables need to be added to justify the functionalities in the new use case diagram.)*
- **health_center_medical_relief**
- **health_center_dependency_list** (If this table is not created globally, then we need to create it separately.)

---

### Data Availability for API and Functional Testing

#### D.1 Populated Tables
*(Mention the tables that are already populated.)*
- **health_center_complaint (UC#6)**
- **health_center_doctor (UC#10, UC#3)**

#### D.2 Tables Required to be Populated
*(Mention the tables that need to be populated.)*
- **health_center_doctor (UC#10, UC#3)**
- **health_center_schedule (UC#10, UC#11, UC#3, UC#4)**
- **health_center_medicine (UC#8)**
- **health_center_prescribed_medicine (UC#13)**
- **health_center_prescription (UC#7, UC#1)**
- **health_center_stock (UC#8)**
- **health_center_expiry (UC#8)**

#### D.3 Difficulties Faced
*(Mention any difficulties faced by your team regarding populating any table, if any.)*

---

### Additional Resources
[PHC_OS2 Database Status Report](https://docs.google.com/document/d/1gUs6zrLwOWPo70dL_Zmc078Di4RP_iMET0i_faHOlZg/edit?usp=sharing)

---
