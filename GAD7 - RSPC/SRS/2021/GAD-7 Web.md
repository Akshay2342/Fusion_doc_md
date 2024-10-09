# Fusion ERP

**Software Requirements Specification**  
**for**  
**GAD-7 RSPC MODULE (web)**

**Prepared by:**  
Banda Satwik (21BCS054)  
Basetty Kuladeep (21BCS055)  
Chandolu Manish Babu (21BCS063)  
Kaukuntla Prudvi Raj (21BCS111)  
Nara Sharan Kumar (21BCS141)  

**Faculty Mentor:**  
Prof. Aparajita Ojha  

**Student Mentor:**  
Harsh Bansal (21BCS093)  

## 1. Introduction

### 1.1 Introduction about the Fusion – A brief Description

FusionIIIT stands as a testament to the seamless integration and automation of diverse functions within PDPM Indian Institute of Information Technology, Design and Manufacturing, Jabalpur. Crafted with precision using Python 3.8 and powered by the Django Web framework, this initiative is a student-driven endeavor designed to elevate the institute's operational landscape. Encompassing everything from efficient administration management to academic prowess and miscellaneous departmental tasks, FusionIIIT is a holistic solution that harmonizes the intricacies of campus life.

Imagine it as a digital wizard that takes care of everything, from organizing the administrative stuff to making academics smoother. It's not just limited to the usual tasks; FusionIIIT jumps into various departments and sections, making sure every corner of campus life runs smoothly.

In the admin side, it handles the complicated paperwork and processes. For academics, it brings a digital touch, making learning and managing courses easier. But it doesn't stop there; FusionIIIT is like a friendly companion for all the different parts of the campus, making sure everything works well.

In simpler terms, FusionIIIT is not just a tool – it's a helpful friend, making life at PDPM IIITDM Jabalpur more organized and enjoyable for everyone.

### 1.2 Purpose of the module

The RSPC Module is a part of the Fusion project that is responsible for maintaining the record of projects of professors, their achievements, conferences, book publications, etc. It provides a platform for professors and staff members to add projects and their details, which are not visible to other users of the system. In addition, the module also maintains the profiles of professors and staff members, which includes their projects, achievements, etc. This is software designed to manage different activities related to the dean RSPC department of PDPM IIITDM Jabalpur. The software is designed to provide automated features to Faculty, Dean, and Staff. The different activities that come under the dean RSPC department such as project funds, eis etc.

### 1.3 Scope of the module

The scope of the RSPC Module is to provide a platform for professors and staff members to manage their projects, achievements, conferences, book publications, etc. It also maintains their profiles and allows them to add projects and their details. The module ensures that the information added by professors and staff members is not visible to other users of the system. In addition to the specific design components of this software, this document will make clear the design team’s goals of creating value-added software which not only correctly captures faculty data, but then efficiently stores it, sorts it, retrieves it, and delivers this critical care information where it is needed by Dean and Staff.

## 2. User/Actor Characteristics

### 2.1 Faculty

Represents individuals who register the project.

- **Role:** Initiates the Application for Research Project  
- **Specific Functionalities:**
  - Online Apply for Project Registration
  - Request for Extension of project
  - Reallocation of the fund Among Different Heads
  - Request for closure of project

### 2.2 RSPC_ADMIN (STAFF)

- **Role:** Forwards different types of applications to the DEAN RSPC.  
- **Specific Functionalities:**
  - Forward applications to Dean RSPC based on requirement.
  - Manage staff appointment
  - View projects
  - Issue NOC

### 2.3 DEAN (RSPC)

Dean Research, Sponsored Projects and Consultancy (RSPC) in the institute to provide specialized administrative and managerial support and awareness for the operation of Sponsored Research Projects, Consultancy, Fieldwork, IPR related issues as well as to co-ordinate and facilitate all Research & Development activities in the Institute.

- **Role:** Approves/rejects different types of applications or forwards to the director depending upon the rights.  
- **Specific Functionalities:**
  - Approves/rejects different types of applications.
  - Forward applications to Director based on requirement.

