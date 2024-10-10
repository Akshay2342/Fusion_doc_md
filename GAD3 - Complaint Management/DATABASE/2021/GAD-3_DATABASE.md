# **Module Name - Complaint Management System**

**Faculty Mentor** - Dr. Avinash Chandra Pandey  
**Student Mentor** - Hardik Pratap Singh (21BCS090)

---

## **Database Documentation of GAD-3 Complaint Management System 4.0**

### **Overview of the Module:**

The Centralized complaint system combines issues related to the Computer Center, Hostels, and Cleanliness under one roof. This software aims to solve the problems of students and staff as soon as possible by providing a platform to connect them directly to the Warden/Caretaker/Supervisor of the respective departments. It allows for the immediate addressing of complaints.

---

### **SRS:**   
[**https://drive.google.com/drive/folders/1hu3qziVNPqExgmbRvBnoOEIs1tcbdhrp?usp=sharing**](https://drive.google.com/drive/folders/1hu3qziVNPqExgmbRvBnoOEIs1tcbdhrp?usp=sharing)

---

### **A. ER Diagram (to be created using draw.io):**    
[**https://drive.google.com/file/d/14EbfEHyxEtVkXuQagIhjfde45ottBVfr/view**](https://drive.google.com/file/d/14EbfEHyxEtVkXuQagIhjfde45ottBVfr/view)

---

### **B. Database Schema Info (in the Google sheet):**   
[**https://docs.google.com/spreadsheets/d/1mvTjGnzoAMMkW7CwIA058el-sfEm9L1Yfm9OA_0eDgM/edit#gid=0**](https://docs.google.com/spreadsheets/d/1mvTjGnzoAMMkW7CwIA058el-sfEm9L1Yfm9OA_0eDgM/edit#gid=0)

---

### **C. Mention all the changes required in the currently implemented Tables:**  
(These changes will be done in this current version 4.0)

#### 1. **complaint_system_studentcomplain**
   1. **worker_id_id**
      - To be removed
      - Assignment of workers should be done offline.
   2. **sup_id_id**
      - To be added.
      - Redirected complaints should be forwarded to a specific section incharge.

#### 2. **complaint_system_workers**
   - To be removed completely.

---

### **D. Data Availability for API and Functional Testing**

#### **D.1 Mention the tables that are already populated:**
   - complaint_system_studentcomplain
   - complaint_system_caretaker

#### **D.2 Mention the tables required to be populated:**
   - complaint_system_supervisor
   - complaint_system_hall

#### **D.3 Mention any difficulties faced by your team regarding populating any table (if any):**
   - (To be filled if any difficulties arise)

