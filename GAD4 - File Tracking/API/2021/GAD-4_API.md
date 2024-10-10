**MODULE: FILE TRACKING GAD-4**

**Student Mentor:**

Priyanshu Agarwal - 21BCS167 Vansh Mittal - 21BCS234

**Prepared by:** Divyansh Tripathi - 21BCS078 Siddhant Raj - 21BCS199 Advay Sagarkar - 21BCS011 Samruddhi Khade - 21BCS115 Bhakti Balanse - 21BCS053

WEB API DOCUMENTATION

**Module Description:-**

The primary objective of the file tracking module is to establish, uphold, and oversee the creation, maintenance, and management of files, while systematically tracking their progress. This module facilitates the seamless transfer and receipt of files related to IIIT work, empowering students, faculty members, or designated individuals to engage in efficient file-related activities within the system.

The System allows people to share, view, track, and forward files and can be used by other modules to implement a specific ‘file-motion’ workflow.

Main Actors in this module are:-

- **Employee (Staff)**
- **System Administrator**

**APIs Used and Status:- VIEWS STATUS**:-

These are the already implemented web views that serve, static-rendered templates. There are minor bugs in some of the views but the implementation and logic are otherwise updated.

1. **filetracking(request):** Already implemented
1. **drafts(request):** Already implemented
1. **fileview(request,id):** Already implemented
4. **fileview1(request,id):** Already implemented
4. **fileview2(request,id):** Already implemented
4. **outward(request,id):** Already implemented
4. **inward(request,id):** Already implemented
4. **confirmdelete(request,id):** Already implemented
4. **forward(request,id):** Already implemented **10.archive\_design(request):** Already implemented **11.archive(request,id):** Already implemented **12.archive\_finish(request,id):** Already implemented **13.finish\_design(request):** Already implemented **14.finish\_fileview(request,id):** Already implemented **15.finish(request,id):** Already implemented **16.AjaxDropdown1(request):** Already implemented **17.AjaxDropdown(request):** Already implemented **18.test(request):** Already implemented **19.delete(request,id):** Already implemented **20.forward\_inward(request,id):**Already implemented
- [GAD-4 File Tracking Use Cases](https://docs.google.com/document/d/1Ow-XYX79gOBDzpJQiwQI5FPUiqClaqF7wMN2-ogirXE/edit?usp=sharing)
- *create\_file - UC#1*
- Index of views used - 1,9,13,14,15,16,17,18
- Description - allows the employee to create a new file, give a description to it, attach files and add remarks to it.
- Database - File, Tracking, Designation, HoldsDesignation, User, ExtraInfo
- *view\_drafts - UC#2*
- Index of views used - 2,3,8,10,11,12,18,19
- Description - allows the user to view drafts that have been saved by the user and allows them to complete it.
- Database - File, HoldsDesignation, User, ExtraInfo
- *view\_inbox - UC#3*
- Index of views used - 5,7,8,9,13,14,15,18,19,20
- Description - allows the user to view the files that have been received by the user and allows them to add remarks and forward it to the next user.
- Database - File, Tracking,HoldsDesignation, User, ExtraInfo
- *view\_outbox - UC#4*
- Index of views used - 4,6,8,18,19
- Description -allows the user to view files that have been sent by them to other employees.
- Database - File, Tracking, Designation, HoldsDesignation, User, ExtraInfo

**DETAILED VIEW EXPLANATION:-**

- **filetracking(request):-**
- Use case (as per SRS):- **UC#1**
- Purpose:-
  - Handles file creation and tracking within the application.
  - Requires user authentication for access.
- Database:- File, Tracking, Designation, HoldsDesignation, User, ExtraInfo
- **drafts(request):-**
- Use case (as per SRS):- **UC#2**
- Purpose:-
  - Retrieves the user's designation and renders it on the "drafts" template.
  - Requires user authentication for access.
- Database:- Designation.
- **fileview(request,id):-**
- Use case (as per SRS):- **UC#2**
- Purpose:-
  - Displays files created by the user, specifically those without tracking entries (likely drafts).
  - Requires user authentication for access.
- Database:- ExtraInfo,file, Tracking, HoldsDesignation
- **fileview1(request,id):-**
- Use case (as per SRS):- **UC#4**
- Purpose:-
- Displays files sent by the user to others, serving as an "Outbox" feature.
- Requires user authentication for access.
- Database:- Tracking, HoldsDesignation.
- **fileview2(request,id):-**
- Use case (as per SRS):- **UC#3**
- Purpose:-
  - Displays files received by the user from others, serving as an "Inbox" feature.
  - Requires user authentication for access.
- Database:- Tracking, HoldsDesignation.
- **outward(request):-**
- Use case (as per SRS):- **UC#4**
- Purpose:-
  - Fetches the different designations held by the user and renders them on the "outward" template.
  - Requires user authentication for access.
- Database:- designation.
- **inward(request):-**
- Use case (as per SRS):- **UC#3**
- Purpose:-
  - Fetches the different designations held by the user and renders them on the "inward" template.
  - Requires user authentication for access.
- Database:- designation.
- **confirmdelete(request,id):-**
- Use case (as per SRS):- **UC#2,UC#3,UC#4**
- Purpose:-
  - Displays a file deletion confirmation page for a specific file.
  - Requires user authentication for access.
  - Serves as an intermediary step before actual deletion, allowing user confirmation.
- Database:- File
- **forward(request,id):-**
- Use case (as per SRS):- **UC#1, UC#3**
- Purpose:-
- Handles forwarding of received files, including marking as read, adding remarks and attachments, and recording forwarding events in the "Tracking" model.
- Database:- File, Tracking, HoldsDesignation, User, Designation,
- **archive\_design(request):**
- Use case (as per SRS):- **UC#2**
- Purpose:-
  - Renders the "archive\_design" template, providing the user's designations for selection or display.
  - Likely serves as the initial step in an archive-related process.
  - Requires user authentication for access.
  - Employs select\_related for optimized database queries.
- Database:- HoldsDesignation
- **archive(request, id):-**
- Use case (as per SRS):- **UC#2**
- Purpose:-
  - Displays a list of archived files, likely for viewing or further actions.
  - Requires user authentication for access.
- Database:- File, HoldsDesignation, ExtraInfo
- **archive\_finish(request, id):-**
- Use case (as per SRS):- **UC#2**
- Purpose:-
  - Renders details of a specific archived file, likely for review or final actions.
  - Requires user authentication for access.
- Database:- File, Tracking
- **finish\_design(request):-**
- Use case (as per SRS):- **UC#1, UC#3**
- Purpose:-
  - Renders the "finish\_design" template, providing the user's designations for selection or display.
  - Serves as the initial step in a process related to finalizing files.
  - Requires user authentication for access.
  - Interacts primarily with the "HoldsDesignation" model to retrieve designation information.
  - Employs **select\_related** for optimized database queries.
  - The specific file finalization logic is handled by a separate view or function, triggered from the "finish\_design" template.
- Database:- HoldsDesignation
- **finish\_fileview(request, id):-**
- Use case (as per SRS):- **UC#1,UC#3**
- Purpose:-
  - Displays a list of files awaiting finalization, specifically those uploaded by the current user and not yet read by any recipient.
  - Serves as a step in the file finalization process.
  - Requires user authentication for access.
  - Filters for files awaiting finalization based on recipient reading status.
- Database:- tracking, designation
- **finish(request, id):-**
- Use case (as per SRS):- **UC#1, UC#3**
- Purpose:-
  - Finalizes a specific file, marking it as read and archiving it.
  - Requires user authentication for access.
  - The template displays file details and tracking history for final review before archiving.
- Database:- file, tracking
- **AjaxDropdown1(request):-**
- Use case (as per SRS):- **UC#1**
- Purpose:-
- Handles AJAX requests to provide dynamic designation suggestions for receiver fields in forward or compose file forms.
- Designed to be called via AJAX from front-end components.
- This view enables dynamic, user-friendly designation selection without full page reloads.
- **AjaxDropdown(request):-**
- Use case (as per SRS):- **UC#1**
- Purpose:-
- Handles AJAX requests to provide dynamic username suggestions for receiver fields in forward or compose file forms.
- Designed to be called via AJAX from front-end components.
- The retrieved usernames are likely used to populate a dropdown list or similar UI element in the forward or compose file form.
- This view, along with AjaxDropdown1, enables a dynamic user experience for selecting receivers without full page reloads.
- **test(request):-**
- Use case (as per SRS):- **all**
- Purpose:-
- Serves as a simple test view for checking server functionality or debugging purposes.
- **delete(request, id):-**
- Use case (as per SRS):- **UC#2,UC#3,UC#4**
- Purpose:-
  - Deletes a specified file and redirects the user to the drafts page.
  - Requires user authentication for access.
  - Assumes that the drafts page is implemented at the specified URL.
- Database:- file
- **forward\_inward(request, id):-**
- Use case (as per SRS):- **UC#3**
- Purpose:-
  - Initiates the forwarding process for a file received in the user's inbox.
  - Prepares data for rendering the "forward" template, where the user can select recipients and add remarks.
  - Employs select\_related for optimized database queries.
  - The actual forwarding logic (creating a new tracking entry) is handled by a separate view or function, triggered when the user submits data in the "forward" template.
- Database:- File, Tracking, Designation

**Current problems you are facing with the module or in its use cases —**

- [Use Case #3]: **view\_inbox ← archive\_file** -> This use can be implemented using a PATCH request endpoint as used in the front end but its interaction with other modules needs to be considered.
- [Use Case #2]: The logic of drafts needs to be implemented separately for each module and is only implemented for the filetracking module currently.

[Google Doc Link:[ GAD-4 FileTracking API ](https://docs.google.com/document/d/1kp8H_cpCyEAWIONtiNtKNlnxLBp5mJ1nHHxrCkYQoFU/edit)]
