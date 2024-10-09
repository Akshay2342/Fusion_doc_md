# **SA4 - PLACEMENT CELL**

### **Faculty Mentor:**  
**Dr. Pritee Khanna**

### **Prepared by:**  
- **Akshay Anand** - 21BCS015  
- **Kush Batla** - 21BCS120  
- **Ayush Shinde** - 21BCS047  
- **Hardik Rana** - 21BEC091  
- **Vaibhavi Bhosale** - 21BCS233

### **Mentor:**  
**Rahul Sankhla** - 21BCS169

---

## **APIs**

1. **placement/**:  
   - Working status: 200 OK

2. **statistics/**:  
   - Working status: 200 OK

3. **get_reference_list/**:  
   - Working status: 403 Forbidden

4. **Checking_roles/**:  
   - Working status: 403 Forbidden

5. **Companyname_dropdown/**:  
   - Working status: 403 Forbidden

6. **student_records/invitation_status/**:  
   - Working status: 403 Forbidden

7. **student_records/delete_invitation_status/**:  
   - Working status: 403 Forbidden

8. **Student_records/**:  
   - Working status: 200 OK (GET request)  
   - Working status: 500 Internal Server Error (POST request)

9. **Manage_records/**:  
   - Working status: 200 OK (GET request)  
   - Working status: 500 Internal Server Error (POST request)

10. **delete_placement_statistics/**:  
    - Working status: 403 Forbidden

11. **add_placement_schedule/**:  
    - Working status: 403 Forbidden

12. **placement_schedule_save/**:  
    - Working status: 403 Forbidden

13. **Delete_placement_record/**:  
    - Working status: 500 Internal Server Error

14. **add_placement_record/**:  
    - Working status: 403 Forbidden

15. **placement_record_save/**:  
    - Working status: 403 Forbidden

16. **add_placement_visit/**:  
    - Working status: 403 Forbidden

17. **Placement_visit_save/**:  
    - Working status: 500 Internal Server Error

18. **Create/generate resume/**:  
    - API not implemented

---

## **Overview of the Module**

The Placement Cell module facilitates streamlined student-employer interaction, including resume creation and tracking, employer communication, interview scheduling, feedback collection, and analytics. It efficiently manages the logistics of interview scheduling, ensuring timely coordination between students and employers, enhancing the overall placement process.

### **Main Actors:**

1. Student
2. Placement Officer
3. Chairman

---

## **APIs Status**

- **Already Implemented**  
  **View Placement Statistics** - API Index 1, 2  
  - **Use Case Description:** All actors (TPO, student, chairman) can view past placement stats of students.  
  - **Database:** API is showing 200 OK response, but no data is getting fetched.

- **Yet to be Implemented:**  
  - API is not implemented or is partially working, i.e., it has breakage.
  - **APIs to be implemented:**  
    - **create/generate_resume**  
    - **add_placement_schedule**  
    - **Update Data (placement)**  
    - **View_placement_schedule**  
    - **View_placement_schedule_activity**  
    - **View_placement_statistics**  
    - **Generate report**  
    - **Make announcement**  
    - **upload_offer_letter/upload documents**  
    - **View_past_placement_records**  
    - **Receive_notifications**  
    - **Alumni data**  
    - **View_jobs**  
    - **apply_in_a_drive**

---

## **Current Problems We Are Facing with the Module or in Its Use Cases**

Only 2 APIs are working, and also no data is getting retrieved properly in them.
