**Module Name     \-**   GAD 5 (Dashboard)  
**Faculty Mentor   \-**   Prof. Neelam Dayal  
**Student Mentor  \-**   Pranjal Jha

**Database Documentation of \[** GAD 5 – Dashboard (mobile and web) **\] 4.0**

**Overview of the Module:**

The primary purpose of the FusionIIIT Dashboard Module is to provide an intuitive and efficient platform for different user roles to access and manage their profiles, navigate to specific modules, and receive notifications from various departments. It aims to streamline administrative processes, enhance academic management, and foster communication across different levels within the institute. 

The Dashboard Module encompasses profile management for users such as Students, Head of Department, Dean Academics, Dr Acad, Chairperson, Director, and Faculty. It allows users to view and manage their profiles, access specific modules based on their roles, and receive notifications from different departments. Administrative profiles are accessible for all roles except students.

**SRS:**

**A. ER Diagram (to be using draw.io): [Gad- 5 ER- Diagram](https://drive.google.com/file/d/1Sxtx5wRC04rpED-tkIBq6QEt3lGYyMJH/view?usp=sharing)**

**B. Database Schema Info (in the google sheet): [Dasboard Database Schema Info](https://docs.google.com/spreadsheets/d/1hHYEP9QZEXUS0MWdLNA1US_2Ptxrod95LNrkszavuN0/edit#gid=0)**

**C. Mention all the changes required in the currently implemented Tables:-**  
    **(These changes will be done in the current version 4.0)**  
       
    **1). auth\_user**

*  last\_login

            a) Change: last login need to be removed  
            b) Justification: not using this field anywhere  

**2). globals\_holdsdesignation**

*      user\_id

                a) change: remove user\_id  
                b) Justification: working\_id and user-id has same reference

**3). globals\_feedback**

*      Remove Feedback table 

             
 

**D. Data Availability for API and Functional Testing**

**D1.  Mention the tables that are already populated**

*  auth\_user  
* globals\_deparmentinfo  
* globals\_extrainfo  
* globals\_designation  
* globals\_staff  
* globals\_holdsdesignation  
* globals\_faculty  
* academic\_information\_student  
* notifications\_notification

**D2. Mention the tables required to be populated**

**D3.Mention any difficulties faced by your team regarding populating any table** 

