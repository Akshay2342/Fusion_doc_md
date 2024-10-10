# Module Name - AC1 (PROGRAMME AND CURRICULUM)

**Student Mentor** - Shubh Mehta (21BCS197)

## API Documentation of AC1-Programme and Curriculum 

### Overview of the module:
The purpose of the project entitled as PROGRAMME AND CURRICULUM MANAGEMENT is to provide addition of new programmes and effective management of various curriculum for different programmes offered in the institute. Each programme could update its curriculum for each batch. The scope of the application covers the entire Programmes and its curriculums offered by the Institute where the user can view their desired curriculum, programme, discipline and batch.
1. **Curriculums Management.**
2. **Forwarding of course proposal forms.**
3. **Addition and updation of courses**

### All the API’s used in the Module are:

#### Already Implemented:

1. **admin_programmes (Get Request)** - Already implemented(Status:200 OK)
   - **Parameters required** - programmes and disciplines.
   - **Description** - The user can view all the programmes.

2. **admin_edit _programme (Get Request)** - Already implemented(Status:200 OK)
   - **Parameters required** - programme name,category,begin year.
   - **Description** - The admin can edit or update a programme.

3. **admin_edit _programme (post Request)** - Already implemented(Status:302 FOUND)
   - **Parameters required** - programme name,category,begin year.
   - **Description** - The admin can edit or update a programme.

4. **admin_add _programme (Get Request)** - Already implemented(Status:200 OK)
   - **Parameters required** - programme category and begin year.
   - **Description** - The admin can add a programme the institute wants to offer.

5. **admin_add _programme (post Request)** - Already implemented(Status:302 FOUND)
   - **Parameters required** - programme name,category and begin year.
   - **Description** - The admin can add a programme the institute wants to offer.

6. **admin_working_curriculum (Get Request)** - Already implemented(Status:200 OK)
   - **Parameters required** - name and version of curriculum,number of semesters,batches.
   - **Description** - The admin can view the working curriculums of the institute.

7. **admin_curriculum_semesters (Get Request)** - Already implemented(Status:200 OK)
   - **Parameters required** - semester structure.
   - **Description** - The admin can view courses for the semester in a curriculum.

8. **admin_instigate_semester (Get Request)** - Already implemented(Status:200 OK)
   - **Parameters required** - curriculum name and programme name,discipline name.
   - **Description** - The admin can instigate a semester.

9. **admin_instigate_semester (post Request)** - Already implemented(Status:302 FOUND)
   - **Parameters required** - curriculum name and programme name,discipline name,start and end semester date,semester information.
   - **Description** - The admin can instigate a semester.

10. **admin_semester(get)** - Already implemented(Status:200 OK)
    - **Parameters required** - semester info and course slots for that semester.
    - **Description** - The admin can view semester information.

11. **admin_add_courseslot(get)** - Already implemented(Status:200 OK)
    - **Parameters required** - semester.
    - **Description** - The admin can add a new course slot.

12. **admin_add_courseslot(post)** - Already implemented(Status:302 FOUND)
    - **Parameters required** - all info about the course.
    - **Description** -The admin can add a new courseslot.

13. **admin_edit_curriculum(get)** - Already implemented(Status:200 OK)
    - **Parameters required** - curriculum name,version,programme,number of semesters,minimum number of semesters.
    - **Description** - The admin can edit or update a curriculum.

14. **admin_edit_curriculum(post)** - Already implemented(Status:302 FOUND)
    - **Parameters required** - curriculum name,version,programme,number of semesters,minimum number of semesters.
    - **Description** - The admin can edit or update a curriculum.

15. **admin_batches(get)** - Already implemented(Status:200 OK)
    - **Parameters required** - programme name,discipline,begin year,curriculum.
    - **Description** - The admin can view all the batches.

16. **admin_edit_courseslot(get)** - Already implemented(Status:200 OK)
    - **Parameters required** - semester,slot name,type,courses,information.
    - **Description** - The admin can edit or update the course slot.

17. **admin_edit_courseslot(post)** - Already implemented
    - **Parameters required** - all info about courseslot.
    - **Description** - The admin can edit or update the course slot.

18. **admin_courses(get)** - Already implemented(Status:200 OK)
    - **Parameters required** - course code ,name and credits.
    - **Description** -The user can view various courses the institute can offer.

19. **admin_update_course(get)** - Already implemented(Status:200 OK)
    - **Parameters required** - meta data of a course.
    - **Description** -The admin can update a course.

