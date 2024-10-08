**Module Name**	- AC1 (PROGRAMME AND CURRICULUM)

**Student Mentor** - Shubh Mehta (21BCS197)

# **API Documentation of AC1-Programme and Curriculum Overview of the module:-**
The purpose of the project entitled as PROGRAMME AND CURRICULUM MANAGEMENT is to provide addition of new programmes and effective management of various curriculum for different programmes offered in the institute. Each programme could update its curriculum for each batch. The scope of the application covers the entire Programmes and its curriculums offered by the Institute where the user can view their desired curriculum, programme, discipline and batch.

- Curriculums Management.
- Forwarding of course proposal forms.
- Addition and updation of courses




# **All the API’s used in the Module are:**
**Already Implemented:**


1. admin\_programmes (Get Request)- Already implemented(Status:200 OK)
   1. Parameters required - programmes and disciplines.
   1. Description -The user can view all the programmes.
1. admin\_edit \_programme (Get Request) - Already implemented(Status:200 OK)
   1. Parameters required - programme name,category,begin year.
   1. Description - The admin can edit or update a programme
1. admin\_edit \_programme (post Request)- Already implemented(Status:302 FOUND)
   1. Parameters required - programme name,category,begin year.
   1. Description -The admin can edit or update a programme
1. admin\_add \_programme (Get Request) - Already implemented(Status:200 OK)
   1. Parameters required - programme category and begin year.
   1. Description - The admin can add a programme the institute wants to offer.
1. admin\_add \_programme (post Request)- Already implemented(Status:302 FOUND)
   1. Parameters required - programme name,category and begin year.

1. Description - The admin can add a programme the institute wants to offer.

1. admin\_working\_curriculum (Get Request) - Already implemented(Status:200 OK)
   1. Parameters required - name and version of curriculum,number of semesters,batches.
   1. Description - The admin can view the working curriculums of the institute.
1. admin\_curriculum\_semesters (Get Request) - Already implemented(Status:200 OK)
   1. Parameters required - semester structure
   1. Description - The admin can view courses for the semester in a curriculum.
1. admin\_instigate\_semester (Get Request) - Already implemented(Status:200 OK)
   1. Parameters required - curriculum name and programme name,discipline name.
   1. Description - The admin can instigate a semester.
1. admin\_instigate\_semester (post Request) - Already implemented(Status:302 FOUND)
   1. Parameters required - curriculum name and programme name,discipline name,start and end semester date,semester information.
   1. Description - The admin can instigate a semester.
1. admin\_semester(get) - Already implemented(Status:200 OK)
   1. Parameters required - semester info and course slots for that semester.
   1. Description - The admin can view semester information.
1. admin\_add\_courseslot(get) - Already implemented(Status:200 OK)
   1. Parameters required - semester
   1. Description - The admin can add a new course slot.
1. admin\_add\_courseslot(post) - Already implemented(Status:302 FOUND)
   1. Parameters required - all info about the course.
   1. Description -The admin can add a new courseslot.
1. admin\_edit\_curriculum(get) - Already implemented(Status:200 OK)
   1. Parameters required - curriculum name,version,programme,number of semesters,minimum number of semesters.
   1. Description - The admin can edit or update a curriculum.
1. admin\_edit\_curriculum(post) - Already implemented(Status:302 FOUND)
   1. Parameters required - curriculum name,version,programme,number of semesters,minimum number of semesters.
   1. Description - The admin can edit or update a curriculum.
1. admin\_batches(get) - Already implemented(Status:200 OK)
   1. Parameters required - programme name,discipline,begin year,curriculum
   1. Description - The admin can view all the batches.
1. admin\_edit\_courseslot(get) - Already implemented(Status:200 OK)

1. Parameters required - semester,slot name,type,courses,information.
1. Description - The admin can edit or update the course slot.
1. admin\_edit\_courseslot(post) - Already implemented
   1. Parameters required - all info about courseslot
   1. Description - The admin can edit or update the course slot.
1. admin\_courses(get)- Already implemented(Status:200 OK)
   1. Parameters required -course code ,name and credits.
   1. Description -The user can view various courses the institute can offer.
1. admin\_update\_course(get) - Already implemented(Status:200 OK)
   1. Parameters required - meta data of a course
   1. Description -The admin can update a course.
1. admin\_update\_course(post) - Already implemented(Status:302 FOUND)
   1. Parameters required - meta data of a course.
   1. Description -The admin can update a course.
1. admin\_add\_course(get) - Already implemented(Status:200 OK)
   1. Parameters required - disciplines,percentage of marks.
   1. Description - The admin can add a new course after getting a approved form.
1. admin\_add\_course(post) - Already implemented(Status:302 FOUND)
   1. Parameters required - meta data of course.
   1. Description - The admin can add a new course after getting a approved form.
