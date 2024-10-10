**Fusion ERP** 

**Software Requirements** 

**Specification**

**for**

**GAD 3 – Complaint management system** 

**Faculty Mentor:** Dr. Avinash Chandra Pandey** 

**Prepared by:** Ayushi Mourya (21BCS050) Bachuwar Esha (21BCS052) Kirankumar G (21BCS116) Nidhi Barapatre (21BCS146) Sadanand Jaiswal (21BCS180) 

**Mentor:** Pratik Kumar (21BCS164) 

1. **Introduction** 
1. **Introduction about the Fusion – A brief Description** 

   FusionIIIT stands as a testament to the seamless integration and automation of diverse functions  within  PDPM  Indian  Institute  of  Information  Technology,  Design  and Manufacturing, Jabalpur. Crafted with precision using Python 3.8 and powered by the Django Web framework, this initiative is a student-driven endeavor designed to elevate the  institute's  operational  landscape.  Encompassing  everything  from  efficient administration  management  to  academic  prowess  and  miscellaneous  departmental tasks, FusionIIIT is a holistic solution that harmonizes the intricacies of campus life. 

   Imagine  it  as  a  digital  wizard  that  takes  care  of  everything,  from  organizing  the administrative stuff to making academics smoother. It's not just limited to the usual tasks; FusionIIIT jumps into various departments and sections, making sure every corner of campus life runs smoothly. 

   In the admin side, it handles the complicated paperwork and processes. For academics, it brings a digital touch, making learning and managing courses easier. But it doesn't stop there; FusionIIIT is like a friendly companion for all the different parts of the campus, making sure everything works well. 

   In simpler terms, FusionIIIT is not just a tool – it's a helpful friend, making life at PDPM IIITDM Jabalpur more organized and enjoyable for everyone. 

2. **Purpose of the module:** 

   The Centralized complaint system combines the issues related to Computer Center, Hostels and Cleanliness under one roof. This software aims at solving problems of students as well as staff as soon as possible by providing a platform to connect them directly to the Warden/Caretaker/Supervisor of the respective departments. It will allow immediate addressal of complaints

3. **Scope of the module:** 

   This module aims to provide a comprehensive solution for efficiently managing and documenting user complaints within our institute. This system is designed to replace traditional paper-based complaint tracking methods, ensuring a centralized and organized approach to handling user complaints and their feedback. 

2. **User / Actor characteristics** 
1. **User (Student, Faculty, Staff):** 

   Represents individuals who intend to lodge a complaint regarding various issues of hostels.** 

   **Specific Functionalities:**  

- Users can lodge complaints. 
- Users can track status of their complaints. 
- Users can give feedback. 
2. **Admin /Section Incharge:** 

   Represents individuals who intend to respond to complaint registered by the Users only when the complaint has been forwarded by the caretaker or not been handled by the caretaker within a specified time period. 

   **Specific Functionalities:** 

- Admin/ Section Incharge can respond to the complaints. 
- Admin/ Section Incharge can change the status of complaint 
3. **Caretaker:** 

   Represents individuals who will be receiving all the complaints and taking actions accordingly. If the complaint remains unresolved or can not be handled at this level, it will be forwarded to the higher concerned authorities (Admin/ Section Incharge). 

   **Specific Functionalities:** 

- Caretaker can view the complaints registered by the users. 
- Caretaker can respond to the complaints. 
- Caretaker can forward the complaints to the respective higher authorities. 
3. **Functional Requirements** 
1. **Use Case Diagram** 

The figure represents the use case diagram for the module features.  

![](images/Aspose.Words.0836ae2b-c725-4d49-9436-629a9edfa807.001.jpeg)

2. **Use Case Description: 3.2.1: Use Case #1** 

 

<table><tr><th colspan="1" valign="top"><b>UC  ID</b></th><th colspan="2" valign="top">UC#1</th></tr>
<tr><td colspan="1" valign="top"><b>Use Case Name</b></td><td colspan="2"><b>lodge_complaint</b> </td></tr>
<tr><td colspan="1" valign="top"><b>Actor</b></td><td colspan="2" valign="top">Student, Staff, Faculty</td></tr>
<tr><td colspan="1" valign="top"><b>Pre-Condition</b></td><td colspan="2" valign="top">The user must fill the all the necessary fields in the complaint page.</td></tr>
<tr><td colspan="1" rowspan="2" valign="top"><b>Main Flow</b></td><td colspan="1" valign="top">1\. </td><td colspan="1" valign="top">User fills all the necessary columns and clicks on the submit button.</td></tr>
<tr><td colspan="1">2\.</b> </td><td colspan="1" valign="top">System displays a message that complaint has been successfully received.</td></tr>
<tr><td colspan="1" valign="top"><b>Post-Condition</b></td><td colspan="2" valign="top">The complaint is successfully received by the system and stored in the database.</td></tr>
</table>