20. **admin_update_course(post)** - Already implemented(Status:302 FOUND)
    - **Parameters required** - meta data of a course.
    - **Description** -The admin can update a course.

21. **admin_add_course(get)** - Already implemented(Status:200 OK)
    - **Parameters required** - disciplines,percentage of marks.
    - **Description** - The admin can add a new course after getting a approved form.

22. **admin_add_course(post)** - Already implemented(Status:302 FOUND)
    - **Parameters required** - meta data of course.
    - **Description** - The admin can add a new course after getting a approved form.

23. **admin_disciplines(get)** - Already implemented(Status:200 OK)
    - **Parameters required** - discipline name and programmes.
    - **Description** - can view all disciplines offered by institute.

24. **admin_curriculums(get)** - Already implemented(Status:200 OK)
    - **Parameters required** - programme info,working curriculums under the programme,obsolete curriculums.
    - **Description** -The admin can view the programme and curriculum details.

25. **admin_add_curriculum(get)** - Already implemented(Status:200 OK)
    - **Parameters required** - programme details.
    - **Description** -The admin can add a curriculum the institute wants to offer.

26. **admin_add_curriculum(post)** - Already implemented(Status:302 FOUND)
    - **Parameters required** - curriculum name, respective programme and curriculum version,number of semesters, minimum number of credits,working curriculum or not.
    - **Description** - The admin can add a curriculum the institute wants to offer.

27. **admin_edit_discipline(get)** - Already implemented(Status:200 OK)
    - **Parameters required** - discipline name ,acronym,programmes.
    - **Description** - The admin can edit or update a discipline.

28. **admin_edit_discipline(post)** - Already implemented(Status:302 FOUND)
    - **Parameters required** - discipline name ,acronym,programmes.
    - **Description** - The admin can edit or update a discipline.

29. **admin_add_discipline (Get Request)** - Already implemented(Status:200 OK)
    - **Parameters required** - programmes.
    - **Description** - The admin can add a new discipline.

30. **admin_add_discipline (post Request)** - Already implemented(Status:302 FOUND)
    - **Parameters required** - discipline name,acronym and programme.
    - **Description** -The admin can add a new discipline.

31. **admin_add_batch (Get Request)** - Already implemented(Status:200 OK)
    - **Parameters required** - programme,discipline,curriculum,running batch or not.
    - **Description** -The admin can add a new batch and can assign a curriculum to it.

32. **admin_add_batch (Post Request)** - Already implemented(Status:302 FOUND)
    - **Parameters required** - programme,discipline,curriculum,running batch or not and batch year.
    - **Description** - The admin can add a new batch and can assign a curriculum to it.

33. **admin_course (Get Request)** - Already implemented(Status:200 OK)
    - **Parameters required** - meta data of a course.
    - **Description** - The user can all the meta data of a course.

34. **programmes (Get Request)** - Already implemented(Status:200 OK)
    - **Parameters required** - programmes and disciplines.
    - **Description** - The user can view the various programmes the institute can offer.

35. **curriculums (Get Request)** - Already implemented(Status:200 OK)
    - **Parameters required** - programme category,name and begin year, working and obsolete curriculums.
    - **Description** -The User can see the programme information and working curriculums under the programme and obsolete curriculums.

36. **curriculum_semesters (Get Request)** - Already implemented(Status:200 OK)
    - **Parameters required** - all courses in a semester.
    - **Description** -The user can view the metadata of a curriculum.

37. **semester (Get Request)** - Already implemented(Status:200 OK)
    - **Parameters required** - semester start and end date,semester info.
    - **Description** - The user can view the semester info of a particular curriculum.

38. **courseslot (Get Request)** - Already implemented(Status:200 OK)
    - **Parameters required** - course slot.
    - **Description** - The user can view all the courses in a slot.

39. **course (Get Request)** - Already implemented(Status:200 OK)
    - **Parameters required** - course code and credits.
    - **Description** -The user can view various courses the institute can offer.

40. **discipline (Get Request)** - Already implemented(Status:200 OK)
    - **Parameters required** - discipline and its acronym.
    - **Description** -The user can view all the disciplines offered by the institute.

41. **batches (Get Request)** - Already implemented(Status:200 OK)
    - **Parameters required** - batch year.
    - **Description** -The user can view all batches offered by the institute.

## Yet to be Implemented:

- **add_course_proposal_form** - Yet to be implemented
  - **Parameters required** - info about course.
  - **Description** - The user can fill a form for a new course to be added.

- **edit_course_proposal_form** - Yet to be implemented
  - **Parameters required** - info about course.
  - **Description** - The user can fill a form for updating details of a course.