### 2.4 HEAD OF DEPARTMENT

- **Role:** Responsible for checking and forwarding the different types of applications to the dean RSPC staff.  
- **Specific Functionalities:**
  - Forwards Applications to DEAN RSPC ADMIN
  - Forwards Staff appointment request

### 2.5 Director

- **Role:** Approves Project fund request.  
- **Specific Functionalities:**
  - Approves/Rejects project fund request.

## 3. Functional Requirements

### 3.1 Use Case Diagram

![Use Case Diagram](images/Aspose.Words.fdc99f75-64cf-406e-b3e9-0552a34497f7.001.jpeg)

### 3.2 Use Case Description

#### UC#1: Manage Projects

| **UC ID** | UC#1 |
|-----------|-------|
| **Use case name** | manage_projects |
| **Description** | The "Manage Projects" use case allows the Faculty to add, view and submit closure reports of the project requests to the Fusion portal. |
| **Actor** | Faculty |
| **Precondition** | The Faculty is logged into the system. |

| **Main Flow** |  |
|---------------|---|
| 1 | The Faculty navigates to the "Manage Projects" section. |
| 2 | The system displays the “Add Projects”, ”View Projects”, “Submit Project Closure Report” sections. |
| 3 | The Faculty can navigate to the “Add Projects” section and add a new project by providing the details. [A1] |
| 4 | The Faculty can navigate to the “View Projects” section and view the completed project details. |
| 5 | The Faculty can navigate to the “Submit Project Closure Report” section and submit the closure report of a pending project. [A1] |

| **Post conditions** | The Faculty is navigated to “Add Projects” or ”View Projects” or “Submit Project Closure Report” sections. |
|---------------------|---|
| **Alternate Flow** | A1: Faculty presses the cancel button while filling the form. |
| **Sub Flow** | NIL |
| **Global Alternate Flow** | GA: If a technical error occurs during the execution of any action (e.g., database failure, server issues), the system displays an error message and logs the incident. |

#### UC#2: Add Projects

| **UC ID** | UC#2 |
|-----------|-------|
| **Use case name** | Add_projects |
| **Description** | The "Add Projects" use case allows the Faculty to add projects to the Fusion portal. |
| **Actor** | Faculty |
| **Precondition** | The Faculty is navigated into the “Manage Projects” section. |

| **Main Flow** |  |
|---------------|---|
| 1 | Faculty selects the “Add Projects” section. |
| 2 | Faculty fills the form and submits it. |

| **Post conditions** | The Faculty is navigated to “Add Projects” or ”View Projects” or “Submit Project Closure Report” sections. |
|---------------------|---|
| **Alternate Flow** | A1: Faculty is navigated to Manage Projects Section. |
| **Sub Flow** | NIL |
| **Global Alternate Flow** | GA: If a technical error occurs during the execution of any action (e.g., database failure, server issues), the system displays an error message and logs the incident. |

#### UC#3: View Projects

| **UC ID** | UC#3 |
|-----------|-------|
| **Use case name** | View_projects |
| **Description** | The "View projects" use case allows the Faculty to view the projects for which the closure reports are submitted. |
| **Actor** | Faculty |
| **Precondition** | The Faculty is navigated into the “Manage projects” section. |

| **Main Flow** |  |
|---------------|---|
| 1 | The faculty selects the “View projects” section. |
| 2 | The faculty views the projects. |

| **Post conditions** | Faculty is navigated to the “Manage Projects” Section. |
|---------------------|---|
| **Alternate Flow** | A1: Faculty clicks on the “back” button to navigate back to the dashboard. |

#### UC#4: Submit Project Closure Report

| **UC ID** | UC#4 |
|-----------|-------|
| **Use case name** | Submit project closure report |
| **Description** | The “Submit project closure report” use case allows the Faculty to submit closure reports for completed projects. |
| **Actor** | Faculty |
| **Precondition** | The Faculty is navigated into the “Manage projects” section. |

