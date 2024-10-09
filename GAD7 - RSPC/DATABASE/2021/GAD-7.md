# **Module Name - RSPC (GAD-7)**

**Faculty Mentor:**  

**Student Mentor:** Yogesh Saini (21BCS250)

---

## **Database Documentation of [GAD-7 - RSPC] 4.0**

### **Overview of the Module:**

### **SRS:**

**A. ER Diagram**  
*(to be created using draw.io)*  
[Example ER Diagram](https://drive.google.com/file/d/1kmG8brbNB10QXaFAynjsmBUCKIbs5VSx/view)

**B. Database Schema Info**  
*(in the Google sheet)*  
[Example Database Schema Template](https://docs.google.com/spreadsheets/d/1zII3DuGzHmhpvQKzWX6SUeIBOF5BukEzft3_Siq4RcE/edit#gid=0)

---

### **C. Changes Required in Currently Implemented Tables:**

1. **Projects**  
   - **Change:** Merging Consultancy projects with Research projects.  
   - **Attribute:** Project type  
   - **Justification:** To specify whether it is a research or consultancy project.

2. **Patents**  
   - **Change:** Completely removing this table as it has no relevance in the present updated use case diagram.

3. **Tech Transfers**  
   - **Change:** Completely removing this table as it has no relevance in the present updated use case diagram.

4. **Facultys**  
   - **Change:** The page is not rendering; unable to see the fields present in the table.

---

### **D. Data Availability for API and Functional Testing**

#### **D.1 Tables That Are Already Populated:**
- [Consultancy projects](http://127.0.0.1:8000/admin/research_procedures/consultancyproject/)
- [Patents](http://127.0.0.1:8000/admin/research_procedures/patent/)
- [Research projects](http://127.0.0.1:8000/admin/research_procedures/researchproject/)
- [Tech transfers](http://127.0.0.1:8000/admin/research_procedures/techtransfer/)
- [Facultys](http://127.0.0.1:8000/admin/globals/faculty/)

#### **D.2 Tables Required to Be Populated:**
- Project_staff_info
- Funds
- Requests
- Inventory

---
