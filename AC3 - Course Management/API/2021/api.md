# Module Name - AC3 (COURSE MANAGEMENT)  
**Student Mentor** - Saurav Raj (21BCS188)

## API Documentation of AC3 - Course Management Module

### APIs: /ocms/  
1. **/{user} - Implemented (name - viewcourses)**  
    a. Parameters required - user  
    b. Description - Shows all the courses under the user  
<br>

2. **/{course_code}/{user, course code} - Partially Working (name - course)**  
    a. Parameters required - user, course code  
    b. Description - Home page for each course for Student/Faculty  
<br>

3. **/{course_code}/get_exam_data{exam name, course code} - Partially Working**  
    a. Parameters required - exam_name, course code  
    b. Description - Shows the marks related to a specific course  
<br>

4. **/{course_code}/forum{user, course code} - Partially Working**  
    a. Parameters required - user, course code  
    b. Description - Shows the forum related to the selected course to the user.  
<br>

5. **/{course_code}/ajax_reply{user, course code} - Partially Working**  
    a. Parameters required - user, course code  
    b. Description - Adds comment to the post on the selected course’s forum.  
<br>

6. **/{course_code}/ajax_new{user, course code} - Partially Working**  
    a. Parameters required - user, course code  
    b. Description - Adds a new post on the selected course’s forum.  
<br>

7. **/{course_code}/ajax_remove{user} - Partially Working**  
    a. Parameters required - user  
    b. Description - Deletes the selected post created by the user on the forum.  
<br>

8. **/{course_code}/upload_assignment{user, course code} - Partially Working**  
    a. Parameters required - user, course code  
    b. Description - Submits the assignment assigned to the Students on the selected course portal.  
<br>

9. **/{course code}/add_document{user, course code} - Partially Working**  
    a. Parameters required - user, course code  
    b. Description - Uploads course content provided by the Instructor to the course portal.  
<br>

10. **/{course_code}/add_assignment{user, course code} - Partially Working**  
    a. Parameters required - user, course code  
    b. Description - Uploads the assignment created by Faculty on the course portal.  
<br>

11. **/{course_code}/delete/{user, course code} - Partially Working**  
    a. Parameters required - user  
    b. Description - Deletes the selected course content/assignment/grade sheet uploaded by the Faculty on the course portal.  
<br>

12. **/{course_code}/submit_attendance{user, course code} - Partially Working**  
    a. Parameters required - user, course code  
    b. Description - Uploads the attendance related to the particular course on the course portal.  
<br>

13. **/{course_code}/view_attendance{user, course code} - Yet to be implemented**  
    a. Parameters required - user, course code  
    b. Description - Shows attendance of students related to the course selected.  
<br>

14. **/add_time_table - Yet to be implemented**  
    a. Parameters required - Yet to be implemented  
    b. Description - Uploads weekly time table to Student/Faculty dashboard, which is created by Acad Admin.  
<br>

15. **/add_academic_calendar - Yet to be implemented**  
    a. Parameters required - Yet to be implemented  
    b. Description - Uploads Academic calendar to Student/Faculty dashboard (created by Acad Admin user)  
<br>

16. **/{course_code}/evaluate_assignment - Yet to be implemented**  
    a. Parameters required - Yet to be implemented  
    b. Description - Uploads the marks and evaluations done by the Instructor to the course portal.  
<br>

17. **/{course_code}/create_grading_scheme - Yet to be implemented**  
    a. Parameters required - Yet to be implemented  
    b. Description - Uploads the grading scheme created by the instructor to the course portal.  
<br>

18. **/{course_code}/view_submissions - Yet to be implemented**  
    a. Parameters required - Yet to be implemented  
    b. Description - Shows the assignment submissions by the students on the portal of the selected course.  
<br>

19. **/{course_code}/view_assignment - Yet to be implemented**  
    a. Parameters required - Yet to be implemented  
    b. Description - Shows the assignment submitted by a student in the selected course to the instructor.  
<br>

20. **/{course_code}/view_modules - Yet to be implemented**  
    a. Parameters required - Yet to be implemented  
    b. Description - Shows all the modules created by the Instructor to the student on the course portal.  
<br>

21. **/{course_code}/download_document - Yet to be implemented**  
    a. Parameters required - Yet to be implemented  
    b. Description - Downloads the selected course content on the local machine of the student.  
<br>