| **Main Flow** |  |
|---------------|---|
| 1 | The faculty selects the “Submit project closure report” section. |
| 2 | The faculty is given a list of projects for which the closure reports are not submitted. |

| **Post conditions** | Faculty is navigated to the “Manage Projects” Section. |
|---------------------|---|
| **Alternate Flow** | A1: Faculty clicks on the “back” button to navigate back to the dashboard. |

#### UC#5: Manage Staff




|**UC ID**|UC#5|
| - | - |
|**Use case name**|**manage\_staff**|
|**Description**|The "Manage staff" use case allows the Faculty to request for staff and view the already assigned staff|
|**Actor**|Faculty|



<table><tr><th colspan="1" valign="top"><b>Precondition</b></th><th colspan="2" valign="top">The Faculty is logged into the system.</th></tr>
<tr><td colspan="1" rowspan="4" valign="top"><b>Main Flow</b></td><td colspan="1" valign="bottom">1</td><td colspan="1" valign="bottom">The Faculty navigates to the "Manage staff" section.</td></tr>
<tr><td colspan="1" valign="top">2</td><td colspan="1" valign="bottom">The system displays the “View staff”, ”Request staff”, sections.</td></tr>
<tr><td colspan="1" valign="top">3</td><td colspan="1" valign="bottom">The Faculty can navigate to the “View staff” section to view staff of existing projects</td></tr>
<tr><td colspan="1" valign="top">4</td><td colspan="1" valign="top">The Faculty can navigate to the “Request staff” section and request for staff</td></tr>
<tr><td colspan="1" valign="top"><b>Post conditions</b></td><td colspan="2">The Faculty is navigated to “View staff” or ”Request staff”, sections .</td></tr>
</table>



|**UC ID**|UC#6||
| - | - | :- |
|**Use case name**|**View\_staff**||
|**Description**|The "View staff" use case allows the Faculty to view the existing staff for the projects.||
|**Actor**|Faculty||
|**Precondition**|The Faculty is navigated into the “Manage staff” section.||
|**Main Flow**|1|The faculty selects the “View staff” section.|
||2|The faculty views the staff assigned to the projects.|
|**Post conditions**|Faculty is navigated to the “Manage staff” Section.||



|**Alternate Flow**|A 1||Faculty clicks on the “back” button to navigate back to the dashboard|
| - | - | :- | :- |



|**UC ID**|UC#7|||
| - | - | :- | :- |
|**Use case name**|**Request\_staff**|||
|**Description**|The "Request staff" use case allows the Faculty to request staff for the projects.|||
|**Actor**|Faculty|||
|**Precondition**|The Faculty is navigated into the “Manage staff” section.|||
|**Main Flow**|1|The faculty selects the “Request staff” section.||
||2|The faculty requests the staff.||
|**Post conditions**|Faculty is navigated to the “Manage staff” Section.|||
|**Alternate Flow**|A 1||Faculty clicks on the “back” button to navigate back to the dashboard|



|**UC ID**|UC#8|
| - | - |
|**Use case name**|**manage\_inventory**|



<table><tr><th colspan="1" valign="top"><b>Description</b></th><th colspan="2" valign="top">The "Manage inventory" use case allows the Faculty to request for funds and view the already allocated funds.</th></tr>
<tr><td colspan="1" valign="top"><b>Actor</b></td><td colspan="2" valign="top">Faculty</td></tr>
<tr><td colspan="1" valign="top"><b>Precondition</b></td><td colspan="2" valign="top">The Faculty is logged into the system.</td></tr>
<tr><td colspan="1" rowspan="4" valign="top"><b>Main Flow</b></td><td colspan="1" valign="bottom">1</td><td colspan="1" valign="bottom">The Faculty navigates to the "Manage inventory" section.</td></tr>
<tr><td colspan="1" valign="top">2</td><td colspan="1" valign="bottom">The system displays the “View inventory”, ”Request requirements”, sections.</td></tr>
<tr><td colspan="1" valign="top">3</td><td colspan="1" valign="bottom">The Faculty can navigate to the “View inventory” section to view inventory of existing projects</td></tr>
<tr><td colspan="1" valign="top">4</td><td colspan="1" valign="top">The Faculty can navigate to the “Request requirements” section and request for requirements(funds).</td></tr>
<tr><td colspan="1" valign="top"><b>Post conditions</b></td><td colspan="2">The Faculty is navigated to “View inventory” or ”Request requirements”, section .</td></tr>
</table>



