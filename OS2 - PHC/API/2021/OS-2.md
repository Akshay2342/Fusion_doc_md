# OS2 - PHC Module

**Student Mentor:** Prabhat Suman (21BCS157)

---

## API Documentation of OS2 - PHC Module

### APIs in the Module

1. **student_view_api/schedule** - Already implemented
2. **student_view_api/prescription** - Already implemented
3. **student_view_api/medicines** - Already implemented
4. **student_view_api/complaints** - Already implemented
5. **student_view_api/doctors** - Already implemented
6. **compounder_view_api/all_complaints** - Already implemented
7. **compounder_view_api/all_hospitals** - Already implemented
8. **compounder_view_api/hospital_list** - Already implemented
9. **compounder_view_api/stocks** - Already implemented
10. **compounder_view_api/schedule** - Already implemented
11. **compounder_view_api/live_meds** - Already implemented
12. **compounder_view_api/presc_hist** - Already implemented
13. **compounder_view_api/hospitals** - Already implemented
14. **compounder_view_api/doctors** - Already implemented
15. **student_request_api/complaints** - Already implemented
16. **compounder_request_api/doctoradd** - Already implemented
17. **compounder_request_api/doctorremove** - Already implemented
18. **compounder_request_api/doctorscheduleadd** - Already implemented
19. **compounder_request_api/doctorscheduleremove** - Already implemented
20. **compounder_request_api/medicineadd** - Already implemented
21. **compounder_request_api/stockadd** - Already implemented
22. **compounder_request_api/prescriptionsubmit** - Already implemented
23. **compounder_request_api/prescripmedicineadd** - Already implemented
24. **compounder_request_api/complaintresponse** - Already implemented
25. **employee_view_api/view_dependent_health_data** - Not implemented
26. **employee_request_api/manage_dependents** - Not implemented
27. **employee_request_api/apply_for_medical_relief** - Not implemented
28. **compounder_request_api/make_announcements** - Not implemented
29. **compounder_request_api/forward_medical_relief** - Not implemented
30. **student_view_api/view_announcement** - Not implemented

---

### Overview of the Module

The purpose of the project entitled **PRIMARY HEALTH CENTRE MANAGEMENT SYSTEM** is to computerize the Office Management and manage different activities related to the Primary Health Centre of PDPM IIITDM Jabalpur.

**Key Features:**
- Patient Registration and Record Management
- Appointment and Prescription Record Keeping
- Doctor Availability and Scheduling
- Implementing measures to ensure the security and privacy of patient data

---

### API Details

#### Already Implemented APIs

1. **view_doctor_schedule**
   - **Index of APIs Used:** 1, 5
   - **Description:** Patients should be able to see the schedule of doctors and their availability.
   - **Database:** `health_center_schedule`

2. **view_health_record**
   - **Index of APIs Used:** 2, 3
   - **Description:** Patients should have access to their own health records.
   - **Database:** `health_center_prescribed_medicine`, `health_center_prescription`

3. **view_pathologist_schedule**
   - **Index of APIs Used:** 5
   - **Description:** Patients should be able to see the schedule of pathologists and their availability.
   - **Database:** `health_center_schedule`

4. **give_feedback**
   - **Index of APIs Used:** 4
   - **Description:** Patients should be able to provide feedback on their experiences.
   - **Database:** `health_center_complaint`

5. **update_doctor_schedule**
   - **Index of APIs Used:** 16, 17, 18, 19
   - **Description:** Compounders should be able to update the schedule of doctors.
   - **Database:** `health_center_schedule`

6. **update_patient_health_record**
   - **Index of APIs Used:** 22, 23
   - **Description:** Compounders should be able to update patient logs and records.
   - **Database:** `health_center_prescribed_medicine`, `health_center_prescription`

7. **update_pathologist_schedule**
   - **Index of APIs Used:** 16, 17, 18, 19
   - **Description:** Compounders will be able to update the schedule of the pathologist.
   - **Database:** `health_center_schedule`

8. **manage_inventory**
   - **Index of APIs Used:** 9, 11, 21
   - **Description:** Compounders should be able to manage the inventory of medicines and medical supplies.
   - **Database:** `health_center_stock`, `health_center_medicine`

9. **generate_report**
   - **Index of APIs Used:** 22, 23
   - **Description:** Compounders should be able to generate reports based on various parameters.
   - **Database:** `health_center_prescribed_medicine`, `health_center_prescription`

---

#### Yet to be Implemented or Partially Working APIs

1. **make_announcements**
   - **Index of APIs Used:** 28
   - **Description:** Compounders will be able to make any announcements related to PHC using this API.
   - **Database:** No table created

2. **view_announcement**
   - **Index of APIs Used:** 30
   - **Description:** Students will be able to view any announcements related to PHC using this API.
   - **Database:** No table created

3. **forward_medical_relief**
   - **Index of APIs Used:** 29
   - **Description:** Process the request for medical reimbursement from employees and forward it to the concerned authorities for acceptance.
   - **Database:** No table created

4. **manage_dependents**
   - **Index of APIs Used:** 25, 26
   - **Description:** Employees will be able to use this API to manage all information about dependents, such as their health records.
   - **Database:** No table created

---

### Current Problems with the Module or Use Cases

- **manage_dependents**
- **apply_for_medical_relief**
- **make_announcements**
- **view_announcements**

---

### Additional Resources

[Modules Testing Assignment.docx](https://docs.google.com/document/d/1gZ3FD60y9aitltMzB1RMeObb-KgUvGyq/edit?usp=sharing&ouid=104512684967527548096&rtpof=true&sd=true)

![Module Testing Assignment](images/Aspose.Words.7b06e12d-d44c-454b-b579-6056b752b31e.001.png)

---