## Overview of Module:
The module is designed to provide a platform for instructors and students to work together more efficiently. The primary objective of the module is to streamline and enhance course management, benefiting both students and faculty.  
Instructors can upload course-related documents, assignments, quizzes, and announcements, while students can view their performance, course content, submit assignments, and ask related queries. The application also allows instructors to evaluate assignments and projects allotted to students and recommends optimal grades for each student.  
The module includes features such as the ability to showcase courses with details such as name, code, instructor, and schedule. The system also addresses the optimal display of courses. A dedicated section for each course facilitates easy access to course materials and resources in various file formats.  
**Main actors include** - Student, Instructor, and Acad admin.

## APIs:

### Yet to be implemented or Partially Working  

- #### UC#1 manage_evaluations  
  - **Index of APIs used** - 1, 2, 3, 16, 17, 18  
  - The view_course API is built but not integrated properly with the application.  
  - The course API is partially working and throws errors at some important test cases.  
  - The get_exam_data API is not properly implemented.  
  - The evaluate_assignment, create_grading_scheme are yet to be implemented in the app.  
  - **Databases** - Curriculum, Curriculum_Instructor, globals_extrainfo, Student, Assignment, Student_Assignment, Grades, online_cms_assignment, online_cms_studentassignment.  

- #### UC#2 manage_course  
  - **Index of APIs used** - 1, 2, 4, 5, 6, 7, 9, 10, 11, 12  
  - The view_course API is built but not integrated properly with the application.  
  - The course API is partially working and throwing errors at some important test cases.  
  - The forum, ajax_reply, ajax_new, ajax_remove, add_document, add_assignment, delete and submit_attendance APIs are not properly implemented.  
  - **Databases** - Curriculum, Curriculum_Instructor, Course, Student_attendance, online_cms_coursedocuments, online_cms_coursevideo, online_cms_assignment, online_cms_forum.  

- #### UC#3 view_course_content  
  - **Index of APIs used** - 1, 2, 4, 5, 6, 19, 20  
  - The view_course API is built but not integrated properly with the application.  
  - The course API is partially working and throwing errors at some important test cases.  
  - The forum, ajax_reply, and ajax_new APIs are not properly implemented.  
  - The view_assignment and view_modules APIs are not created and hence would be implemented in the app.  
  - **Database** - Curriculum, Course, online_cms_assignment, online_cms_coursedocuments, online_cms_coursevideo, online_cms_studentassignment, online_cms_forum.  

- #### UC#4 submit_assignment  
  - **Index of APIs used** - 1, 2, 8  
  - The view_course API is built but not integrated properly with the application.  
  - The course API is partially working and throwing errors at some important test cases.  
  - The upload_assignment API is not properly implemented.  
  - **Database** - Curriculum, Course, online_cms_studentassignment.  

- #### UC#5 view_progress  
  - **Index of APIs used** - 1, 2, 3, 13.  
  - The view_course API is built but not integrated properly with the application.  
  - The course API is partially working and throwing errors at some important test cases.  
  - The get_exam_data API is not properly implemented.  
  - The view_attendance API is not created and hence would be implemented in the app.  
  - **Database** - Curriculum, Course, Student_attendance, Grades, online_cms_marks.  

- #### UC#6 download_content  
  - **Index of APIs used** - 1, 2, 21  
  - The view_course API is built but not integrated properly with the application.  
  - The course API is partially working and throwing errors at some important test cases.  
  - The download_document API is not created and hence would be implemented in the app.  
  - **Database** - Curriculum, Course, online_cms_coursedocuments.  

- #### UC#7 add_time_table  
  - **Index of APIs used** - 14  
  - A new API has to be implemented for the Acad admin to add the Time table for the current semester.  
  - **Database** - Timetable.  

- #### UC#8 add_academic_calendar  
  - **Index of APIs used** - 15  
  - A new API has to be implemented for the Acad admin to add the Academic calendar for the current semester.  
  - **Database** - Academic calendar.  
  
---

# Current Problems with the Module or its Use Cases

##### [UC#1 Manage Evaluations]
- **Problem**: The APIs are not properly developed, and the frontend is partially developed.

##### [UC#2 Manage Courses]
- **Problem**: The APIs are not properly developed, and the frontend is partially developed.

##### [UC#3 View Course Content]
- **Problem**: The APIs are not properly developed, and the frontend is partially developed. Two APIs need to be freshly developed.

##### [UC#4 Submit Assignment]
- **Problem**: The APIs are not properly developed, and the frontend is not developed at all.

##### [UC#5 View Progress]
- **Problem**: The APIs are not properly developed, and the frontend is not developed. One API needs to be developed from scratch.

##### [UC#6 Download Content]
- **Problem**: The APIs are not properly developed, and the frontend is not developed. One API needs to be developed from scratch.
  