|**UC ID**|UC#9|
| - | - |
|**Use case name**|**View\_inventory**|
|**Description**|The "View inventory" use case allows the Faculty to view the existing inventory for the projects.|
|**Actor**|Faculty|
|**Precondition**|The Faculty is navigated into the “Manage inventory” section.|



|**Main Flow**|1|The faculty selects the “View inventory” section.||
| - | - | - | :- |
||2|The faculty views the inventory allocated to the projects.||
|**Post conditions**|Faculty is navigated to the “Manage inventory” Section.|||
|**Alternate Flow**|A 1||Faculty clicks on the “back” button to navigate back to the dashboard|



|**UC ID**|UC#10|||
| - | - | :- | :- |
|**Use case name**|**Request\_requirements**|||
|**Description**|The "Request requirements" use case allows the Faculty to request requirements for the projects.|||
|**Actor**|Faculty|||
|**Precondition**|The Faculty is navigated into the “Manage inventory” section.|||
|**Main Flow**|1|The faculty selects the “Request requirements” section.||
||2|The faculty requests the requirements or funds.||
|**Post conditions**|Faculty is navigated to the “Manage inventory” Section.|||
|**Alternate Flow**|A 1||Faculty clicks on the “back” button to navigate back to the dashboard|



<table><tr><th colspan="1" valign="bottom"><b>UC ID</b></th><th colspan="3" valign="bottom">UC#11</th></tr>
<tr><td colspan="1" valign="bottom"><b>Use case name</b></td><td colspan="3" valign="bottom"><b>view_projects</b></td></tr>
<tr><td colspan="1" valign="top"><b>Description</b></td><td colspan="3" valign="bottom">The "View Projects" use case allows the RSPC admin to view projects submitted by faculty.</td></tr>
<tr><td colspan="1" valign="bottom"><b>Actor</b></td><td colspan="3" valign="bottom">Rspc Admin</td></tr>
<tr><td colspan="1" valign="bottom"><b>Precondition</b></td><td colspan="3" valign="bottom">The Rspc Admin is logged in into the system.</td></tr>
<tr><td colspan="1" rowspan="2" valign="top"><b>Main Flow</b></td><td colspan="1" valign="bottom">1</td><td colspan="2" valign="bottom">The Rspc Admin navigates to the "View Projects" section.</td></tr>
<tr><td colspan="1" valign="bottom">2</td><td colspan="2" valign="bottom">The system displays the list of ongoing and closed projects.</td></tr>
<tr><td colspan="1" valign="bottom"><b>Post conditions</b></td><td colspan="3" valign="bottom">The Rspc Admin is able to view projects list</td></tr>
<tr><td colspan="1" rowspan="2" valign="top"><b>Alternate Flow</b></td><td colspan="1" rowspan="2" valign="top">A 1</td><td colspan="1"></td><td colspan="1" valign="bottom">Rspc Admin clicks on back which navigates to dashboard</td></tr>
<tr><td colspan="1"></td><td colspan="1"></td></tr>
</table>