1. admin\_disciplines(get) - Already implemented(Status:200 OK)
   1. Parameters required - discipline name and programmes.
   1. Description - can view all disciplines offered by institute.
1. admin\_curriculums(get)- Already implemented(Status:200 OK)
   1. Parameters required - programme info,working curriculums under the programme,obsolete curriculums.
   1. Description -The admin can view the programme and curriculum details.
1. admin\_add\_curriculum(get) - Already implemented(Status:200 OK)
   1. Parameters required - programme details.
   1. Description -The admin can add a curriculum the institute wants to offer.
1. admin\_add\_curriculum(post) - Already implemented(Status:302 FOUND)
   1. Parameters required - curriculum name, respective programme and curriculum version,number of semesters, minimum number of credits,working curriculum or not.
   1. Description - The admin can add a curriculum the institute wants to offer.
1. admin\_edit\_discipline(get) - Already implemented(Status:200 OK)
   1. Parameters required - discipline name ,acronym,programmes.
   1. Description - The admin can edit or update a discipline.
1. admin\_edit\_discipline(post) - Already implemented(Status:302 FOUND)
   1. Parameters required - discipline name ,acronym,programmes.

1. Description - The admin can edit or update a discipline.
1. admin\_add\_discipline (Get Request )- Already implemented(Status:200 OK)
   1. Parameters required - programmes.
   1. Description - The admin can add a new discipline.
1. admin\_add\_discipline (post Request )- Already implemented(Status:302 FOUND)
   1. Parameters required - discipline name,acronym and programme.
   1. Description -The admin can add a new discipline.
1. admin\_add\_batch (Get Request ) - Already implemented(Status:200 OK)
   1. Parameters required - programme,discipline,curriculum,running batch or not.
   1. Description -The admin can add a new batch and can assign a curriculum to it.
1. admin\_add\_batch (Post Request ) - Already implemented(Status:302 FOUND)
   1. Parameters required - programme,discipline,curriculum,running batch or not and batch year
   1. Description - The admin can add a new batch and can assign a curriculum to it.
1. admin\_course (Get Request)- Already implemented(Status:200 OK)
   1. Parameters required - meta data of a course
   1. Description - The user can all the meta data of a course.
1. programmes (Get Request)- Already implemented(Status:200 OK)
   1. Parameters required -programmes and disciplines.
   1. Description - The user can view the various programmes the institute can offer.
1. curriculums (Get Request)- Already implemented(Status:200 OK)
   1. Parameters required - programme category,name and begin year, working and obsolete curriculums.
   1. Description -The User can see the programme information and working curriculums under the programme and obsolete curriculums.
1. curriculum\_semesters (Get Request)- Already implemented(Status:200 OK)
   1. Parameters required - all courses in a semester
   1. Description -The user can view the metadata of a curriculum.
1. semester (Get Request)- Already implemented(Status:200 OK)
   1. Parameters required -semester start and end date,semester info.
   1. Description The user can view the semester info of a particular curriculum.
1. courseslot (Get Request)- Already implemented(Status:200 OK)
   1. Parameters required - course slot
   1. Description - The user can see the course slot in which semester it belongs.
1. course (Get Request)- Already implemented(Status:200 OK)
   1. Parameters required -all info about course
   1. Description - The user can view the metadata of a course.
1. working\_curriculums(Get Request)- Already implemented(Status:200 OK)
   1. Parameters required - curriculum name,version,batches,number of semesters.

1. Description -The user can view the working curriculums in the institute.
1. courses(Get Request)- Already implemented(Status:200 OK)
   1. Parameters required - course code,name and credits.
   1. Description - The user can view all the courses the institute can offer.
1. disciplines(Get Request)- Already implemented(Status:200 OK)
   1. Parameters required -discipline name and programmes.
   1. Description -The user can view all the various disciplines the institute can offer.
1. batches(Get Request)- Already implemented(Status:200 OK)
   1. Parameters required - batch name discipline,year and curriculum.
   1. Description - The user can view various batches in the institute.


**Yet to be Implemented:**

1. add\_course\_proposal \_form - Yet to be implemented
   1. Parameters required - info about course.
   1. Description - The user can fill a form for a new course to be added.
1. edit\_course\_proposal \_form- Yet to be implemented
   1. Parameters required - info about course.
   1. Description -The user can fill a form for updating details of a course.
1. forward\_course\_proposal \_form- Yet to be implemented
   1. Parameters required - info about course,forwarded/not.
   1. Description - The user can forward the form to the next authority.
1. hod\_reject\_course\_proposal \_form- Yet to be implemented
   1. Parameters required - info about course,rejected/not.
   1. Description - The user can forward or reject the form.
1. approve\_course\_proposal \_form - Yet to be implemented
   1. Parameters required - info about course,approved/not.
   1. Description - The user can approve the course proposal form.
