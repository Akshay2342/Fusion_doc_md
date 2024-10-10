# **Module Name** - GAD 3 (Complaint Module)

**Student Mentor** - Hardik Pratap Singh (21BCS090)

---

## **API Documentation of GAD3 - Complaint Module**

Please mention all the APIs used in the module below:

1. **user/detail/complain_id/** - Already implemented  
   - Parameters: complaint id  
   - Description: Get details of a particular complaint

2. **newcomplain/** - Already implemented  
   - Parameters: none  
   - Description: Lodge a new complaint

3. **studentcomplain/** - Already implemented  
   - Parameters: none  
   - Description: View complaints of the currently logged-in user

4. **updatecomplain/complain_id/** - Already implemented  
   - Parameters: complaint id  
   - Description: Update a particular complaint

5. **removecomplain/complain_id** - Already implemented  
   - Parameters: complaint id  
   - Description: Delete a particular complaint

6. **workers/** - Already implemented  
   - Parameters: none  
   - Description: Get a list of workers

7. **addworker/** - Already implemented  
   - Parameters: none  
   - Description: Add a new worker

8. **removeworker/worker_id** - Already implemented  
   - Parameters: worker id  
   - Description: Delete a particular worker

9. **updateworker/worker_id** - Already implemented  
   - Parameters: worker_id  
   - Description: Update a particular worker’s details

10. **caretakers/** - Already implemented  
    - Parameters: none  
    - Description: Get the list of caretakers

11. **addcaretaker/** - Already implemented  
    - Parameters: none  
    - Description: Add a new caretaker

12. **removecaretaker/caretaker_id** - Already implemented  
    - Parameters: caretaker id  
    - Description: Remove a caretaker

13. **updatecaretaker/caretaker_id** - Already implemented  
    - Parameters: caretaker id  
    - Description: Update a caretaker

14. **supervisors/** - Already implemented  
    - Parameters: none  
    - Description: Get a list of supervisors

15. **addsupervisor/** - Already implemented  
    - Parameters: none  
    - Description: Add a new supervisor

16. **removesupervisor/supervisor_id** - Already implemented  
    - Parameters: supervisor id  
    - Description: Remove a supervisor

17. **update supervisor/supervisor_id** - Already implemented  
    - Parameters: supervisor id  
    - Description: Update a particular supervisor

---

## **Overview of the Module:**

The central complaint system is designed to efficiently manage and resolve issues related to electricity, hostels, and cleanliness in each campus building. The primary goal of this software is to provide a swift and effective mechanism for addressing concerns raised by individuals within the campus community, ensuring a seamless resolution process. Additionally, it serves as a communication platform, facilitating a direct connection between users and the relevant Caretaker/Supervisor for each department.

---

## **APIs:**

### Already Implemented (This means that API is already implemented and working as expected.)

- **Lodge_Complaint**
  - Lodge New Complaint
  - API Index: 2
  - Database: Complaint_system_studentcomplain

- **Track_Status**
  - Track Status of complaint
  - API Index: 1
  - Database: Complaint_system_studentcomplain

- **Response_Complaint**
  - Respond to the lodged Complaint
  - API Index: 4
  - Database: Complaint_system_studentcomplain

- **Change_Status**
  - Change status of lodged complaint after resolving the complaint
  - API Index: 4
  - Database: Complaint_system_studentcomplain

- **View_Complaint**
  - View Lodged Complaint
  - API Index: 1, 3
  - Database: Complaint_system_studentcomplain

- **Feedback**
  - Provide Feedback on the complaint
  - API Index: 4
  - Database: Complaint_system_studentcomplain

---

### Yet to be implemented or Partially Working (API is not implemented)

- **Forward**: Not Implemented  
  API has to be developed from scratch using the API provided by the FTS module. Complaints can be forwarded to the admin by the caretaker.  
  Database: Complaint_system_studentcomplain

---

## **Current Problems You Are Facing with the Module or in Its Use Cases:**

- Forward Complaint Functionality

---

**Google doc:** [API Status - GAD3](https://docs.google.com/document/d/1wd8fYVKhvaygebrva4bh33ZsFIuG8jmE6VmxOIk2biI/edit)