<table><tr><th colspan="1" valign="bottom"><b>UC ID</b></th><th colspan="2" valign="bottom">UC#12</th></tr>
<tr><td colspan="1" valign="bottom"><b>Use case name</b></td><td colspan="2" valign="bottom"><b>Forward_fund_request</b></td></tr>
<tr><td colspan="1" valign="top"><b>Description</b></td><td colspan="2" valign="bottom">The "Forward_fund_request" use case allows the RSPC admin to forward fund requests of projects submitted by faculty to dean RSPC.</td></tr>
<tr><td colspan="1" valign="bottom"><b>Actor</b></td><td colspan="2" valign="bottom">Rspc Admin</td></tr>
<tr><td colspan="1" valign="bottom"><b>Precondition</b></td><td colspan="2" valign="bottom">The Rspc Admin is logged in into the system.</td></tr>
<tr><td colspan="1" rowspan="2" valign="top"><b>Main Flow</b></td><td colspan="1" valign="top">1</td><td colspan="1" valign="bottom">The Rspc Admin navigates to the "Forward_fund_request" section.</td></tr>
<tr><td colspan="1" valign="bottom">2</td><td colspan="1" valign="bottom">The system displays the list of fund requests.</td></tr>
</table>



||3|Forwards to Dean RSPCon clicking forward button||
| :- | - | - | :- |
|**Post conditions**|The Rspc Admin is able to view projects fund request list and able to forward to Dean RSPC|||
|**Alternate Flow**|A 1||Rspc Admin clicks on back which navigates to dashboard|



<table><tr><th colspan="1" valign="bottom"><b>UC ID</b></th><th colspan="3" valign="bottom">UC#13</th></tr>
<tr><td colspan="1" valign="bottom"><b>Use case name</b></td><td colspan="3" valign="bottom"><b>manage_staff_appointment</b></td></tr>
<tr><td colspan="1" valign="top"><b>Description</b></td><td colspan="3" valign="bottom">The "manage_staff-appointment" use case allows the RSPC admin to staff requests of projects submitted by faculty to dean RSPC..</td></tr>
<tr><td colspan="1" valign="bottom"><b>Actor</b></td><td colspan="3" valign="bottom">Rspc Admin</td></tr>
<tr><td colspan="1" valign="bottom"><b>Precondition</b></td><td colspan="3" valign="bottom">The Rspc Admin is logged in into the system.</td></tr>
<tr><td colspan="1" rowspan="2" valign="top"><b>Main Flow</b></td><td colspan="1" valign="top">1</td><td colspan="2" valign="bottom">The Rspc Admin navigates to the "manage_staff-appointment" section.</td></tr>
<tr><td colspan="1" valign="bottom">2</td><td colspan="2" valign="bottom">The system displays the list of approved projects.</td></tr>
<tr><td colspan="1"></td><td colspan="1" valign="bottom">3</td><td colspan="2" valign="bottom">Forwards to Dean RSPC on clicking forward button</td></tr>
<tr><td colspan="1" valign="bottom"><b>Post conditions</b></td><td colspan="3" valign="bottom">The Rspc Admin is able to view staff requests list</td></tr>
<tr><td colspan="1" rowspan="2" valign="top"><b>Alternate Flow</b></td><td colspan="1" rowspan="2" valign="top">A 1</td><td colspan="1"></td><td colspan="1" valign="bottom">Rspc Admin clicks on back which navigates to dashboard</td></tr>
<tr><td colspan="1"></td><td colspan="1"></td></tr>
</table>


|**UC ID**|UC#14|
| - | - |
|**Use case name**|**issue\_NOC**|
|**Description**|The "issue\_NOC" use case allows the RSPC admin to issue NOC to faculty.|



<table><tr><th colspan="1" valign="bottom"><b>Actor</b></th><th colspan="3" valign="bottom">Rspc Admin</th></tr>
<tr><td colspan="1" valign="bottom"><b>Precondition</b></td><td colspan="3" valign="bottom">The Rspc Admin is logged in into the system.</td></tr>
<tr><td colspan="1" rowspan="2" valign="top"><b>Main Flow</b></td><td colspan="1" valign="bottom">1</td><td colspan="2" valign="bottom">The Rspc Admin navigates to the "issue_NOC" section.</td></tr>
<tr><td colspan="1" valign="bottom">2</td><td colspan="2" valign="bottom">The system displays the list of closure project reports.</td></tr>
<tr><td colspan="1"></td><td colspan="1" valign="bottom">3</td><td colspan="2" valign="bottom">Forwards NOC to faculty</td></tr>
<tr><td colspan="1" valign="bottom"><b>Post conditions</b></td><td colspan="3" valign="bottom">The Rspc Admin is able to view closed project list</td></tr>
<tr><td colspan="1" rowspan="2" valign="top"><b>Alternate Flow</b></td><td colspan="1" rowspan="2" valign="top">A 1</td><td colspan="1"></td><td colspan="1" valign="bottom">Rspc Admin clicks on back which navigates to dashboard</td></tr>
<tr><td colspan="1"></td><td colspan="1"></td></tr>
</table>