**3.2.2: Use Case #2** 



<table><tr><th colspan="1" valign="top"><b>UC ID</b></th><th colspan="2" valign="top">UC#2</th></tr>
<tr><td colspan="1" valign="top"><b>Use Case Name</b></td><td colspan="2"><b>track_Status</b> </td></tr>
<tr><td colspan="1" valign="top"><b>Description</b></td><td colspan="2" valign="top">After logging into the system, the user can see the complaint history and the status of the respective complaints.</td></tr>
<tr><td colspan="1" valign="top"><b>Actor</b></td><td colspan="2" valign="top">Student, Staff, Faculty</td></tr>
<tr><td colspan="1" valign="top"><b>Pre-Condition</b> </td><td colspan="2" valign="top">User must be logged-in. </td></tr>
<tr><td colspan="1" rowspan="3" valign="top"><b>Main Flow</b></td><td colspan="1" valign="top">1\. </td><td colspan="1" valign="top">User choose the Complaint History to check the status of the complaints.</td></tr>
<tr><td colspan="1" valign="top">2\. </td><td colspan="1" valign="top">System displays the page showing the status of all the complaints i.e whether the complaint has been addressed by the caretaker or not, with the time and date when the user had registered the complaint.</td></tr>
<tr><td colspan="1" valign="top">3\.</td><td colspan="1" valign="top">User can see which of his complaints are resolved, kept on-hold  and complaints that are declined. </td></tr>
<tr><td colspan="1" valign="top"><b>Alternate Flow</b></td><td colspan="2" valign="top">NIL</td></tr>
</table>

**3.2.3: Use Case #3** 
<table><tr><th colspan="1" valign="top"><b>UC ID</b></th><th colspan="2" valign="top">UC#3</th></tr>
<tr><td colspan="1" valign="top"><b>Use Case Name</b></td><td colspan="2"><b>give_feedback</b> </td></tr>
<tr><td colspan="1" valign="top"><b>Description</b></td><td colspan="2" valign="top">User has the option to give feedbacks to the service after his/her complaint has been resolved.</td></tr>
<tr><td colspan="1" valign="top"><b>Actors</b></td><td colspan="2" valign="top">Student, Staff, Faculty</td></tr>
<tr><td colspan="1" valign="top"><b>Pre-Condition</b> </td><td colspan="2" valign="top">User must be logged-in. </td></tr>
<tr><td colspan="1" rowspan="6" valign="top"><b>Main Flow</b></td><td colspan="1" valign="top">1\. </td><td colspan="1" valign="top">User chooses the feedback option given on the first page.</td></tr>
<tr><td colspan="1" valign="top">2\. </td><td colspan="1" valign="top">System shows the next page.</td></tr>
<tr><td colspan="1" valign="top">3\. </td><td colspan="1" valign="top">User choose the type of feedback i.e whether the feedback is about CC (Library+CC), hostel, residential or garbage. </td></tr>
<tr><td colspan="1" valign="top">4\.  </td><td colspan="1" valign="bottom">User gives the feedback. </td></tr>
<tr><td colspan="1" valign="top">5\.  </td><td colspan="1" valign="bottom">User submits the feedback. </td></tr>
<tr><td colspan="1" valign="top">6\. </td><td colspan="1" valign="bottom">System displays the initial page. </td></tr>
<tr><td colspan="1" valign="top"><b>Post-Condition</b> </td><td colspan="2" valign="top">Feedback is successfully received by the system and stored in the database.  </td></tr>
<tr><td colspan="1" valign="top"><b>Alternate Flow</b></td><td colspan="2" valign="top">NILL</td></tr>
</table>