1. dean\_academics\_reject\_course\_proposal \_form - Yet to be implemented
   1. Parameters required - info about course,rejected/not.
   1. Description - The user can reject the course proposal form.


# **APIs:-**


- **Already Implemented (**This means that API is already implemented and working as expected.**)**
- [AC-1 Programme and Curriculum Use Case Diagram](https://docs.google.com/document/d/1LdWS-N_ZtQiEOtNaObfywRRRDXHeGbYzy2C0a4oN4K0/edit?usp=sharing)

- *browse\_programme\_catalog - UC#1*
  - Actor : generic\_user
  - Index of api’s used - 35,43
  - Description - User can view all programmes the institute can offer.
  - Database - programme\_curriculum\_programme,programme\_curriculum\_discipline.
- *browse\_curriculum\_catalog - UC#2*
  - Actor : generic\_user
  - Index of api’s used - 36,37,38,39,40,41,42,44
  - Description - Users can view all curriculums the institute can offer.
  - Database - programme\_curriculum\_curriculum,programme\_curriculum\_semester,pr ogramme\_curriculum\_courseslot,programme\_curriculum\_batch,progra mme\_curriculum\_course.
- *add\_programme- UC#3*
  - Actor : Acad\_admin
  - Index of apis used - 4,5
  - Description - User can add a new programme.
  - Database - programme\_curriculum\_programme

- *update\_programme - UC#4*
  - Actor : Acad\_admin
  - Index of api’s used - 1,2,3
  - Description -User can update a programme.
  - Database - programme\_curriculum\_programme
- *add\_curriculum - UC#5*
  - Actor : Acad\_admin
  - Index of api’s used - 6,7,8,9,10,26,27
  - Description - User can add a new curriculum.
  - Database - programme\_curriculum\_curriculum
- *Update\_curriculum - UC#6*

- Actor : Acad\_admin
- Index of api’s used - 6,7,8,9,10,13,14,25
- Description - User can update a curriculum.
- Database - programme\_curriculum\_curriculum
- *add\_new\_course - UC#7*
  - Actor : Acad\_admin
  - Index of api’s used - 12,22,23
  - Description - User can add a new Course.
  - Database - programme\_curriculum\_course
- *update\_course - UC#8*
  - Actor : Acad\_admin
  - Index of api’s used - 11,12,17,18,19,20,21,34
  - Description - User can update a Course.
  - Database - programme\_curriculum\_course

- **Yet to be implemented or Partially Working** (API is not implemented so yet to be implemented.)
- [AC-1 Programme and Curriculum Use Case Diagram](https://docs.google.com/document/d/1LdWS-N_ZtQiEOtNaObfywRRRDXHeGbYzy2C0a4oN4K0/edit?usp=sharing)
  - *add\_new\_course\_proposal\_form - UC#9*
    - Actor : Faculty
    - Index of api’s used - 44
    - Description - User can apply for a course by filling the data of the course which he wants to add.
    - Database - No table created,suggested table name:”course\_proposal\_form”

- *Update\_course\_proposal\_form - UC#10*
  - Actor : Faculty
  - Index of api’s used - 45
  - Description - Faculty can propose any changes in the existing course slot by filling the form and submitting.

- Database - programme\_curriculum\_course,programme\_curriculum\_courseslot,one more new table needs to be created.(suggested table name:”course\_proposal\_form”)
- *Forward/reject\_course\_proposal\_form*- UC#11
  - Actor : Head of Discipline
  - Index of api’s used - 46,47
  - Description - The actor should be able to view proposed forms in a notifications section exclusively under him/her and should be able to forward to the dean academics or should be able to reject the form.Subsequently the necessary notifications should be displayed to the respective faculty that proposed.The expected difficulty of implementing the work is easy.
  - Database - no table created.

- *Approve/reject\_course\_proposal\_form*- UC#12
  - Actor : Dean Academics
  - Index of api’s used - 48,49
  - Description - The actor should be able to view proposed forms in a notifications section exclusively under him/her and should be able to approve the add / modify course form or should be able to reject the form. The approved course to add/update a course details should be forwarded to the acad admin and the acad\_admin adds it.The expected difficulty of implementing the work is easy.
  - Database - no table created

# **Current problems you are facing with the module or in its use cases —**

- No endpoint found ,only done by rendering.(data is only being rendered) Google Doc Link : [Modules Testing Assignment.docx](https://docs.google.com/document/d/1lKKkY0wqEsLCYoSoqIOAkmx3sg669nMAJhz0gCNLJoo/edit?usp=sharing3FD60y9aitltMzB1RMeObb-KgUvGyq/edit%3Fusp%3Dsharing&ouid=104512684967527548096&rtpof=true&sd=true)

![](Aspose.Words.28cf15b0-5b62-4e10-a3e5-5385dd215d52.001.png)
