# Software Requirements Specification

## Module - AC3

### Course Management (Web)

**Prepared by:**
- Ashu Srivastava (21BCS042)
- Ashutosh Choudhary (21BCS043)
- Ayush Sonkar (21BCS048)
- Ayush Srivastava (21BCS049)
- Daksh Bajaj (21BCS068)

**Faculty Mentor** - Dr. Munesh Singh  
**Student Mentor** - Saurav Raj (21BCS188)

---

## Table of Contents

1. [Introduction](#1-introduction)  
   1.1 [Introduction About Fusion](#11-introduction-about-fusion)  
   1.2 [Purpose of the Module](#12-purpose-of-the-module)  
   1.3 [Product Scope](#13-product-scope)
2. [Use case/Actor Description](#2-useractor-description-characteristics)
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

### 1.1 Introduction About Fusion

Fusion IIIT at PDPM Indian Institute of Information Technology, Design, and Manufacturing, Jabalpur, is a sophisticated integration of functions, showcasing the seamless fusion of diverse operations through the adept use of Python 3.8 and the robust Django Web framework. This student-driven initiative has been meticulously crafted to enhance the operational dynamics of the institute. From streamlining administrative processes to boosting academic excellence and handling various departmental tasks, FusionIIIT emerges as a comprehensive solution, orchestrating the nuances of campus life with finesse.

Think of FusionIIIT as a digital maestro, orchestrating the symphony of campus life. It goes beyond traditional boundaries, delving into every facet of the institute to ensure a harmonious experience. On the administrative front, it navigates through complex paperwork and processes, simplifying the intricacies. In the academic realm, it introduces a digital touch, making learning and course management more accessible. However, FusionIIIT's impact transcends these domains; it functions as a genial companion, extending its support to every nook and cranny of campus life, ensuring seamless operations.

In essence, FusionIIIT is not merely a tool, it's a friendly guide, dedicated to organizing and enhancing the quality of life for everyone at PDPM IIITDM Jabalpur.

### 1.2 Purpose of the Module

The main objective of our module in this application is to offer a platform for Instructors and students to work hand in hand. Its primary purpose is to streamline and enhance the management of courses, providing benefits to both students and faculty. Instructors can upload course-related documents, assignments, quizzes and also make announcements. Students are able to see their performance, course content, submit assignments, and ask related queries. The application also lets Instructors evaluate the assignment, and projects allotted to students and recommends optimal grades for each student.

### 1.3 Product Scope

A streamlined platform for students to effectively manage their academic courses. The product will include features like the ability to showcase courses with details such as name, code, instructor, and schedule, coupled with user-friendly search and filtering options. The system also addresses the optimal display of courses, incorporating pagination or infinite scroll for improved navigation through course listings.

A dedicated section for each course facilitates easy access to course materials and resources in various file formats. The portal further supports announcements, allowing instructors to communicate important updates and events. Comprehensive course-related information, including credits, and instructor details, is presented along with external resource links. Additional considerations encompass secure user authentication, personalized profiles, notification features, and adherence to accessibility standards.

---

## 2. User/Actor Description (Characteristics):

### 2.1 Student:

Represents all the students who intend to complete the course and receive all the important announcements and course updates (attendance, course timetable, assignments, projects, and their marks) made by the Instructor.  
**Role**: Enroll in the course and access the content provided by the instructor  
Access Course Content and details, download the assignment, and see previous quiz performance.

#### Specific Functionalities:
- Access Course Content and details
- Download assignment
- See previous quiz performance
- See the Attendance uploaded by the instructor

### 2.2 Instructor:

Represents all the Instructors who intend to provide the course content, announcements, and projects/assignments to the students who can access them at a common portal in Fusion.  
**Role**: Share the course link/portal with the students and all the important information and contents on the portal.

#### Specific Functionalities:
- Make announcements for the courses offered
- Upload Content (important notes) on the course portal
- Add assignments and course-related projects on the portal of the course
- Share the grading scheme with the students
- Share the grades of all the students of a particular course

### 2.3 Acad Admin:

Represents the Academic Administrator of the college responsible for managing other academic procedures such as creating a timetable and creating an academic calendar.  
**Role**: Add the necessary information on the portal required for efficient flow of academic procedures.

#### Specific Functionalities:
- Uploads the latest Timetable for the new semester
- Uploads the Academic calendar for the new academic year

---

## 3. Functional Requirements:

### 3.1 Use Case Diagram:
![Use Case Diagram](../../Diagrams/AC3%20V2.png)

### 3.2 Use Case Description:

##### 3.2.1 manage_evaluations

| **UC ID**         | UC#1                                   |
|-------------------|----------------------------------------|
| **Use Case Name**  | manage_evaluation                      |
| **Description**    | The manage_evaluation use case allows Instructors to assess various submissions of students. |
| **Actor**          | Instructor                             |
| **Precondition**   | The instructor must be logged in.      |
| **Main Flow**      | 1. The instructor chooses the desired courses from the list of courses displayed by the system.<br>2. The instructor clicks on the Manage Evaluations tab.<br>3. The instructor chooses the desired action and is redirected to the specific page. |
| **Post Conditions**| Assignment scores and grades are recorded. |
| **Alternate Flow** | A1: If not already specified, the instructor creates a grading scheme for how scores will be calculated and translated into grades.<br>A2: 1. The instructor selects from assignments that need to be evaluated.<br>2. The instructor evaluates and records scores, which are reflected in the database.<br>A3: The instructor views the details of submitted assignments under the view_submission field. |
| **Sub Flow**       | NIL                                    |
| **Global Alternate Flow** | NIL                            |

##### 3.2.2 manage_course

| **UC ID**         | UC#2                                   |
|-------------------|----------------------------------------|
| **Use Case Name**  | manage_course                          |
| **Description**    | The Instructor can manage all the course-related information. |
| **Actor**          | Instructor                             |
| **Precondition**   | 1. The Instructor must be logged in.<br>2. The Instructor must be in charge of some courses. |
| **Main Flow**      | 1. Instructor selects from the list of courses where changes need to be made.<br>2. Instructor chooses from the options to make changes.<br>3. Instructor adds or updates the necessary changes. |
| **Post Conditions**| 1. The system relays the changes made by the Instructor to other actors.<br>2. The uploaded content is stored in the database. |
| **Alternate Flow** | A1: Instructor makes an announcement about the course.<br>A2: 1. Instructor clicks on the upload content tab for the selected course.<br>2. Instructor uploads the course content.<br>A3: 1. Instructor uploads assignments.<br>A4: Instructor views course content.<br>A5: Instructor adds or marks attendance. |
| **Sub Flow**       | NIL                                    |
| **Global Alternate Flow** | NIL                            |

##### 3.2.3 view_course_content

| **UC ID**         | UC#3                                   |
|-------------------|----------------------------------------|
| **Use Case Name**  | view_course_content                    |
| **Description**    | Students can view the content of various courses they are enrolled in. |
| **Actor**          | Student                                |
| **Precondition**   | 1. The Student must be logged in.<br>2. Student must be registered in that particular course. |
| **Main Flow**      | 1. The system displays the list of registered courses.<br>2. Student selects the desired course.<br>3. Student clicks "View Content".<br>4. Student selects the type of information they want (assignments, modules, or announcements).<br>5. Student views or downloads the content. |
| **Post Conditions**| Students can view and access specific content they want. |
| **Alternate Flow** | A1: The system displays all assignments.<br>A2: The system displays course modules.<br>A3: Student views announcements in the notifications tab. |
| **Sub Flow**       | NIL                                    |
| **Global Alternate Flow** | NIL                            |

##### 3.2.4 submit_assignment

| **UC ID**         | UC#4                                   |
|-------------------|----------------------------------------|
| **Use Case Name**  | submit_assignment                      |
| **Description**    | Students can solve and submit assignments, and check previous submissions. |
| **Actor**          | Student                                |
| **Precondition**   | 1. The student must be logged in.<br>2. Student must be registered in the course.<br>3. The assignment must be open. |
| **Main Flow**      | 1. Student selects the course.<br>2. Student clicks "Assignment".<br>3. The system displays assignments with deadlines.<br>4. Student views previous assignments.<br>5. Student submits current assignment.<br>6. Submissions can be PDF/DOC/ZIP.<br>7. Student clicks "Submit".<br>8. The system confirms submission. |
| **Post Conditions**| Student successfully submits or resubmits assignments. |
| **Alternate Flow** | NIL                                    |
| **Sub Flow**       | NIL                                    |
| **Global Alternate Flow** | Student can cancel the assignment. |

##### 3.2.5 view_progress

| **UC ID**         | UC#5                                   |
|-------------------|----------------------------------------|
| **Use Case Name**  | view_progress                          |
| **Description**    | Students can view their progress within a course. |
| **Actor**          | Student                                |
| **Precondition**   | 1. The student must be logged in.<br>2. Student must be enrolled in the course.<br>3. Progress data must be available. |
| **Main Flow**      | 1. List of registered courses is displayed.<br>2. Student selects a course.<br>3. Student chooses "View Marks" or "View Attendance".<br>4. Student is redirected to the respective page. |
| **Post Conditions**| Students have a clear understanding of their progress in the course. |
| **Alternate Flow** | A1: Students view detailed marks.<br>A2: Students view attendance records. |
| **Sub Flow**       | NIL                                    |
| **Global Alternate Flow** | NIL                            |

##### 3.2.6 download_content

| **UC ID**         | UC#6                                   |
|-------------------|----------------------------------------|
| **Use Case Name**  | download_content                       |
| **Description**    | Students can download course content provided by the Instructor. |
| **Actor**          | Student                                |
| **Precondition**   | 1. The student must be logged in.<br>2. Student must be registered in the course. |
| **Main Flow**      | 1. System displays the course list.<br>2. Student selects a course.<br>3. Student clicks "Download Content".<br>4. System displays files shared by the instructor.<br>5. Student downloads desired files. |
| **Post Conditions**| Students download the course content.   |
| **Alternate Flow** | NIL                                    |
| **Sub Flow**       | NIL                                    |
| **Global Alternate Flow** | NIL                            |

##### 3.2.7 add_time_table

| **UC ID**         | UC#7                                   |
|-------------------|----------------------------------------|
| **Use Case Name**  | add_time_table                         |
| **Description**    | The add_time_table use case allows the Acad admin to upload the latest timetable for the upcoming or ongoing semester. |
| **Actor**          | Acad admin                             |
| **Precondition**   | The Acad admin must be logged in.      |
| **Main Flow**      | 1. The Acad admin visits the course management module.<br>2. The Acad admin clicks "Add Timetable".<br>3. The Acad admin uploads the timetable file (PDF/DOCX). |
| **Post Conditions**| The timetable is recorded in the database. |
| **Alternate Flow** | NIL                                    |
| **Sub Flow**       | NIL                                    |
| **Global Alternate Flow** | NIL                            |

##### 3.2.8 add_academic_calendar

| **UC ID**         | UC#8                                   |
|-------------------|----------------------------------------|
| **Use Case Name**  | add_academic_calendar                  |
| **Description**    | The add_academic_calendar use case allows the Acad admin to upload an updated academic calendar for the new academic year. |
| **Actor**          | Acad admin                             |
| **Precondition**   | The Acad admin must be logged in.      |
| **Main Flow**      | 1. The Acad admin visits the course management module.<br>2. The Acad admin clicks "Add Academic Calendar".<br>3. The Acad admin fills in the table of events and finalizes the calendar. |
| **Post Conditions**| The new academic calendar is displayed. |
| **Alternate Flow** | NIL                                    |
| **Sub Flow**       | NIL                                    |
| **Global Alternate Flow** | NIL                            |


### 3.3 Other Functional Requirements

1. This module will make use of the communication module for sending notifications and alerts to various actors involved in the module regarding new uploads, extra information, or modifications, etc.  
2. The downloading and uploading system for downloading course content and other course material.  
3. Alerts regarding deadlines for submission of tasks.  
4. The Super admin of Fusion should be able to assign roles for students and instructors.

### 3.4 Other Constraints

#### 3.4.1 User Interfaces

The user interface should comply with the color scheming and dashboard design of FusionIIIT. Users should be able to navigate from one functionality to another. Inter-module navigation should be smooth. All the functionalities should be easy to use and no specific training should be required for the usage of the module.

#### 3.4.2 Software (Tech) Stack Used

- ##### 3.4.2.1 Frontend

  - **HTML**: The application's user interface is developed using HTML for structuring web content  
  - **CSS**: Styling in our application

- ##### 3.4.2.2 Backend

  - **Django**: Python web framework employed for building the application's back-end logic, facilitating efficient development and integration

- ##### 3.4.2.3 Database

  - **PostgreSQL**: The relational database management system (RDBMS) used for storing and managing application data with a focus on scalability and performance.

- ##### 3.4.2.4 Version Control

  - **Git**: Git is a distributed version control system that is widely used for tracking changes in source code during software development.

#### 3.4.3 Business Rules

1. Users must authenticate using a valid username and password to access the system.  
2. Different user roles (e.g., admin, faculty, student) have distinct access permissions, and access is restricted based on these roles.  
3. The system must comply with data privacy regulations, ensuring that sensitive user information is securely stored and accessed only by authorized personnel.  
4. Uploaded files must follow a specific naming convention for consistency and easier management.

## 4. Non-Functional Requirements

### 4.1 Performance

The system should be scalable for concurrent users and for huge data volumes of different actors.

### 4.2 Reliability

The system should have availability and fault-tolerant error handling.

### 4.3 Security

Data encryption for sensitive information and role-based access control should be there in the product to ensure security.

### 4.4 Usability

The product will have a consistent and intuitive user interface.

### 4.5 Scalability

Database scalability for courses and users.

### 4.6 Maintainability

Modular architecture for easy updates.

## 5. Module Dependencies with Other Fusion Modules

### 5.1 UI Level

The Course Management module can be accessed from the dashboard (the very first page after login) or from the sidebar. There are different tabs within the module for all the actors as different actors have different tasks to perform. The UI design for the Course Management module is correlated to the overall design of Fusion IIIT and other Fusion modules.

### 5.2 DB Level Dependencies

The following schemas are shared with other modules:
1. **Course** - Imported from the Academic information module. Used by all other course-related modules.  
2. **Student** - Imported from the Academic information module for Student information.  
3. **Curriculum** - Imported from the Academic information module  
4. **Curriculum_Instructor** - Imported from the Academic information module.  
5. **Student_attendance** - Imported from the Academic information module.  
6. **Register** - Imported from the Academic procedures module. Used to find the courses a student is registered in.  
7. **ExtraInfo** - Global schema.

### 5.3 Module Level Dependencies

- **AC1 - Program and curriculum** - Getting predefined course and curriculum details  
- **AC2 - Course Registration** - All the information related to adding, removal, or updation of courses among different actors have to be coordinated.  
- **AC4 - Other academic Procedures** - Probable dependencies include finalizing of marks, grades, and Course List.  
- **GAD4 - File Tracking** - Uploads and downloads of files (Assignments, etc)  
- **OS3 - Notifications** - Announcements