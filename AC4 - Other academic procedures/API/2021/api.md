## Module Name - Other Academic Procedures [AC4]  
**Mentor:** Prakash Dwivedi (21BCS159)

### Please mention all the API used in the module below

1. **Check_no_dues_status API**
   - Endpoint: `http://localhost:8000/academic-procedures/stu/`
   - Status: Not working.

2. **leave_application_form submit API**
   - Endpoint: `http://localhost:8000/leave/`
   - Status: Partially Working (Data is not getting submitted to database).

3. **leave form status view API**
   - Endpoint: `http://localhost:8000/leave/`
   - Status: Partially Working

4. **apply_for_bonafide API**
   - Endpoint: `http://localhost:8000/academic-procedures/stu/`
   - Status: Yet to be implemented

5. **check status for_bonafide API**
   - Endpoint: `http://localhost:8000/academic-procedures/stu/`
   - Status: Yet to be implemented

6. **view_graduate_seminar_status API**
   - Status: Yet to be implemented

7. **Fill form for assistantship API**
   - Endpoint: `http://localhost:8000/academic-procedures/stu/`
   - Status: Not working

8. **check_assistantship_claim_status API**
   - Endpoint: `http://localhost:8000/academic-procedures/stu/`
   - Status: Not Working

9. **verify_nodues_status API**
   - Status: Yet to be implemented

10. **approve/reject leave request API**
    - Endpoint: `http://localhost:8000/academic-procedures/fac/`
    - Status: Yet to be implemented for HOD

11. **generate_nodues_form API**
    - Status: Yet to be implemented

12. **verify_bonafide API**
    - Status: Yet to be implemented

13. **assistantship_claim_approval_form API (TA)**
    - Endpoint: `http://localhost:8000/aims/`
    - Status: Not Working

14. **assistantship_claim_approval_form API (Thesis)**
    - Status: To be implemented

15. **sign_assistantship_claim_form API (HOD)**
    - Status: To be implemented

16. **give_assistantship (Acad Admin)**
    - Status: To be implemented

17. **assistantship_data API**
    - Status: Yet to be Implemented.

18. **log_graduate_seminar_data API**
    - Status: Yet to be Implemented

19. **Apply for no_dues API**
    - Status: Yet to be Implemented.

---

### Overview of the module

The aim of the document is to gather and analyse and give an in-depth insight of the Academic Procedures of IIITDM Jabalpur which includes Leave, Bonafide, and No-dues. It will define the users and functionality of the Software.

Also, we shall predict and sort out how we hope this product will be used in order to gain a better understanding of the Software, outline concepts that may be developed later, and document ideas that are being considered, but may be discarded as the product develops. This document describes the project's target audience and its user interface, hardware and software requirements. It defines how our client, team and audience see the product and its functionality. Nonetheless, it helps any designer and developer to assist in Software Development Lifecycle (SDLC) processes.

---

### APIs

##### Yet to be implemented or Partially Working (API is not implemented so yet to be implemented or API is partially working i.e. it has breakage)

- **Check no_dues status**
  - Description: Student will be able to check their nodues status & apply for the no_dues through their portal.
  - Index of API used: 1, 18
  - Database: Not clear database connection

- **Fill leave form**
  - Description: Student will be able to fill the leave form and apply for the leave. And view the status of their leave form.
  - Index of API used: 2, 3
  - Database: Not clear database connection

- **Fill bonafide form**
  - Description: Students will be able to fill the bonafide form through their portal. And view the status of their bonafide form.
  - Index of API used: 4, 5
  - Database: Not clear database connection

- **View graduate seminar status**
  - Description: Students will be able to check the schedule of their seminar through their portal.
  - Index of API used: 6
  - Database: Not clear database connection

- **Check Assistantship claim status**
  - Description: Students will be able to fill the assistantship form and check their assistantship claim status through their portal.
  - Index of API used: 7
  - Database: Not clear database connection

- **Verify no dues status**
  - Description: All the departments, labs, offices, etc. will be able to verify the nodues of all those students whose nodues are cleared.
  - Index of API used: 8
  - Database: Not clear database connection

- **Approve/reject leave request**
  - Description: HOD will be able to approve and reject the leave request of all the respective students.
  - Index of API used: 9
  - Database: Not clear database connection

- **Sign assistantship claim form**
  - Description: HOD will be able to sign the assistantship claim form after the approval of thesis supervisor.
  - Index of API used: 14
  - Database: Not clear database connection

- **Verify bonafide**
  - Description: Acad admin will be able to verify the bonafide request of the students through their portal.
  - Index of API used: 11
  - Database: Not clear database connection

- **Update nodues status**
  - Description: Acad admin will update the nodues status of every student given by all the departments and other respective people so that the students can then check it through the student portal.
  - Index of API used: 9
  - Database: Not clear database connection

- **Give assistantship**
  - Description: Acad Admin will verify all the details of respective student then forward it to the bank for transfer of stipends to the students.
  - Index of API used: 15
  - Database: Not clear database connection

- **Log Graduate seminar data**
  - Description: Department admin will be able to put the schedule of seminar for PG students.
  - Index of API used: 17
  - Database: Not clear database connection

- **Log assistantship claim data**
  - Description: Dept Admin will be able to verify whether the assistantship status of students is approved by TA supervisor, thesis supervisor, and HOD and then log the data in the database so that the students can check.
  - Index of API used: 16
  - Database: Not clear database connection

- **Approve assistantship claim form (TA)**
  - Description: TA Supervisor will be able to look through the forms of PG students and then approve it as per rules.
  - Index of API used: 12
  - Database: Not clear database connection

- **Approve assistantship claim form (Thesis Supervisor)**
  - Description: Thesis Supervisor will be able to look through the forms of PG students and then approve it as per rules.
  - Index of API used: 13
  - Database: Not clear database connection