|**UC ID**|UC#15||
| - | - | :- |
|**Use case name**|**forward\_staff\_appointment**||
|**Description**|The "forward\_staff\_appointment" use case allows the Department head to forward staff appointment requests.||
|**Actor**|Department head||
|**Precondition**|The Department head is logged in into the system.||
|**Main Flow**|1|The system displays the “Forward staff appointment”, and “Forward fund requests” sections.|



<table><tr><th colspan="1"></th><th colspan="1" valign="top">2</th><th colspan="2" valign="bottom">The Department head can navigate to the “Forward staff appointment” section and forward the staff appointment request for approval.</th></tr>
<tr><td colspan="1" valign="top"><b>Post conditions</b></td><td colspan="3">The Department head has forwarded the staff appointment requests</td></tr>
<tr><td colspan="1" rowspan="2" valign="top"><b>Alternate Flow</b></td><td colspan="1" valign="bottom">A 1</td><td colspan="1"></td><td colspan="1" valign="bottom">Department head clicks on the “back” which navigates to the dashboard.</td></tr>
<tr><td colspan="1" valign="bottom">A 4</td><td colspan="1"></td><td colspan="1" valign="bottom">Department navigates to the “forward fund requests” section.</td></tr>
</table>



<table><tr><th colspan="1" valign="bottom"><b>UC ID</b></th><th colspan="2" valign="bottom">UC#16</th></tr>
<tr><td colspan="1" valign="top"><b>Use case name</b></td><td colspan="2" valign="top"><b>forward_fund_requests</b></td></tr>
<tr><td colspan="1" valign="top"><b>Description</b></td><td colspan="2" valign="top">The "forward_fund_requests" use case allows the Department head to forward fund requests.</td></tr>
<tr><td colspan="1" valign="top"><b>Actor</b></td><td colspan="2" valign="top">Department head</td></tr>
<tr><td colspan="1" valign="top"><b>Precondition</b></td><td colspan="2" valign="top">The Department head is logged in into the system.</td></tr>
<tr><td colspan="1" rowspan="2" valign="top"><b>Main Flow</b></td><td colspan="1" valign="top">1</td><td colspan="1" valign="bottom">The system displays the “Forward staff appointment”, and “Forward fund requests” sections.</td></tr>
<tr><td colspan="1" valign="top">2</td><td colspan="1" valign="bottom">The Department head can navigate to the “Forward fund requests” section and forward the fund requests for approval.</td></tr>
<tr><td colspan="1" valign="top"><b>Post conditions</b></td><td colspan="2" valign="top">The Department head has forwarded the fund requests</td></tr>
</table>



<table><tr><th colspan="1" rowspan="2" valign="top"><b>Alternate Flow</b></th><th colspan="1" valign="bottom">A 1</th><th colspan="1"></th><th colspan="1" valign="bottom">Department head clicks on the “back” which navigates to the dashboard.</th></tr>
<tr><td colspan="1" valign="bottom">A 4</td><td colspan="1"></td><td colspan="1" valign="bottom">Department navigates to the “forward staff appointment ” section.</td></tr>
</table>