4. **Use Case #4** 
<table><tr><th colspan="1" valign="top"><b>UC ID</b></th><th colspan="2" valign="top">UC#4</th></tr>
<tr><td colspan="1" valign="top"><b>Use case Name</b></td><td colspan="2"><b>change_status</b> </td></tr>
<tr><td colspan="1" valign="top"><b>Description</b></td><td colspan="2" valign="top">Admin/Section Incharge can change the status of the complaint. </td></tr>
<tr><td colspan="1" valign="top"><b>Actor</b></td><td colspan="2" valign="top">Admin/Section Incharge </td></tr>
<tr><td colspan="1" valign="top"><b>Pre-Condition</b> </td><td colspan="2" valign="top">The user must be logged-in. Then he/she must click on the unresolved complaints thereafter on Hold Complaints. </td></tr>
<tr><td colspan="1" rowspan="3" valign="top"><b>Main Flow</b></td><td colspan="1" valign="top">1\. </td><td colspan="1" valign="top">System displays the page of on hold complaints.</td></tr>
<tr><td colspan="1" valign="top">2\. </td><td colspan="1" valign="top">User clicks on the change status button at the corner.</td></tr>
<tr><td colspan="1" valign="top">3\. </td><td colspan="1" valign="top">User changes the state of work from unresolved to resolved. </td></tr>
<tr><td colspan="1" valign="top"><b>Post-Condition</b> </td><td colspan="2" valign="top">Student/Staff gets notified with the changed status of the complaint. </td></tr>
<tr><td colspan="1" valign="top"><b>Alternate Flow</b></td><td colspan="2" valign="top">NIL</td></tr>
</table>

5. **Use Case #5:** 



<table><tr><th colspan="1" valign="top"><b>UC ID</b></th><th colspan="2" valign="top">UC#5</th></tr>
<tr><td colspan="1" valign="top"><b>Use case Name</b></td><td colspan="2"><b>respond_to_complaint</b> </td></tr>
<tr><td colspan="1" valign="top"><b>Description</b></td><td colspan="2" valign="top">Enables Admin/Section Incharge to efficiently respond to a complaint forwarded by the caretaker.</td></tr>
<tr><td colspan="1" valign="top"><b>Actor</b></td><td colspan="2" valign="top">Admin/Section Incharge</td></tr>
<tr><td colspan="1" valign="top"><b>Pre-Condition</b> </td><td colspan="2" valign="top">The user must be logged-in. There should be an existing unresolved complaint. </td></tr>
<tr><td colspan="1" rowspan="3" valign="top"><b>Main Flow</b></td><td colspan="1" valign="top">1\.   </td><td colspan="1" valign="top">`  `User navigates to the “View Complaint” section.</td></tr>
<tr><td colspan="1" valign="top">2\. </td><td colspan="1" valign="top">Chooses a complaint.</td></tr>
<tr><td colspan="1" valign="top">3\. </td><td colspan="1" valign="top">Drafts and submits a response to the complaint. </td></tr>
<tr><td colspan="1" valign="top"><b>Post-Condition</b> </td><td colspan="2" valign="top">Successfully respond to the complaint. </td></tr>
<tr><td colspan="1" valign="top"><b>Alternate Flow</b></td><td colspan="2" valign="top">If no complaints are available the system notifies the admin / section incharge that there are no complaints to view.</td></tr>
</table>

6. **Use Case #6** 
<table><tr><th colspan="1" valign="top"><b>UC ID</b></th><th colspan="2" valign="top">UC#6</th></tr>
<tr><td colspan="1" valign="top"><b>Use case Name</b></td><td colspan="2"><b>view_complaint</b> </td></tr>
<tr><td colspan="1" valign="top"><b>Description</b></td><td colspan="2" valign="top">Caretaker can view the complaint detail.</td></tr>
<tr><td colspan="1" valign="top"><b>Actor</b></td><td colspan="2" valign="top">Caretaker </td></tr>
<tr><td colspan="1" valign="top"><b>Pre-Condition</b> </td><td colspan="2" valign="top">The Caretaker must be logged-in. There should be existing complaint submitted by the User. </td></tr>
<tr><td colspan="1" rowspan="3" valign="top"><b>Main Flow</b></td><td colspan="1" valign="top">1\. </td><td colspan="1" valign="top">Caretaker login into the Complain Management System.</td></tr>
<tr><td colspan="1" valign="top">2\. </td><td colspan="1" valign="top">Navigates to the “View Complaint” section.</td></tr>
<tr><td colspan="1" valign="top">3\. </td><td colspan="1" valign="top">Selects a complaint from the list. </td></tr>
<tr><td colspan="1" valign="top"><b>Post-Condition</b> </td><td colspan="2" valign="top">NIL </td></tr>
<tr><td colspan="1" valign="top"><b>Alternate Flow</b></td><td colspan="2" valign="top">If no complaints are available the system notifies the care taker that there are no complaints to view.</td></tr>
</table>

6. **Use Case #7:** 



