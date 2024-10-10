# MODULE: FILE TRACKING GAD-4

## Student Mentor:
- Priyanshu Agarwal - 21BCS167
- Vansh Mittal - 21BCS234

## Prepared by:
- Divyansh Tripathi - 21BCS078
- Siddhant Raj - 21BCS199
- Advay Sagarkar - 21BCS011
- Samruddhi Khade - 21BCS115
- Bhakti Balanse - 21BCS053

---

## WEB API DOCUMENTATION

### Module Description:
The primary objective of the file tracking module is to establish, uphold, and oversee the creation, maintenance, and management of files, while systematically tracking their progress. This module facilitates the seamless transfer and receipt of files related to IIIT work, empowering students, faculty members, or designated individuals to engage in efficient file-related activities within the system.

The System allows people to share, view, track, and forward files and can be used by other modules to implement a specific ‘file-motion’ workflow.

### Main Actors in this module are:
- **Employee (Staff)**
- **System Administrator**

---

### APIs Used and Status: VIEWS STATUS
These are the already implemented web views that serve static-rendered templates. There are minor bugs in some of the views but the implementation and logic are otherwise updated.

1. **filetracking(request):** Already implemented
2. **drafts(request):** Already implemented
3. **fileview(request,id):** Already implemented
4. **fileview1(request,id):** Already implemented
5. **fileview2(request,id):** Already implemented
6. **outward(request,id):** Already implemented
7. **inward(request,id):** Already implemented
8. **confirmdelete(request,id):** Already implemented
9. **forward(request,id):** Already implemented
10. **archive_design(request):** Already implemented
11. **archive(request,id):** Already implemented
12. **archive_finish(request,id):** Already implemented
13. **finish_design(request):** Already implemented
14. **finish_fileview(request,id):** Already implemented
15. **finish(request,id):** Already implemented
16. **AjaxDropdown1(request):** Already implemented
17. **AjaxDropdown(request):** Already implemented
18. **test(request):** Already implemented
19. **delete(request,id):** Already implemented
20. **forward_inward(request,id):** Already implemented