<table><tr><th colspan="1" valign="bottom"><b>UC ID</b></th><th colspan="3" valign="bottom">UC#17</th></tr>
<tr><td colspan="1" valign="top"><b>Use case name</b></td><td colspan="3" valign="top"><b>Approve_staff_appointment</b></td></tr>
<tr><td colspan="1" valign="top"><b>Description</b></td><td colspan="3" valign="top">The "Approve_staff_appointment" use case allows the Dean RSPC to Approve staff appointment requests.</td></tr>
<tr><td colspan="1" valign="top"><b>Actor</b></td><td colspan="3" valign="top">Dean RSPC</td></tr>
<tr><td colspan="1" valign="top"><b>Precondition</b></td><td colspan="3" valign="top">The Dean RSPC is logged in into the system.</td></tr>
<tr><td colspan="1" rowspan="2" valign="top"><b>Main Flow</b></td><td colspan="1" valign="top">1</td><td colspan="2" valign="bottom">The system displays the “Approve staff appointment”, and “Forward fund requests” sections.</td></tr>
<tr><td colspan="1" valign="top">2</td><td colspan="2" valign="bottom">The Dean RSPC can navigate to the “Approve staff appointment” section and Approves the staff appointment request.</td></tr>
<tr><td colspan="1" valign="top"><b>Post conditions</b></td><td colspan="3" valign="top">The Dean RSPC has Approved the staff appointment requests</td></tr>
<tr><td colspan="1" rowspan="2" valign="top"><b>Alternate Flow</b></td><td colspan="1" valign="bottom">A 1</td><td colspan="1"></td><td colspan="1" valign="bottom">Dean RSPC clicks on the “back” which navigates to the dashboard.</td></tr>
<tr><td colspan="1" valign="bottom">A 4</td><td colspan="1"></td><td colspan="1" valign="bottom">Dean RSPC navigates to the “forward fund requests” section.</td></tr>
</table>



<table><tr><th colspan="1" valign="bottom"><b>UC ID</b></th><th colspan="3" valign="bottom">UC#18</th></tr>
<tr><td colspan="1" valign="top"><b>Use case name</b></td><td colspan="3" valign="top"><b>forward_fund_requests</b></td></tr>
<tr><td colspan="1" valign="top"><b>Description</b></td><td colspan="3" valign="top">The "forward_fund_requests" use case allows the Dean RSPC to forward fund requests.</td></tr>
<tr><td colspan="1" valign="top"><b>Actor</b></td><td colspan="3" valign="top">Dean RSPC</td></tr>
<tr><td colspan="1" valign="top"><b>Precondition</b></td><td colspan="3" valign="top">The Dean RSPC is logged in into the system.</td></tr>
<tr><td colspan="1" rowspan="2" valign="top"><b>Main Flow</b></td><td colspan="1" valign="top">1</td><td colspan="2" valign="bottom">The system displays the “Approve staff appointment”, and “Forward fund requests” sections.</td></tr>
<tr><td colspan="1" valign="top">2</td><td colspan="2" valign="bottom">The Dean RSPC can navigate to the “Forward fund requests” section and forward the fund requests for approval.</td></tr>
<tr><td colspan="1" valign="top"><b>Post conditions</b></td><td colspan="3" valign="top">The Dean RSPC has forwarded the fund requests</td></tr>
<tr><td colspan="1" rowspan="2" valign="top"><b>Alternate Flow</b></td><td colspan="1" valign="bottom">A 1</td><td colspan="1"></td><td colspan="1" valign="bottom">Dean RSPC clicks on the “back” which navigates to the dashboard.</td></tr>
<tr><td colspan="1" valign="bottom">A 4</td><td colspan="1"></td><td colspan="1" valign="bottom">Dean RSPC navigates to the “Approve staff appointment ” section.</td></tr>
</table>



|**UC ID**|UC#19|
| - | - |
|**Use case name**|**Approve\_fund\_requests**|
|**Description**|The "Approve\_fund\_requests" use case allows the Director to Approve fund requests|



