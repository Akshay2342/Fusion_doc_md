# Software Requirements Specification for AC-1 (Web Application)

## Programme and Curriculum

**Prepared by:**

- 21BCS126 - Mamidi Ravi Chendraa
- 21BCS066 - Chilukuri Surya Manikanta Chowdary
- 21BCS082 - G Srinath Reddy
- 21BCS081 - Duggireddy Gnana Sainath Reddy
- 21BCS125 - Maloth Ritesh Pragnu Naik
- 21BCS197 - Shubh Mehta (Student Mentor)

**Faculty Mentor:**  
Dr. Vinod Kumar Jain (Head CSE)

## Table of Contents

1. [Introduction](#1-introduction)  
   1.1 [Introduction about the Fusion](#11-introduction-about-the-fusion)  
   1.2 [Purpose of the Module](#12-purpose-of-the-module)  
   1.3 [Scope of the Module](#13-scope-of-the-module)
2. [User/Actor Description (Characteristics)](#2-useractor-description-characteristics)
3. [Functional Requirements](#3-functional-requirements)  
   3.1 [Use Case Diagram](#31-use-case-diagram)  
   3.2 [Use Case Description](#32-use-case-description)  
   3.3 [Other Functional Requirements](#33-other-functional-requirements)  
   3.4 [Other Constraints](#34-other-constraints)  
   3.4.1 [User Interfaces](#341-user-interfaces)  
   3.4.2 [Software (Tech) Stack Used](#342-software-tech-stack-used)  
   3.4.3 [Business Rules](#343-business-rules)
4. [Non-Functional Requirements](#4-non-functional-requirements)
5. [Module Dependencies with Other Fusion Modules](#5-module-dependencies-with-other-fusion-modules)  
   5.1 [UI Level](#51-ui-level)  
   5.2 [DB Level Dependencies](#52-db-level-dependencies)  
   5.3 [Module Level Dependencies](#53-module-level-dependencies)

---

## 1. Introduction

### 1.1 Introduction about the Fusion

FusionIIIT stands as a testament to the seamless integration and automation of diverse functions within PDPM Indian Institute of Information Technology, Design, and Manufacturing, Jabalpur. Crafted with precision using Python 3.8 and powered by the Django Web framework, this initiative is a student-driven endeavor designed to elevate the institute's operational landscape. Encompassing everything from efficient administration management to academic prowess and miscellaneous departmental tasks, FusionIIIT is a holistic solution that harmonizes the intricacies of campus life.

### 1.2 Purpose of the Module

The objective of this module is to provide the addition of new programs and effective management of various curriculums for different programs offered at the institute. Each program can update its curriculum for the respective batch.

Additionally, this module allows users to view various programs and curriculums, batches, and disciplines offered at the institute, along with viewing the timetable and academic calendar.

### 1.3 Scope of the Module

The application covers the entire program and its curriculums offered by the Institute, where the user can view their desired curriculum, program, discipline, and batch, along with the academic calendar and timetable.

---

## 2. User/Actor Description (Characteristics)

### 2.1 Student

Represents individuals who intend to browse the program catalog and curriculum catalog.

**Role:** Can browse program catalog, browse curriculum catalog.  
**Specific Functionalities:**  
- Search specific programs, curriculums, and courses by name or discipline.
- View course information in detail.

### 2.2 ACAD ADMINISTRATOR

Responsible for managing and updating information related to academic programs and curriculums.

**Role:** Add and update programs, curriculums, and courses.  
**Specific Functionalities:**  
- Can add or modify programs, curriculums, and courses.

### 2.3 Head of Department

Represents individuals who are the heads of certain departments in the institute.

**Role:** Same as a user's roles and also forwards or rejects the course proposal form to the Dean of academics.  
**Specific Functionalities:**  
- Forwards or rejects the course proposal form to the Dean of academics.

### 2.4 Dean of Academics

Represents a high-ranking academic official overseeing major academic operations, including curriculum approval and course evaluation.

**Role:** Browse program catalog, browse curriculum catalog, approve or reject course proposal forms.  
**Specific Functionalities:**  
- Approves or rejects course proposal forms.

### 2.5 Faculty

Represents individuals who can view the current semester courses and request course additions or updates.

**Role:** Browse program catalog, browse curriculum catalog, and apply for course addition or modification.  
**Specific Functionalities:**  
- Can apply for course addition or modification through a course proposal form.

---

## 3. Functional Requirements

### 3.1 Use Case Diagram

### 3.2 Use Case Description

| UCID        | UC#1                         |
|-------------|------------------------------|
| **Usecase name** | browse_programme_catalog  |
| **Actor**        | Student, Acad Admin, HOD, Faculty, Dean |
| **Description**  | The user of the system can browse the available programme categorically. |
| **Pre Condition** | The User must be logged-in through their credentials |
| **Main Flow**    | 1. The Actor logs into the system. <br> 2. The Actor then opens the Programme and Curriculum module. <br> 3. The Actor can see the available Programmes the Institute can offer. [S1] |
| **Sub Flow**     | Extend "browse_curriculum_catalogue". |
| **Post Condition** | The necessary details of the Programmes are displayed. |

| UCID        | UC#2                         |
|-------------|------------------------------|
| **Usecase name** | browse_curriculum_catalog  |
| **Actor**        | Student, Acad Admin, HOD, Faculty, Dean |
| **Description**  | The user of the system can browse the available curriculums categorically. |
| **Pre Condition** | The User must be logged-in through their credentials |
| **Main Flow**    | 1. The Actor logs into the system. <br> 2. The Actor then opens the Programme and Curriculum module. <br> 3. The Actor then selects the desired programme. <br> 4. The Actor now can see the various curriculums for that programme by clicking the curriculum link. |
| **Post Condition** | The necessary details of the curriculum are displayed. |

| UCID        | UC#3                         |
|-------------|------------------------------|
| **Usecase name** | add_programme  |
| **Actor**        | Acad Admin |
| **Description**  | The Acad Admin can add a new programme that institute can offer |
| **Pre Condition** | The User must be logged-in through their credentials |
| **Main Flow**    | 1. The User logs into the system. <br> 2. The actor then opens the programme and curriculum module and clicks on add programme option. [S1] <br> 3. The Actor then adds the discipline, batch year, and the no. of semesters. <br> 4. The Actor then can add courses/elective courses, or labs in each Semester, and the academic load of a particular course. <br> 5. After successfully entering the details, the Actor then clicks on Submit. |
| **Sub Flow**     | S1. Extend "update_programme". |
| **Post Condition** | The programme is added successfully and is saved in the database and the programme needs to be assigned a curriculum and discipline. |

| UCID        | UC#4                         |
|-------------|------------------------------|
| **Usecase name** | update_programme  |
| **Actor**        | Acad Admin |
| **Description**  | The Acad Admin can update a programme that institute can offer |
| **Pre Condition** | The User must be logged-in through their credentials |
| **Main Flow**    | 1. The User logs into the system. <br> 2. The actor then opens the programme and curriculum module and clicks on update programme option. <br> 3. The Actor then does the desired changes <br> 4. After successfully updating the details, the Actor then clicks on Submit. |
| **Post Condition** | The programme is updated successfully and is saved in the database. |

| UCID        | UC#5                         |
|-------------|------------------------------|
| **Usecase name** | add_new_course_proposal_form  |
| **Actor**        | Faculty |
| **Description**  | The user of the system can apply for addition or modification of a course. |
| **Pre Condition** | The User must be logged-in through their credentials |
| **Main Flow**    | 1. The Actor logs into the system. <br> 2. The Actor then opens the programme and curriculum module. <br> 3. The Actor then selects the "course proposal form". <br> 4. The Actor then fills in the necessary details and then submits the form. [S1] |
| **Sub Flow**     | S1. Extend "update_course_proposal_form". |
| **Post Condition** | The form is submitted successfully and is forwarded to the respective head of department. |

| UCID        | UC#6                         |
|-------------|------------------------------|
| **Usecase name** | update_course_proposal_form  |
| **Actor**        | Faculty |
| **Description**  | The user of the system can apply for addition or modification of a course. |
| **Pre Condition** | The User must be logged-in through their credentials |
| **Main Flow**    | 1. The Actor logs into the system. <br> 2. The Actor then opens the programme and curriculum module. <br> 3. The Actor then selects "course modification form". <br> 4. The Actor then updates the necessary details and then submits the form. |
| **Post Condition** | The form is submitted successfully and is forwarded to the respective head of department. |

| UCID        | UC#7                         |
|-------------|------------------------------|
| **Usecase name** | forward/reject_course_proposal_form  |
| **Actor**        | Head of Department |
| **Description**  | The user of the system can forward/reject the course addition or modification proposal applied by the faculty. |
| **Pre Condition** | The User must be logged-in through their credentials |
| **Main Flow**    | 1. The Actor logs into the system. <br> 2. The Actor then opens the notifications module. <br> 3. The Actor then checks the notifications related to course addition or modifications proposals. <br> 4. The Actor then verifies and decides to forward or reject. |
| **Post Condition** | The course proposal form will be forwarded to the dean academics for approval or is not forwarded if rejected by Head of department. |

| UCID        | UC#8                         |
|-------------|------------------------------|
| **Usecase name** | approve/reject_course_proposal_form  |
| **Actor**        | Dean academics |
| **Description**  | The user of the system can approve/reject the course addition or modification proposal applied by the faculty. |
| **Pre Condition** | The User must be logged-in through their credentials |
| **Main Flow**    | 1. The Actor logs into the system. <br> 2. The Actor then opens the notifications module. <br> 3. The Actor then checks the notifications related to course addition or modifications proposals. <br> 4. The Actor then verifies and decides to approve or reject. |
| **Post Condition** | The course proposal form will be approved and the Acad admin will be notified to add/modify the course. |

| UCID        | UC#9                         |
|-------------|------------------------------|
| **Usecase name** | add_curriculum  |
| **Actor**        | Acad Admin |
| **Description**  | The Acad admin can add a new curriculum. |
| **Pre Condition** | The User must be logged-in through their credentials |
| **Main Flow**    | 1. The Actor logs into the system. <br> 2. The Actor then opens the Programme and Curriculum module. <br> 3. Actor clicks on the 'Add curriculum' option. <br> 4. Then, the Actor selects the disciplines/elective course, no. of semesters, labs in each Semester, and the Academic load of a particular course. <br> 5. After successfully adding the details, the Actor clicks on Submit. [S1] |
| **Sub Flow**     | S1. Extend "update_curriculum". |
| **Post Condition** | The new curriculum is added with mentioned details. |

| UCID        | UC#10                         |
|-------------|------------------------------|
| **Usecase name** | update_curriculum  |
| **Actor**        | Acad Admin |
| **Description**  | The user of the system can update the existing course. |
| **Pre Condition** | The User must be logged-in through their credentials |
| **Main Flow**    | 1. The Actor logs into the system. <br> 2. The Actor then opens the Programme and Curriculum module. <br> 3. Actor clicks on the "Update curriculum" option. <br> 4. Then, the Actor updates the necessary details. <br> 5. After successfully changing the details, the Actor clicks on Submit. |
| **Post Condition** | An update notification is displayed and the curriculum is successfully updated. |

| UCID        | UC#11                         |
|-------------|------------------------------|
| **Usecase name** | add_new_course  |
| **Actor**        | Acad Admin |
| **Description**  | The user of the system can add a new course. |
| **Pre Condition** | The User must be logged-in through their credentials |
| **Main Flow**    | 1. The Actor logs into the system. <br> 2. The Actor then opens the Programme and Curriculum module. <br> 3. The Actor clicks on the 'Add new course' option. <br> 4. Actor enters the course name along with all the metadata like Course code, Prerequisites, etc. <br> 5. After that, the Actor can add the syllabus of a particular course. <br> 6. After successfully entering the details, the Actor clicks on Submit. [S1] |
| **Sub Flow**     | S1. Extend "update_existing_course". |
| **Post Condition** | The course is added successfully and saved in the database. |

| UCID        | UC#12                         |
|-------------|------------------------------|
| **Usecase name** | update_existing_course  |
| **Actor**        | Acad Admin |
| **Description**  | The user of the system can update the course. |
| **Pre Condition** | The User must be logged-in through their credentials |
| **Main Flow**    | 1. The Actor logs into the system. <br> 2. The Actor then opens the Programme and Curriculum module. <br> 3. Actor clicks on the "Update course" option. <br> 4. The Actor enters the necessary course details to update. <br> 5. After successfully updating the details, the Actor clicks on Submit. |
| **Post Condition** | The course is updated and is saved in the database. |


#### 3.2.1 Browse Program Catalog

- **Actor:** Student, Acad Admin, HOD, Faculty, Dean  
- **Description:** Users can browse the available programs categorically.  
- **Precondition:** User must be logged in.  
- **Main Flow:**  
  1. Log into the system.
  2. Open the Programme and Curriculum module.
  3. Browse available programs.

#### 3.2.2 Browse Curriculum Catalog

- **Actor:** Student, Acad Admin, HOD, Faculty, Dean  
- **Description:** Users can browse available curriculums categorically.  
- **Precondition:** User must be logged in.  
- **Main Flow:**  
  1. Log into the system.
  2. Open the Programme and Curriculum module.
  3. Select a program.
  4. View the curriculums for the program.

#### 3.2.3 Add Program

- **Actor:** Acad Admin  
- **Description:** Acad Admin can add a new program offered by the institute.  
- **Precondition:** User must be logged in.  
- **Main Flow:**  
  1. Log into the system.
  2. Open the Programme and Curriculum module and click on the "Add Program" option.
  3. Add program details, including discipline, batch year, semesters, courses, and academic load.
  4. Submit the form.

---

### 3.3 Other Functional Requirements

- **Search Functionality**
- **Filter and Sort**
- **Integration with other modules (e.g., course registration)**

### 3.4 Other Constraints

#### 3.4.1 User Interfaces

Users will log in using their credentials, access their profile, and browse programs, curriculums, timetables, and academic calendars based on the relevant details (e.g., branch, batch, semester).

#### 3.4.2 Tech Stack Used

- **Database:** PostgreSQL  
- **Backend:** Django

---

## 4. Non-Functional Requirements

- **Performance:** Quick response times for viewing programs, curriculums, timetables, and academic calendars.
- **Scalability:** The system should handle a large number of concurrent users.
- **Availability:** The system should be available 99.9% of the time.
- **Security:** Role-based authorization ensures data confidentiality and integrity.

---

## 5. Module Dependencies with Other Fusion Modules

### 5.1 UI Level

- **User Authentication and Authorization:** 
- Dependency: Users, especially students, need the ability to search
for programs and courses easily. Admins should have filtering
options for efficient course management.
● Implementation: Include search bars, filters, and sorting options to
enhance the user experience. Ensure that admins have convenient
tools for quickly finding and managing courses.
● Example : Full-text search (fts) in a web application involves using
a search engine or a database feature that allows searching through
the content of textual data efficiently.
- **Search and Filtering Functionality:** 
- Full-text search and filters for programs and courses.
- **Data Presentation and Visualization:** Organized layouts for program and course details.

### 5.2 DB Level Dependencies

- `course`
- `programme_curriculum_course`
- `programme_curriculum_course_prerequisite_courses`
- `programme_curriculum_course_disciplines`

### 5.3 Module Level Dependencies

Course registration, notifications and course management modules are the
modules dependent on this module.
The course registration module will require various details like course
name, course id, discipline offered, prerequisites of the course.
The course management module will require course name ,course id and
discipline offered, prerequisites of the course.

The notifications module will require to generate several important
notifications like modification of course, curriculum to the respective users.

