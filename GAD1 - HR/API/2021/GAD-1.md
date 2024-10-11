**Module Name** – GAD1 (HR MODULE)

**Faculty Mentor: Dr. Aparajita Ojha Project Head: Dr Atul Gupta**

**Student Mentor** – Sanapala Anudeep (21BCS185) (Web)

Priyansh Prajapati (21BCS166) (App)

TEAM MEMBERS:

Web:

21bcs017 – Akshay Pahuja 21bcs033 – Arpit Kumar 21bcs035 – Arpit Yadav 21bcs184 – Samyak Jain 21bcs224 – Tushar Solanki

App:

21bcs077 – Dhruv Ghevariya 21bcs045 – Avdhesh Kumar 21bcs117 – Kishan Patel 21bcs140 – Naman Bhagat 21bcs151 – Omkar Wadekar

**API Documentation of GAD1 - HR Module**

**APIs in the module**

1. employee/submit\_ltc/ : Not Implemented
1. employee/approve\_ltc/id : Not Implemented
1. employee/reject\_ltc/id : Not Implemented
1. employee/forward\_ltc/id : Not Implemented
1. employee/track\_status\_ltc/id : Not Implemented
1. employee/withdraw\_ltc/id : Not Implemented
1. employee/view\_assigned\_ltc/id : Not Implemented
8. hr\_admin/assign\_reviewer\_ltc/id : Not Implemented.
8. hr\_admin/assign\_reviewer\_cpda/id : Not Implemented.
8. hr\_admin/assign\_reviewer\_appraisal/id : Not Implemented.
8. hr\_admin/assign\_reviewer\_leave\_application/id : Not Implemented.
8. hr\_admin/view\_ltc\_requests/id : Not Implemented.
8. hr\_admin/view\_cpda\_requests/id : Not Implemented.
8. hr\_admin/view\_appraisal\_requests/id : Not Implemented.
8. hr\_admin/view\_leave\_application/id : Not Implemented.
8. employee/submit\_leave\_application/ : Not Implemented.
8. employee/approve\_leave\_application/id : Not Implemented.
8. employee/reject\_leave\_application/id : Not Implemented. 19.employee/forward\_leave\_application/id : Not Implemented.
20. employee/track\_status\_leave\_application/id : Not Implemented.
20. employee/withdraw\_leave\_application/id : Not Implemented. 22.employee/view\_assigned\_leave\_applications/id : Not Implemented.
23. hr\_admin/get\_all\_emp\_records/id : Not Implemented.
23. hr\_admin/edit\_emp\_details/id : Not Implemented.
23. hr\_admin/create\_new/id : Not Implemented.
23. hr\_admin/archive\_emp/id : Not Implemented.
23. employee/submit\_cpda/ : Not Implemented.
23. employee/approve\_cpda/id : Not Implemented
23. employee/reject\_cpda/id : Not Implemented 30.employee/forward\_cpda/id : Not Implemented
31. employee/withdraw\_cpda/id : Not Implemented
31. employee/track\_status\_cpda/id : Not Implemented 33.employee/view\_assigned\_cpda/id : Not Implemented
34. employee/track\_status\_appraisal/ : Not Implemented
34. employee/submit\_appraisal/id : Not Implemented
34. employee/approve\_appraisal/id : Not Implemented
34. employee/reject\_appraisal/id : Not Implemented 38.employee/forward\_appraisal/id : Not Implemented
39. employee/withdraw\_appraisal/id : Not Implemented
39. employee/view\_assigned\_appraisal/id : Not Implemented

**Overview of the module:-**

GAD-1 Module is software designed to manage different administrative procedures related to the faculties of PDPM IIITDM Jabalpur.

The software is designed to provide automated features to the faculties and Administration Staff, to handle different faculties’ activities.

The different activities that come under this module are CPDA, LTC, and Appraisal.

The HR-1 module consists of many activities. This software product will have a limited scope as some of the activities are taken care of by other software. This software will take care of the following activities:

- CPDA (Cumulative Professional Development Allowance)
- LTC (Leave Travel Concession)
- Leave Application
- Appraisal

**APIs:-**

- **Already Implemented (**API’s are not yet implemented **)**

No API’s are implemented

- **Yet to be implemented or Partially Working** (API is not implemented so yet to be implemented or API is partially working i.e it has breakage.)

●

- LTC form submission
  - Index of apis used - 1, 5, 6
  - Description - Employee should be able to submit the LTC form after filling it.
  - Database - No table created
- LTC approval
- Index of apis used - 2, 3
- Description - Director should be able to approve or reject the LTC request.

■ Database - No table created

- CPDA form submission
  - Index of apis used - 27,31,32
  - Description - Employees should be able to submit the CPDA form after filling it.
  - Database - No table created
- CPDA HOD recommendation
  - Index of apis used - 29 ,30
  - Description - Assigned HOD should be able to forward the CPDA request to the Estt section.
  - Database - No table created
- CPDA ESTT section
  - Index of apis used - 29 , 30
  - Description - Assigned AR/DR should be able to forward the CPDA request to the Director.
  - Database - No table created
- CPDA Internal Audit
  - Index of apis used - 29 , 30
  - Description - Assigned AR/DR should be able to process the request application and forward the CPDA request to the Director.
  - Database - No table created
- CPDA form Approval
- Index of apis used - 28
- Description - Director should be able to approve or reject the CPDA form application.
- Database - No table created


- Appraisal
  - Index of apis used - 34 , 35, 39
  - Description - Employees should be able to apply for the appraisal by filling the form and submitting it.
  - Database - no table created
- Review and Remarks
  - Index of apis used - NONE
  - Description - Director and/or HOD should be able to review and give remarks on the appraisal request.
  - Database - No table created
- Assign reviewer
  - Index of apis used - 8,9,10,11
  - Description - HR Admin should be able to assign the different applications to the competent authorities for review and further procedure.
  - Database - No table created
- LTC Estt. Section
- Index of apis used - 3 , 4
- Description - Assigned AR/DR should be able to forward the LTC request to the Director.
- Database - No table created
- LTC Internal Audit
- Index of apis used - 3, 4
- Description - Assigned AR/DR should be able to process the request application and forward the LTC request to the Director.
- Database - No table created
- LTC HOD Recommendation
- Index of apis used - 3, 4
- Description - Assigned HOD should be able to forward the LTC request to the Estt section.
- Database - No table created
- Leave HOD Recommendation
  - Index of apis used - 18, 19
  - Description - Assigned HOD should be able to forward the leave application request to the Estt section.
  - Database - No table created
- Leave Estt. Section
  - Index of apis used - 18, 19
  - Description - Assigned AR/DR should be able to process the request and forward the leave application to the Director.
  - Database - No table created
- Leave Form Submission
- Index of apis used - 16 , 20 ,21
- Description: Employee should be able to submit the leave application form.
- Database - No table created

**Current problems you are facing with the module or in its use cases —**

- HR module not visible in right panel for faculty and staff
- APIs not implemented
- None of the use cases implemented
- Notifications not implemented
- Error handling not done
- REST framework not implemented (This will help in correctly implementing APIs)

**Google Doc Link : [https://docs.google.com/document/d/1mxz9Aaec3tUOlzOg_lp3NKL47ssxwRFA4ON UIEBB8es/edit?usp=sharing](https://docs.google.com/document/d/1mxz9Aaec3tUOlzOg_lp3NKL47ssxwRFA4ONUIEBB8es/edit?usp=sharing)**

\+
