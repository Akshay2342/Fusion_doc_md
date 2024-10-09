# **Module Name** - GAD-7 (RSPC MODULE)  
## **Student Mentor** - Harsh Bansal (21BCS093)  
### **Group Members:**

- Banda Satwik (21bcs054)
- Basetty Kuladeep (21bcs055)
- Chandolu Manish Babu (21BCS63)
- Kaukuntla Prudhvi Raj (21BCS111)
- Nara Sharan Kumar (21bcs141)

---

# **API Documentation of OS2 - PHC Module**

## **APIs in the module**

1. **/research_procedures/consult_insert** (Implemented but not working)
2. **/research_procedures/transfer_insert** (Implemented but not working)
3. **/research_procedures/project/project_insert** (Not Implemented)
4. **/research_procedures/project/view** (Not Implemented)
5. **/research_procedures/project/closure_report** (Not Implemented)
6. **/research_procedures/staff/view_staff** (Not Implemented)
7. **/research_procedures/staff/request_staff** (Not Implemented)
8. **/research_procedures/inventory/request_requirements** (Not Implemented)
9. **/research_procedures/inventory/view** (Not Implemented)
10. **/research_procedures/forward_fund_request** (Not Implemented)
11. **/research_procedures/forward_staff_appointment** (Not Implemented)
12. **/research_procedures/approve_fund_request** (Not Implemented)
13. **/research_procedures/forward_fund_request** (Not Implemented)
14. **/research_procedures/approve_staff_appointment** (Not Implemented)
15. **/research_procedures/issue_noc** (Not Implemented)
16. **/research_procedures/view_projects** (Not Implemented)
17. **/research_procedures/forward_fund_request** (Not Implemented)
18. **/research_procedures/manage_staff_appointment** (Not Implemented)

---

## **Overview of the Module:**

Whenever faculty wants to start a project, we add the project and request funds and staff appointment. These requests are carried through the RSPC admin to the Department head, where they are forwarded to the Dean RSPC. The Dean RSPC then forwards the fund request to the Director. Once the Director approves the request, the Dean RSPC takes care of staff appointment and approves it. Once all requests are approved, the RSPC admin issues the NOC to the project. After the NOC is issued, the faculty can start working on the project.

---

## **APIs:**

### **Already Implemented** 
*(This means that the API is already implemented and working as expected.)*
- [*GAD - 7 (SRS)*](https://docs.google.com/document/d/1j6K9sQBRTCN8TmC5Dy8hjk17SsGDwjtv7A7qiEy2fjk/edit)

*As the use case diagram has been updated, the implemented APIs don’t contribute to our present Use Cases.*

### **Yet to be Implemented** 
*(This means that the API is not yet implemented.)*

- **Add_projects UC #2**
  - **Index of APIs used:** 3
  - **Description:** RSPC admin should be able to add the approved project.
  - **Database:** No table created.
  
- **View_projects UC #3**
  - **Index of APIs used:** 4
  - **Description:** Faculty should be able to view projects.
  - **Database:** No table created.
  
- **Submit_project_closure_report UC #4**
  - **Index of APIs used:** 5
  - **Description:** Faculty should be able to add the closure report of the pending projects.
  - **Database:** No table created.
  
- **View_staff UC #6**
  - **Index of APIs used:** 6
  - **Description:** Faculty should be able to view his staff.
  - **Database:** No table created.
  
- **Request_staff UC #7**
  - **Index of APIs used:** 7
  - **Description:** Faculty should be able to request staff.
  - **Database:** No table created.
  
- **View_inventory UC #9**
  - **Index of APIs used:** 9
  - **Description:** Faculty can view the allotted inventory.
  - **Database:** No table created.
  
- **Request_requirements UC #10**
  - **Index of APIs used:** 8
  - **Description:** Faculty should be able to request requirements.
  - **Database:** No table created.
  
- **Forward_fund_request UC #12**
  - **Index of APIs used:** 10
  - **Description:** RSPC admin should be able to forward fund requests to Dean RSPC.
  - **Database:** No table created.
  
- **issue_NOC UC #14**
  - **Index of APIs used:** 15
  - **Description:** The "issue_NOC" use case allows the RSPC admin to issue NOC to faculty.
  - **Database:** No table created.
  
- **Forward_staff_appointment UC #15**
  - **Index of APIs used:** 11
  - **Description:** The "forward_staff_appointment" use case allows the Department head to forward staff appointment requests.
  - **Database:** No table created.
  
- **Forward_fund_requests UC #16**
  - **Index of APIs used:** 13
  - **Description:** The "forward_fund_requests" use case allows the Department head to forward fund requests.
  - **Database:** No table created.
  
- **Approve_staff_appointment UC #17**
  - **Index of APIs used:** 14
  - **Description:** The "Approve_staff_appointment" use case allows the Dean RSPC to approve staff appointment requests.
  - **Database:** No table created.
  
- **Forward_fund_requests UC #18**
  - **Index of APIs used:** 17
  - **Description:** The "forward_fund_requests" use case allows the Dean RSPC to forward fund requests.
  - **Database:** No table created.
  
- **Approve_fund_requests UC #18**
  - **Index of APIs used:** 12
  - **Description:** The "Approve_fund_requests" use case allows the Dean RSPC to approve fund requests.
  - **Database:** No table created.

---

## **Google Doc Link:** 
[RSPC-API-report](https://docs.google.com/document/d/1icXoa_sXRJmT1rtlJ8tGfh8rz1xl7Q5PV01H3H-e_rI/edit?usp=sharing)

![](images/Aspose.Words.8d97d367-107e-45a7-b5c5-af7a07864de2.001.png)

---