<table><tr><th colspan="1" valign="top"><b>UC ID</b></th><th colspan="2" valign="top">UC#7</th></tr>
<tr><td colspan="1" valign="top"><b>Use case Name</b></td><td colspan="2"><b>forward / respond</b> </td></tr>
<tr><td colspan="1" valign="top"><b>Description</b></td><td colspan="2" valign="top">Caretaker can forward the complaint to concerned higher authorities or respond to the complaint if it has been resolved or will be resolved without the interference of higher authorities.</td></tr>
<tr><td colspan="1" valign="top"><b>Actor</b></td><td colspan="2" valign="top">Caretaker </td></tr>
<tr><td colspan="1" valign="top"><b>Pre-Condition</b> </td><td colspan="2" valign="top">The Caretaker must be logged-in. There should be an existing complaint that needs to be forwarded. </td></tr>
<tr><td colspan="1" rowspan="2" valign="top"><b>Main Flow</b></td><td colspan="1" valign="top">1\. </td><td colspan="1" valign="top">User navigates to the “View Complaint” section.</td></tr>
<tr><td colspan="1" valign="top">2\. </td><td colspan="1" valign="top">Choose a complaint and either forward or respond by changing the status.</td></tr>
<tr><td colspan="1" valign="top"><b>Post-Condition</b> </td><td colspan="2" valign="top">The Caretaker may update the complaint status. </td></tr>
<tr><td colspan="1" valign="top"><b>Alternate Flow</b></td><td colspan="2" valign="top">If no complaints are available the system notifies the care taker that there are no complaints to view.</td></tr>
</table>


3. **Other Functional Requirements** 
- This module will use notification and alert to notify the complaints to respective actors. 
- This software should be compatible with different browsers like Google Chrome, Firefox, Edge and Safari. Users should be able to use and navigate on any browser available.
4. **Other Constraints:** 
1. **User Interface:** 

The color palette should match the design and pattern of the FusionIIIT dashboard. All the buttons should be clickable and there should be smooth navigation from one functionality to another. Inter module navigation should be reachable from within the module. The UI should be easy to use and intuitive. 

2. **Tech Stack:** 

Web  application  uses  Django  framework  for  frontend  and  backend  functionality. PostgreSQL is used as the RDBMS. 

4. **Non-Functional requirements** 
1. **Ensuring security**  

The user has to login before he/she could access anything or make a complaint. Admin can only make changes in the categories of complaints and other related issues. Access to any application resource will depend upon user’s designation. 

2. **Performance Requirements** 

The server on which the website and database are hosted must be online 24X7.It must be able to  handle multiple requests of different  users at  a time. Response time of the complaint management system should be less. Response time refers to the waiting time while the system accesses queries and retrieves the information from the database**.**  

3. **Reliability**  

It should be robust with high degree of fault tolerance. Any user error should be identified and user should be notified about it.  It should have mechanisms to overcome hardware failures, power failures and roll back databases to their last checkpoint. This application should be highly reliable and it should generate all the updated information by student, faculty and administrator in correct order. 

4. **Usability**  

The interface should be easy to use. The web interface should be intuitive and easy to navigate. Users should be able to understand the menu and options provided by the software. Any notification or error messages should be precise and clear. The software should be able to understand and capable to learn, Use and attractive to the user when used under specified condition.  

**5 Module dependencies with other fusion modules** 

1. **UI Level :** 

` `Users log in to the Fusion application and are presented with the main dashboard. The user (student, staff, faculty) can lodge a complaint by filling the required input fields. They can also view their respective complaint history. 

2. **Database Level:** 

`      `Following are the tables and their respective dependencies. 



|**S.no** |**Table Name** |**Foreign key** |**Referenced Table** |
| - | - | - | - |
|1 |complaint\_system\_caretaker |staff\_id\_id |globals\_extrainfo |
|2 |complaint\_system\_hall|staff\_id\_id |globals\_extrainfo |
|3 |complaint\_system\_studentcomplaint |complainer\_id |globals\_extrainfo |
|||worker\_id\_id |complaint\_system\_workers |
|4 |complaint\_system\_supervisor|sup\_id\_id |globals\_extrainfo |
|5 |complaint\_system\_workers|caretaker\_id\_id |complaint\_system\_caretaker |

3. **Module Level:** 
- **Notification:** 

  Dependency Direction: Complaint management system Module depends on Notifications Extension. 

  **Purpose:** To trigger notification when a complaint is registered or solved. 

- **Dashboard:** 

  Dependency Direction: Complaint management system Module depends on Dashboard Extension. 

  **Purpose**:  To  provide  a  unified  and  real-time  interface  for  monitoring,  tracking,  and resolving complaints. 

- **FTS:**

  Dependency  Direction:  Complaint  management  system  Module  depends  on  FTS Extension.  