- [GAD-4 File Tracking Use Cases](https://docs.google.com/document/d/1Ow-XYX79gOBDzpJQiwQI5FPUiqClaqF7wMN2-ogirXE/edit?usp=sharing)

---

### Use Cases
- **create_file - UC#1**
  - Index of views used: 1, 9, 13, 14, 15, 16, 17, 18
  - **Description:** Allows the employee to create a new file, give a description to it, attach files, and add remarks to it.
  - **Database:** File, Tracking, Designation, HoldsDesignation, User, ExtraInfo

- **view_drafts - UC#2**
  - Index of views used: 2, 3, 8, 10, 11, 12, 18, 19
  - **Description:** Allows the user to view drafts that have been saved by the user and allows them to complete it.
  - **Database:** File, HoldsDesignation, User, ExtraInfo

- **view_inbox - UC#3**
  - Index of views used: 5, 7, 8, 9, 13, 14, 15, 18, 19, 20
  - **Description:** Allows the user to view the files that have been received by the user and allows them to add remarks and forward it to the next user.
  - **Database:** File, Tracking, HoldsDesignation, User, ExtraInfo

- **view_outbox - UC#4**
  - Index of views used: 4, 6, 8, 18, 19
  - **Description:** Allows the user to view files that have been sent by them to other employees.
  - **Database:** File, Tracking, Designation, HoldsDesignation, User, ExtraInfo

---

### DETAILED VIEW EXPLANATION

- **filetracking(request):**
  - **Use case (as per SRS):** UC#1
  - **Purpose:**
    - Handles file creation and tracking within the application.
    - Requires user authentication for access.
  - **Database:** File, Tracking, Designation, HoldsDesignation, User, ExtraInfo

- **drafts(request):**
  - **Use case (as per SRS):** UC#2
  - **Purpose:**
    - Retrieves the user's designation and renders it on the "drafts" template.
    - Requires user authentication for access.
  - **Database:** Designation.

- **fileview(request,id):**
  - **Use case (as per SRS):** UC#2
  - **Purpose:**
    - Displays files created by the user, specifically those without tracking entries (likely drafts).
    - Requires user authentication for access.
  - **Database:** ExtraInfo, file, Tracking, HoldsDesignation

- **fileview1(request,id):**
  - **Use case (as per SRS):** UC#4
  - **Purpose:**
    - Displays files sent by the user to others, serving as an "Outbox" feature.
    - Requires user authentication for access.
  - **Database:** Tracking, HoldsDesignation.

- **fileview2(request,id):**
  - **Use case (as per SRS):** UC#3
  - **Purpose:**
    - Displays files received by the user from others, serving as an "Inbox" feature.
    - Requires user authentication for access.
  - **Database:** Tracking, HoldsDesignation.

- **outward(request):**
  - **Use case (as per SRS):** UC#4
  - **Purpose:**
    - Fetches the different designations held by the user and renders them on the "outward" template.
    - Requires user authentication for access.
  - **Database:** Designation.

- **inward(request):**
  - **Use case (as per SRS):** UC#3
  - **Purpose:**
    - Fetches the different designations held by the user and renders them on the "inward" template.
    - Requires user authentication for access.
  - **Database:** Designation.

- **confirmdelete(request,id):**
  - **Use case (as per SRS):** UC#2, UC#3, UC#4
  - **Purpose:**
    - Displays a file deletion confirmation page for a specific file.
    - Requires user authentication for access.
    - Serves as an intermediary step before actual deletion, allowing user confirmation.
  - **Database:** File

- **forward(request,id):**
  - **Use case (as per SRS):** UC#1, UC#3
  - **Purpose:**
    - Handles forwarding of received files, including marking as read, adding remarks and attachments, and recording forwarding events in the "Tracking" model.
  - **Database:** File, Tracking, HoldsDesignation, User, Designation.

- **archive_design(request):**
  - **Use case (as per SRS):** UC#2
  - **Purpose:**
    - Renders the "archive_design" template, providing the user's designations for selection or display.
    - Likely serves as the initial step in an archive-related process.
    - Requires user authentication for access.
    - Employs select_related for optimized database queries.
  - **Database:** HoldsDesignation

- **archive(request, id):**
  - **Use case (as per SRS):** UC#2
  - **Purpose:**
    - Displays a list of archived files, likely for viewing or further actions.
    - Requires user authentication for access.
  - **Database:** File, HoldsDesignation, ExtraInfo

- **archive_finish(request, id):**
  - **Use case (as per SRS):** UC#2
  - **Purpose:**
    - Renders details of a specific archived file, likely for review or final actions.
    - Requires user authentication for access.
  - **Database:** File, Tracking

- **finish_design(request):**
  - **Use case (as per SRS):** UC#1, UC#3
  - **Purpose:**
    - Renders the "finish_design" template, providing the user's designations for selection or display.
    - Serves as the initial step in a process related to finalizing files.
    - Requires user authentication for access.
    - Interacts primarily with the "HoldsDesignation" model to retrieve designation information.
    - Employs select_related for optimized database queries.
    - The specific file finalization logic is handled by a separate view or function, triggered from the "finish_design" template.
  - **Database:** HoldsDesignation

- **finish_fileview(request, id):**
  - **Use case (as per SRS):** UC#1, UC#3
  - **Purpose:**
    - Displays a list of files awaiting finalization, specifically those uploaded by the current user and not yet read by any recipient.
    - Serves as a step in the file finalization process.
    - Requires user authentication for access.
    - The list likely serves as a reference for the user to proceed with finalizing specific files.
  - **Database:** File, Tracking

- **finish(request, id):**
  - **Use case (as per SRS):** UC#1, UC#3
  - **Purpose:**
    - Finalizes a file by marking it as completed within the system, updating its status and associated tracking information.
    - Requires user authentication for access.
    - Interacts with the "Tracking" model to update file status and may also involve notifying relevant parties or logging actions for audit purposes.
  - **Database:** File, Tracking

- **AjaxDropdown1(request):**
  - **Use case (as per SRS):** UC#1
  - **Purpose:**
    - Serves as an endpoint for fetching dropdown options dynamically, likely for forms within the module.
    - Facilitates user interactions by providing real-time selections based on existing data.
    - Can be utilized by JavaScript on the frontend for seamless user experience.
  - **Database:** Designation

- **AjaxDropdown(request):**
  - **Use case (as per SRS):** UC#1
  - **Purpose:**
    - Similar to `AjaxDropdown1`, this endpoint likely serves a different set of dropdown options or data for dynamic forms.
    - Enhances user experience by enabling live updates of selectable options based on user input or selections.
  - **Database:** HoldsDesignation

- **test(request):**
  - **Use case (as per SRS):** UC#1
  - **Purpose:**
    - A test endpoint used for development and debugging purposes, possibly for testing AJAX calls or form submissions.
    - Likely not a part of the final module but serves to ensure that individual components are functioning correctly.
  - **Database:** None

- **delete(request, id):**
  - **Use case (as per SRS):** UC#2, UC#3, UC#4
  - **Purpose:**
    - Permanently deletes a specified file from the system, requiring user confirmation before proceeding.
    - Essential for maintaining file management and preventing unauthorized deletions.
    - Requires user authentication for access.
  - **Database:** File

- **forward_inward(request, id):**
  - **Use case (as per SRS):** UC#1, UC#3
  - **Purpose:**
    - Similar to the `forward` function, but specifically handles the forwarding of inward files, with tracking and remarks as necessary.
  - **Database:** File, Tracking, HoldsDesignation, User, Designation

# CURRENT PROBLEMS WITH THE FILE TRACKING MODULE (GAD-4)

## Issues Identified

1. **Use Case #3: `view_inbox ← archive_file`**
   - **Description:** This use case can be implemented using a PATCH request endpoint as utilized in the front end. 
   - **Considerations:** Its interaction with other modules needs to be taken into account to ensure seamless functionality.

2. **Use Case #2: Drafts Logic Implementation**
   - **Description:** The logic for handling drafts needs to be implemented separately for each module. 
   - **Current Status:** The drafts logic is currently only implemented for the file tracking module.

---

## References
- [Google Doc Link: GAD-4 FileTracking API](https://docs.google.com/document/d/1kp8H_cpCyEAWIONtiNtKNlnxLBp5mJ1nHHxrCkYQoFU/edit)
