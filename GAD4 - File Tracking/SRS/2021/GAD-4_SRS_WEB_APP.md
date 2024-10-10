**Fusion ERP**

**Software Requirements Specification**

**for**

**GAD- 4 - FILE TRACKING SYSTEM**

**Prepared by:**

Divyansh Tripathi - 21BCS078 Siddhant Raj - 21BCS199 Advay Sagarkar - 21BCS011 Samruddhi Khade - 21BCS115 Bhakti Balanse - 21BCS053 Yash Rastogi - 21BCS249 Aishwarya Saxena - 21BCS013 Kallam Yashwanth - 21BCS106 Venkatesh Kumar - 21BCS127 Sudhanshu - 21BCS210

**Faculty Mentor:** Avinash Chandra Pandey **Student Mentor:**

Priyanshu Agarwal-21bcs167 Vansh Mittal-21bcs234

**1. Introduction**

1. **Introduction about the Fusion – A Brief Description**

Fusion IIIT is a special project at PDPM Indian Institute of Information Technology, Design, and Manufacturing in Jabalpur. It's like a smart helper created by students using Python 3.8 and Django Web framework. The goal is to make things easier and better at the institute.

Fusion IIIT does many things. First, it helps with administrative tasks, making paperwork and processes simpler and more organized. It's like a superhero for efficient management. Second, in academics, it adds a digital touch to make learning better and easily manage courses. But Fusion IIIT doesn't stop there; it helps in different departments and sections, making sure everything runs smoothly on campus.

2. **Purpose of the module:**

The primary objective of the file tracking module is to establish, uphold, and oversee the creation, maintenance, and management of files, while systematically tracking their progress. This module facilitates the seamless transfer and receipt of files related to IIIT work, empowering students, faculty members, or designated individuals to engage in efficient file-related activities within the system.

Designed for simplicity and user interaction, this module aims to create a user-friendly experience for all members utilizing the system. Whether it involves transferring or receiving files pertinent to IIIT-related tasks, the module ensures a smooth and straightforward process, fostering effective collaboration and streamlined file management within the IIIT community.

3. **Scope of the module:**

The scope of the File Tracking System encompasses several key aspects to enhance user experience and ensure security. This includes creating a user-friendly interface tailored for employees, establishing a secure mode for system interactions, and implementing secure processes for file creation, tracking, and visualizing the entire file flow. The system prioritizes secured storage of confidential data on the server and grants appropriate privileges to different authorities. Additionally, it aims to efficiently handle a large number of files. Moreover, authenticated users will have the privilege to modify their account settings, such as the registered email address and login password, contributing to a more personalized and secure user environment.

2. **User/Actor characteristics**
1. **Employee:**

Represents individuals who are employed by the institution such as Faculty and Staff Members who wish to share important files.

**Role:** They are responsible for managing files and attaching extra information so that further actions can be taken on them.

**Specific Functionalities:**

- Create files and attach documents necessary to them
- Receive files from other employees and forward them with documents attached
- Tracks files that are sent or forwarded by the individual to other employees
- Can finish file whose objective has been achieved and send them to archive
- Save unfinished files to draft so that they can be edited later
2. **System Administrator**

**Role:** Supervises and manages the designations of employee accounts **Specific Functionalities:**

- Creating new designations
- Managing mapping of designations of employees
3. **Functional Requirements**
1. **Use Case Diagram**

![](images/Aspose.Words.232da011-4990-4ad8-9884-3da03063bf43.001.jpeg)