- **forward_course_proposal_form** - Yet to be implemented
  - **Parameters required** - info about course, forwarded/not.
  - **Description** - The user can forward the form to the next authority.

- **hod_reject_course_proposal_form** - Yet to be implemented
  - **Parameters required** - info about course, rejected/not.
  - **Description** - The user can forward or reject the form.

- **approve_course_proposal_form** - Yet to be implemented
  - **Parameters required** - info about course, approved/not.
  - **Description** - The user can approve the course proposal form.

- **dean_academics_reject_course_proposal_form** - Yet to be implemented
  - **Parameters required** - info about course, rejected/not.
  - **Description** - The user can reject the course proposal form.

## APIs:

### Already Implemented (This means that API is already implemented and working as expected.)

- **AC-1 Programme and Curriculum Use Case Diagram**
  - **browse_programme_catalog** - UC#1
    - **Actor**: generic_user
    - **Index of api’s used** - 35,43
    - **Description** - User can view all programmes the institute can offer.
    - **Database** - programme_curriculum_programme, programme_curriculum_discipline.

  - **browse_curriculum_catalog** - UC#2
    - **Actor**: generic_user
    - **Index of api’s used** - 36,37,38,39,40,41,42,44
    - **Description** - Users can view all curriculums the institute can offer.
    - **Database** - programme_curriculum_curriculum, programme_curriculum_semester, programme_curriculum_courseslot, programme_curriculum_batch, programme_curriculum_course.

  - **add_programme** - UC#3
    - **Actor**: Acad_admin
    - **Index of apis used** - 4,5
    - **Description** - User can add a new programme.
    - **Database** - programme_curriculum_programme.

  - **update_programme** - UC#4
    - **Actor**: Acad_admin
    - **Index of api’s used** - 1,2,3
    - **Description** - User can update a programme.
    - **Database** - programme_curriculum_programme.

  - **add_curriculum** - UC#5
    - **Actor**: Acad_admin
    - **Index of api’s used** - 6,7,8,9,10,26,27
    - **Description** - User can add a new curriculum.
    - **Database** - programme_curriculum_curriculum.

  - **Update_curriculum** - UC#6
    - **Actor**: Acad_admin
    - **Index of api’s used** - 6,7,8,9,10,13,14,25
    - **Description** - User can update a curriculum.
    - **Database** - programme_curriculum_curriculum.

  - **add_new_course** - UC#7
    - **Actor**: Acad_admin
    - **Index of api’s used** - 12,22,23
    - **Description** - User can add a new Course.
    - **Database** - programme_curriculum_course.

  - **update_course** - UC#8
    - **Actor**: Acad_admin
    - **Index of api’s used** - 11,12,17,18,19,20,21,34
    - **Description** - User can update a Course.
    - **Database** - programme_curriculum_course.

### Yet to be implemented or Partially Working (API is not implemented so yet to be implemented.)

- **AC-1 Programme and Curriculum Use Case Diagram**
  - **add_new_course_proposal_form** - UC#9
    - **Actor**: Faculty
    - **Index of api’s used** - 44
    - **Description** - User can apply for a course by filling the data of the course which he wants to add.
    - **Database** - No table created, suggested table name: "course_proposal_form".

  - **Update_course_proposal_form** - UC#10
    - **Actor**: Faculty
    - **Index of api’s used** - 45
    - **Description** - Faculty can propose any changes in the existing course slot by filling the form and submitting.
    - **Database** - programme_curriculum_course, programme_curriculum_courseslot, one more new table needs to be created (suggested table name: "course_proposal_form").

  - **Forward/reject_course_proposal_form** - UC#11
    - **Actor**: Head of Discipline
    - **Index of api’s used** - 46,47
    - **Description** - The actor should be able to view proposed forms in a notifications section exclusively under him/her and should be able to forward to the dean academics or should be able to reject the form. Subsequently, the necessary notifications should be displayed to the respective faculty that proposed. The expected difficulty of implementing the work is easy.
    - **Database** - no table created.

  - **Approve/reject_course_proposal_form** - UC#12
    - **Actor**: Dean Academics
    - **Index of api’s used** - 48,49
    - **Description** - The actor should be able to view proposed forms in a notifications section exclusively under him/her and should be able to approve the add/modify course form or should be able to reject the form. The approved course to add/update a course details should be forwarded to the acad admin and the acad_admin adds it. The expected difficulty of implementing the work is easy.
    - **Database** - no table created.

## Current problems you are facing with the module or in its use cases —

- No endpoint found, only done by rendering (data is only being rendered).