<table><tr><th colspan="1" valign="top"><b>Actor</b></th><th colspan="3" valign="top">Director</th></tr>
<tr><td colspan="1" valign="top"><b>Precondition</b></td><td colspan="3" valign="top">The Director is logged in into the system.</td></tr>
<tr><td colspan="1" rowspan="2" valign="top"><b>Main Flow</b></td><td colspan="1" valign="top">1</td><td colspan="2" valign="top">The system displays the “Approve fund requests”.</td></tr>
<tr><td colspan="1" valign="bottom">2</td><td colspan="2" valign="bottom">The Director can navigate to the “Approve fund requests”.</td></tr>
<tr><td colspan="1" valign="top"><b>Post conditions</b></td><td colspan="3" valign="top">The Director has approved the fund requests</td></tr>
<tr><td colspan="1" valign="top"><b>Alternate Flow</b></td><td colspan="1" valign="bottom">A 1</td><td colspan="1"></td><td colspan="1" valign="bottom">Director clicks on the “back” which navigates to the dashboard.</td></tr>
</table>

**3.3. Other Functional Requirements**

1  This module will make use of the **communication module** for sending notifications and alerts to various actors involved in the module suitably for booking confirmations, rejections, or modifications, etc.
1  Automated email or SMS notifications for booking confirmations, rejections, or modifications.
1  Alerts for critical inventory levels and other important updates.
1  The **Super admin** of Fusion should be able to assign roles for VH In charge and VH caretaker.
1  The system should be able to deal with offline bookings.
1  The category conversion of the visitors may be possible subjected to the approval of the competent authority.
1  Changes in the tariff may be possible time to time and the decision of the institute authorities.
1  …

**3.4 Other constraints**

1. **User Interfaces**

The user interface should comply with the colour scheming and dashboard design of the FUSIONIIT. Users should be able to navigate from one functionality to other. Inter module navigation should be smooth. All the functionalities should be easy to use and no specific training should be required for the usage of the module

2. **Tech Stack Used**

FRONTEND- HTML,CSS,Python BACKEND- DJANGO DATABASE- PostgreSQL

3. **Business rules (if any)**

1\. NA

4. **Non- Functional Requirements**
1. **Performance:**

The system should respond to user interactions quickly. Response time for booking actions, inventory updates, and notifications should be less.

2. **Scalability:**

The system should handle a mass of concurrent users. System performance should be evaluated under increasing load conditions.

3. **Availability:**

The system should be available 99.9% of the time.

4. **Security:**

Ensure data confidentiality and integrity. Role-based authorization ensures that users can only perform actions relevant to their designated roles.

5. **Module dependencies with other fusion modules**

**5.1. UI Level**

Whenever faculty wants to start a project we would add the project and request for funds and staff appointment ,these requests are carried through RSPC admin to the Department head where the requests are again forwarded to the Dean RSPC , now Dean RSPC forwards the fund request to the Director.

Once the Director approves the request , Dean RSPC takes care of staff appointment and approves it .Once all requests are approved ,RSPC admin issues NOC to the project ,Once NOC is issued ,the faculty can start working on the project

In [Figma](https://www.figma.com/file/w2Mx7biMn2PJsYsPm7Qxdi/GAD-7?type=design&node-id=0-1&mode=design) we have demonstrated the following webpages

**5.2 DB Level Dependencies**

- This module will share the Notification schema with the notifications module.
- This module will share project information schema from the database with the purchase and store module.
- This module will share information regarding the NOCs issued with File Tracking module

**5.3. Module Level Dependencies**

FILE TRACKING MODULE(GAD4)-

- Once a request from the Director is approved , RSPC admin will issue NOC to the faculty.

NOTIFICATIONS MODULE(OS3)-

- Whenever a faculty adds a project,submits a project closure report , RSPC admin gets a notification alerting about the action.
- Whenever a faculty requests for staff , it will be notified to the RSPC admin.
- Whenever a faculty requests for requirements ,it will be notified to the RSPC admin.
- All forwarded requests from RSPC admin will be notified to the Department Head.
- All forwarded requests from the Department Head will be notified to the Dean RSPC.
- All forwarded requests from Dean RSPC will be notified to the Director.
- Once the requests are approved ,it will be notified to the faculty,RSPC admin.

PURCHASE AND STORE MODULE (GAD6)-

- Once the Fund requests are approved ,the purchase store admin will be notified.