**([useCase draw.io](https://app.diagrams.net/#G1zSkuoL04nwgNblDc3lMn0HgREDf1S66O))**

We have incorporated a few changes in the use case diagram by introducing new use cases - view\_inbox, view\_outbox to differentiate between the received and sent files respectively.

The use cases - forward\_file, finish\_file have been included in the view\_inbox giving these functionalities to the user , either to forward the received file or to add remarks placing it to archives.

2. **Use Case Description**

Documentation of various use cases is as follows:



<table><tr><th colspan="1"><b>UC ID</b></th><th colspan="3">UC#1</th></tr>
<tr><td colspan="1"><b>Use case Name</b></td><td colspan="3"><b>create_file</b></td></tr>
<tr><td colspan="1" valign="top"><b>Description</b></td><td colspan="3" valign="top">The "create file" use case allows the employee to create a new file, give a description to it, attach files and add remarks to it. The employee can then send the created file to another employee by entering their name and designation through the Fusion portal.</td></tr>
<tr><td colspan="1" valign="top"><b>Actor</b></td><td colspan="3" valign="top">Employee</td></tr>
<tr><td colspan="1" valign="top"><b>Precondition</b></td><td colspan="3" valign="top">The employee is logged in into the portal.</td></tr>
<tr><td colspan="1" rowspan="4" valign="top"><b>Main Flow</b></td><td colspan="1" valign="top">1</td><td colspan="2" valign="top">The employee navigates to the "create file" section.</td></tr>
<tr><td colspan="1" valign="top">2</td><td colspan="2" valign="top">The system displays the sections to add descriptions, content, remarks and attach files.</td></tr>
<tr><td colspan="1" valign="top">3</td><td colspan="2" valign="top">The employee fills the respective sections and then enters the name and designation of the next employee to whom the file is to be sent.</td></tr>
<tr><td colspan="1" valign="top">4</td><td colspan="2" valign="top">The employee has the option to save the created file as a draft or send it to the next employee. [A1]</td></tr>
<tr><td colspan="1"><b>Post conditions</b> </td><td colspan="3">The created file is sent to the next employee and an entry is made in the tracking section.</td></tr>
<tr><td colspan="1"><b>Alternate Flow</b></td><td colspan="1">A1</td><td colspan="1">1</td><td colspan="1">The file is saved as draft in the drafts folder.</td></tr>
<tr><td colspan="1"><b>Sub Flow</b></td><td colspan="3">NIL</td></tr>
<tr><td colspan="1"><b>Global Alternate Flow</b></td><td colspan="1"></td><td colspan="2" valign="top">NIL</td></tr>
</table>



<table><tr><th colspan="1"><b>UC ID</b></th><th colspan="3">UC#2</th></tr>
<tr><td colspan="1"><b>Use case Name</b></td><td colspan="3"><b>view_drafts</b></td></tr>
<tr><td colspan="1" valign="top"><b>Description</b></td><td colspan="3">The view_drafts use case allows the user to view drafts that have been saved by the user and allows them to complete it.</td></tr>
<tr><td colspan="1"><b>Actor</b></td><td colspan="3">Employee</td></tr>
<tr><td colspan="1" valign="top"><b>Precondition</b></td><td colspan="3" valign="top">The employee is logged in into the system.</td></tr>
<tr><td colspan="1" rowspan="3" valign="top"><b>Main Flow</b></td><td colspan="1" valign="top">1</td><td colspan="2" valign="top">The employee navigates to the "Drafts" section and selects his designation to view the saved drafts</td></tr>
<tr><td colspan="1" valign="top">2</td><td colspan="2" valign="top">The system displays the list of drafts saved by the user.</td></tr>
<tr><td colspan="1" valign="top">3</td><td colspan="2" valign="top">The employee can complete the draft or delete it. [A1][A2]</td></tr>
<tr><td colspan="1" valign="top"><b>Postconditions</b> </td><td colspan="3" valign="top">The created file is sent to the next employee and an entry is made in the tracking section.</td></tr>
<tr><td colspan="1" rowspan="2" valign="top"><b>Alternate Flow</b></td><td colspan="1" valign="top">A1</td><td colspan="1" valign="top">1</td><td colspan="1" valign="top">The user complete the file and sends it to the next user</td></tr>
<tr><td colspan="1" valign="top">A2</td><td colspan="1" valign="top">1</td><td colspan="1" valign="top">The user deletes the draft and it is removed from the drafts section.</td></tr>
<tr><td colspan="1"><b>Sub Flow</b></td><td colspan="3">NIL</td></tr>
<tr><td colspan="1"><b>Global Alternate Flow</b></td><td colspan="1" valign="top">NIL</td><td colspan="2"></td></tr>
</table>


<table><tr><th colspan="1"><b>UC ID</b></th><th colspan="3">UC#3</th></tr>
<tr><td colspan="1" valign="top"><b>Use case Name</b></td><td colspan="3" valign="top"><b>view_inbox</b></td></tr>
<tr><td colspan="1" valign="top"><b>Description</b></td><td colspan="3" valign="top">The view_inbox use case allows the user to view the files that have been received by the user and allows them to add remarks and forward it to the next user.</td></tr>
<tr><td colspan="1" valign="top"><b>Actor</b></td><td colspan="3" valign="top">Employee</td></tr>
<tr><td colspan="1" valign="top"><b>Precondition</b></td><td colspan="3" valign="top">The employee is logged in into the system.</td></tr>
<tr><td colspan="1" rowspan="3" valign="top"><b>Main Flow</b></td><td colspan="1">1</td><td colspan="2">The employee navigates to the "inbox" section and selects his designation to view the inbox</td></tr>
<tr><td colspan="1">2</td><td colspan="2">The system displays the list of files , who sent it along with file ID.</td></tr>
<tr><td colspan="1" valign="top">3</td><td colspan="2" valign="top">The employee can add remarks to the file or forward it to the next employee.[A1][A2]</td></tr>
<tr><td colspan="1" valign="top"><b>Postconditions</b> </td><td colspan="3" valign="top">The file is sent to the next employee and an entry is made in the tracking section.</td></tr>
<tr><td colspan="1" valign="top"><b>Alternate Flow</b></td><td colspan="1" valign="top">A1</td><td colspan="1" valign="top">1</td><td colspan="1" valign="top">The user adds remarks and forwards the file.</td></tr>
</table>



||A2|2|The user reviews the file and forwards it without adding comments.|
| :- | - | - | :- |
|**Sub Flow**|NIL|||
|**Global Alternate Flow**|NIL|||


<table><tr><th colspan="1" valign="top"><b>UC ID</b></th><th colspan="3" valign="top">UC#4</th></tr>
<tr><td colspan="1"><b>Use case Name</b></td><td colspan="3"><b>view_outbox</b></td></tr>
<tr><td colspan="1" valign="top"><b>Description</b></td><td colspan="3" valign="top">The view_outbox use case allows the user to view files that have been sent by them to other employees.</td></tr>
<tr><td colspan="1" valign="top"><b>Actor</b></td><td colspan="3" valign="top">Employee</td></tr>
<tr><td colspan="1"><b>Precondition</b></td><td colspan="3">The employee is logged in into the system.</td></tr>
<tr><td colspan="1" rowspan="2" valign="top"><b>Main Flow</b></td><td colspan="1" valign="top">1</td><td colspan="2" valign="top">The employee navigates to the "Outbox" section and selects his designation to view the files sent.</td></tr>
<tr><td colspan="1" valign="top">2</td><td colspan="2" valign="top">The system displays the list of files sent by the user.[A1]</td></tr>
<tr><td colspan="1"><b>Postconditions</b> </td><td colspan="3">The user has successfully viewed the outbox and now can track the files</td></tr>
<tr><td colspan="1" rowspan="2" valign="top"><b>Alternate Flow</b></td><td colspan="1">A1</td><td colspan="1">1</td><td colspan="1">The user can track the file by seeing the status in outbox.</td></tr>
<tr><td colspan="1"></td><td colspan="1"></td><td colspan="1"></td></tr>
<tr><td colspan="1"><b>Sub Flow</b></td><td colspan="3">NIL</td></tr>
<tr><td colspan="1" valign="top"><b>Global Alternate Flow</b></td><td colspan="1" valign="top">NIL</td><td colspan="2"></td></tr>
</table>


<table><tr><th colspan="1"><b>UC ID</b></th><th colspan="2">UC#5</th></tr>
<tr><td colspan="1"><b>Use case Name</b></td><td colspan="2"><b>create_designation</b></td></tr>
<tr><td colspan="1" valign="top"><b>Description</b></td><td colspan="2" valign="top">The create_designation use case allows the SA to create new users and assign designation to them.</td></tr>
<tr><td colspan="1" valign="top"><b>Actor</b></td><td colspan="2" valign="top">System administrator (SA)</td></tr>
<tr><td colspan="1" valign="top"><b>Precondition</b></td><td colspan="2" valign="top">The administrator is logged in into the system.</td></tr>
<tr><td colspan="1" rowspan="2" valign="top"><b>Main Flow</b></td><td colspan="1" valign="top">1</td><td colspan="1" valign="top">The SA enters the details for the new user such as PFId [A1], email address [A1], full name [A1], password [A1], confirm password [A2] and indicate whether the new user account is of a new system administrator or not.</td></tr>
<tr><td colspan="1">2</td><td colspan="1">Click the “Create User” button. A success message is displayed back.</td></tr>
</table>



<table><tr><th colspan="1"></th><th colspan="1" valign="top">3</th><th colspan="2" valign="top">The SA will be redirected to Dashboard.</th></tr>
<tr><td colspan="1" valign="top"><b>Postconditions</b> </td><td colspan="3" valign="top">A new user will be created successfully and entry will be made into the database.</td></tr>
<tr><td colspan="1" rowspan="2" valign="top"><b>Alternate Flow</b></td><td colspan="1" valign="top">A1</td><td colspan="1" valign="top">1</td><td colspan="1" valign="top">PFId, new password and retype new password fields should not be empty and should contain valid PFid, valid password.</td></tr>
<tr><td colspan="1" valign="top">A2</td><td colspan="1" valign="top">1</td><td colspan="1" valign="top">The confirm (retype) password and password fields must be the same. If not, an error pops up.</td></tr>
<tr><td colspan="1"><b>Sub Flow</b></td><td colspan="3">NIL</td></tr>
<tr><td colspan="1" valign="top"><b>Global Alternate Flow</b></td><td colspan="1" valign="top">NIL</td><td colspan="2"></td></tr>
</table>


<table><tr><th colspan="1"><b>UC ID</b></th><th colspan="3">UC#6</th></tr>
<tr><td colspan="1"><b>Use case Name</b></td><td colspan="3"><b>assign/update designation</b></td></tr>
<tr><td colspan="1" valign="top"><b>Description</b></td><td colspan="3" valign="top">The assign/update designation use case allows the user to view files that have been sent by them to other employees.</td></tr>
<tr><td colspan="1" valign="top"><b>Actor</b></td><td colspan="3" valign="top">System administrator (SA)</td></tr>
<tr><td colspan="1" valign="top"><b>Precondition</b></td><td colspan="3" valign="top">The administrator is logged in into the system.</td></tr>
<tr><td colspan="1" rowspan="2" valign="top"><b>Main Flow</b></td><td colspan="1" valign="top">1</td><td colspan="2" valign="top">The SA assigns or updates the existing designations. [A1][A2]</td></tr>
<tr><td colspan="1" valign="top">2</td><td colspan="2" valign="top">Click the “Save” button. A success message is displayed back.</td></tr>
<tr><td colspan="1"></td><td colspan="1" valign="top">3</td><td colspan="2" valign="top">The SA will be redirected to Dashboard.</td></tr>
<tr><td colspan="1" valign="top"><b>Post conditions</b> </td><td colspan="3" valign="top">The designation is successfully updated and assigned.</td></tr>
<tr><td colspan="1" rowspan="2" valign="top"><b>Alternate Flow</b></td><td colspan="1" valign="top">A1</td><td colspan="1" valign="top">1</td><td colspan="1" valign="top">The SA updates the designation.</td></tr>
<tr><td colspan="1" valign="top">A2</td><td colspan="1" valign="top">1</td><td colspan="1" valign="top">The SA assigns the designation.</td></tr>
<tr><td colspan="1" valign="top"><b>Sub Flow</b></td><td colspan="3" valign="top">NIL</td></tr>
<tr><td colspan="1" valign="top"><b>Global Alternate Flow</b></td><td colspan="1" valign="top">NIL</td><td colspan="2"></td></tr>
</table>
**3.3. Other Functional Requirements**

1. The user should be able to attach a variety of types of files with the file they are sending and should be able to view them easily as well.
1. The user must be able to browse their computer and attach the required attachments to the main file
1. The **Super admin** as well as the System Administrator of Fusion should be able to assign designations and the inbox of the designations should be different as well.
1. The notifications generated should be able to redirect the user into the inbox
1. The file tracking module must be able to integrate multiple workflows into the system.

**3.4 Other constraints**

1. **User Interfaces**

The user interface should comply with the color scheming and dashboard design of the FUSIONIIT. Users should be able to navigate from one functionality to another. Intermodule navigation should be smooth. All the functionalities should be easy to use and no specific training should be required for the usage of the module

2. **Tech Stack Used**
- Django Web Framework
- Django Rest Framework
3. **Business rules**
1. System Administrator can only be able to manage user accounts, but he

cannot perform any operations on their files.

2. Only authenticated users with proper credentials are allowed access to the File

Tracking System of only those files that are associated with them

3. User roles and permissions determine the actions they can perform within the

system.

4. Each file must follow a standardized workflow for processing, ensuring

consistency.

5. Only administrators can modify system-wide settings.
4. **Non-Functional Requirements**

**4.1 Security:**

Ensure data confidentiality and integrity. Role-based authorization provided by Django ensures that users can only perform actions relevant to their designated roles. This ensures that only the authorized users with the correct designation can access the files that are associated with the actor.

5. **Module dependencies with other fusion modules**

**5.1. UI Level**

- The File tracking interface is accessed through the dashboard and therefore has a dependency on the dashboard UI
- The File Tracking System is also dependent on the notifications tab of a user, to showcase notifications when they are received for an incoming file.

**5.2 DB Level Dependencies**

Outbound dependencies:



|Sr No.|DB Model|Owner|User|
| - | - | - | - |
|1|File|file tracking|office\_module|

Inbound dependencies:



|Sr No.|DB Model|Owner|User|
| - | - | - | - |
|1|ExtraInfo|global|file tracking|
|2|Designation|global|file tracking|
|3|HoldsDesignation|global|file tracking|

**5.3. Module Level Dependencies**

- The File Tracking module has a dependency on the notifications module for the generation of notifications.
