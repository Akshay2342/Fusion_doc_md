##### Module Name - AC2 (Course Registration)				
##### Student Mentor - Pranav Bharadwaj (21BCS160)

# API - DOCUMENTATION OF AC-2 COURSE REGISTRATION

## Overview of the module:
Academic Course Registration (AC-2) is a software designed to manage different activities related to the Course Registrations of PDPM IIITDM Jabalpur. The module seeks to provide automated features and a smooth interface to the Academic staff, students and faculties to handle different Course registration and corresponding related activities such as:
- Admission
- Courses Registration
- add-drop
- replace
- apply for backlog
- manage schedule
- course-list generation
- roll list generation
- and more.

### Please mention all the API used in the module below 
1. **POST academic-procedures/auto_pre_registration/** - Implemented  
   **Description** - used by student to do the pre registration by new method (without priority system) by directly assigning the courses is available, for the next semester 
<br>

2. **POST academic-procedures/final_registration/** - Implemented  
   **Description** - used by student to do the final registration for the next semester by providing fee payment details
<br>

3. **POST academic-procedures/api/stu/view_offered_courses** - Implemented  
   **Description** - used by student to see the courses offered in the upcoming semester
<br>

4. **POST academic-procedures/addCourse/** - Implemented  
   **Description** - used by student to add the courses that are not registered till now
<br>

5. **POST academic-procedures/drop_course/** - Implemented  
   **Description** - used by student to drop the registered courses
<br>

6. **POST academic-procedures/replace_one_course/** - Implemented  
   **Description** - used by student to replace the registered optional course in a slot with another optional course in same slot
<br>

7. **POST academic-procedures/replaceCourse/** - Implemented  
   **Description** - used by student to replace the multiple optional courses from the currently registered optional to other choices in the same optional slot
<br>

8. **POST academic-procedures/register_backlog_course/** - Implemented  
   **Description** - student can apply for backlog in any course with this request
<br>

9. **POST academic-procedures/api/stu/pre_registration/** - Implemented  
   **Description** - used by student to do pre registration using priority based logic (not used now instead auto_pre_registration used)
<br>

10. **GET academic-procedures/api/fac** - Implemented  
    **Description** - returns details of the faculty that is currently logged in the system
<br>

11. **GET academic-procedures/api/stu** - Implemented  
    **Description** - returns all details of the student currently logged in the system such as profile details, curr sem details, courses registered, next sem courses, backlog course list and more. 
<br>

12. **POST academic-procedures/acad_person/student_list/** - Implemented  
    **Description** - returns the list of students who have done the final registration and completed the fee payment, but their verification is pending
<br>

13. **POST academic-procedures/auto_process_verification_request/** - Implemented  
    **Description** - with this api request acad admin can approve or decline the final registration of any student 
<br>

14. **POST academic-procedures/acad_person/allot_courses/** - Implemented  
    **Description** - acad person can give an excel sheet with specified columns, and the record from that sheet will be used to allot courses to student
<br>

15. **POST academic-procedures/acad_person/remove_course_from_slot/** - Implemented  
    **Description** - acad person can remove some course in a course slot by giving course code of the course and slot code
<br>

16. **POST academic-procedures/acad_person/add_course_to_slot/** - Implemented  
    **Description** - acad person can add some course in a course slot by giving course code of the course and slot code
<br>

17. **POST academic-procedures/acad_person/get_next_sem_courses/** - Implemented  
    **Description** - acad person can get the list of courses for any batch semester that will be show to students during their next sem pre registration
<br>

18. **POST academic-procedures/acad_person/replaceSwayam/** - Implemented  
    **Description** - acad person can get the all swayam courses and optional courses that will be needed for allotting swayam to any specific student
<br>

19. **POST academic-procedures/acad_person/swayam_replace/** - Implemented  
    **Description** - acad person can replace swayam courses with optional courses for any student
<br>

20. **POST academic-procedures/api/acad/configure_pre_registration/** - Implemented  
    **Description** - with this request acad person can schedule the pre registration date for any upcoming semester
<br>

21. **POST academic-procedures/api/acad/configure_final_registration/** - Implemented  
    **Description** - with this request acad person can schedule the final registration/fee payment date for upcoming semester
<br>

22. **POST /aims/generate_preregistration_report/** - Implemented  
    **Description** - with this api request acad admin can generate the pre registration report of any batch and semester in excel sheet
<br>

23. **POST /aims/generatexlsheet/** - Implemented  
    **Description** - with this api request excel sheet of the registered student in any course can be downloaded for any batch
<br>

24. **GET academic-procedures/api/fac/view_assigned_courses** - Implemented  
    **Description** - Faculty will be able to see the courses assigned to him that are currently running and active with this api request.
<br>

25. **GET academic-procedures/api/get_user_info/** - Implemented  
    **Description** - Extra api for knowing the details of the currently logged user into the system.

<br>

### APIs:-	

#### Actor: Student

###### Implemented by us:

- #### view_offered_courses: UC#8
  - **Index of api’s used** -  3, 11  
  - This use case helps students to see all the courses offered to them in the upcoming semester.  
  - Databases - [programme_curriculum_course, extra_info , student , auth_user, semester]

- #### add course: UC#1
  - **Index of api’s used** -  4  
  - The use case describes how to add courses to the course list of a UG student.  
  - Databases -[programme_curriculum_course , auth_user, course_registration , ,academic_procedures_minimumcredits]

- #### Drop course: UC#2
  - **Index of api’s used** -  5  
  - The use case describes how to drop courses to the course list of a UG student.  
  -  Databases -[programme_curriculum_course , auth_user, course_registration ,academic_procedures_minimumcredits]

- #### Replace course: UC#3
  - **Index of api’s used** -  6 , 7  
  - The use case describes how to replace a course from the course list with a swayam course of the same credit.  
  - Databases -[programme_curriculum_course , course_registration ,auth_user,academic_procedures_minimumcredits]

- #### fill_backlog _form: UC#6
  - **Index of api’s used** -  8  
  - This use case helps the student to fill the form for covering their backlog courses.  
  - Databases - [course_registration , programme_curriculum_course, auth_user, semester ,batch]

- #### Pre_registration: UC#5
  - **Index of api’s used** -  1, 9  
  - The use case handles the student registration system.  
  - Databases - [InitialRegistration , auth_user , programme_curriculum_course, StudentRegistrationChecks , semester , course_registration]

- #### Final_register: UC#4
  - **Index of api’s used** -  2  
  - The use case handles the students final registration system.  
  - Databases - [FinalRegistration , auth_user , StudentRegistrationChecks, semester]

- #### view_registration: UC#7
  - **Index of api’s used** -  11  
  - This use case describes how the Students can check their profile and courses after registration.  
  - Databases - [course_registration , auth_user , StudentRegistrationChecks]


---

#### Actor: Acad Admin

##### APIs:-
###### Already Implemented 

- #### manage_schedule: UC#9
  - **Index of api’s used** -  20 , 21  
  - This use case describes how the Academic Person updates and adds the schedule of courses and time table.  
  - Databases - [programme_curriculum_course, programme_curriculum_curriculum, Timetable]

- #### view_registration: UC#10
  - **Index of api’s used** -  13 , 22  
  - This use case describes how the Academic Person checks the final registration of students for the semester.  
  - Databases - [programme_curriculum_course, auth_user, FinalRegistration]

- #### list_courses: UC#14
  - **Index of api’s used** -  14  
  - This use case allows an Academic Admin to generate a roll list for a specific course, containing student information such as names, ID numbers, and contact details.  
  - Databases - [Courses, auth_user, programme_curriculum_curriculum, FinalRegistration, academic_information_student]

- #### generate_roll_list: UC#11
  - **Index of api’s used** -  23  
  - This use case allows an Academic Admin to generate a roll list for a specific course, containing student information such as names, ID numbers, and contact details.  
  - Databases - [Courses, auth_user, programme_curriculum_curriculum, FinalRegistration, faculty, batch]

- #### configure_pre_reg: UC#12
  - **Index of api’s used** -  15 , 16 , 17  
  - This use case allows an Academic Admin to configure the settings for the pre-registration period, including dates, eligibility criteria, and student permissions.  
  - Databases - [InitialRegistration, auth_user, courses, faculty, timetable, programme_curriculum_curriculum]

- #### configure_main_reg: UC#13
  - **Index of api’s used** -  14  
  - This use case allows an Academic Admin to configure the settings for the main-registration period, including dates, eligibility criteria, and student permissions.  
  - Databases - [InitialRegistration, auth_user, courses, timetable, programme_curriculum_curriculum]

- #### allot_swayam: UC#17
  - **Index of api’s used** -  18 , 19  
  - This use case allows an Academic Admin to replace optional courses of any student with swayam courses.  
  - Databases - [programme_curriculum_course, course_registration, student, extra_info]

---


#### Actor: Faculty

##### APIs:-
###### Already Implemented 

- #### generate_roll_list: UC#16
  - **Index of api’s used** -  23  
  - This use case allows a Faculty to generate a roll list for a specific course, containing student information such as names, ID numbers, and contact details.  
  - Databases - [Courses, auth_user, faculty, batch, course_registration, programme_curriculum_course]

- #### View_assigned_course: UC#15
  - **Index of api’s used** -  24  
  - This use case allows a Faculty to view a list of courses that he is going to teach in the upcoming semester.  
  - Databases - [curriculum_instructor, programme_curriculum_course, auth_user, programme_curriculum_curriculum]
