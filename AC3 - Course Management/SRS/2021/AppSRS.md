# Software Requirements Specification For Course Management

**Prepared by:**  
- Aditya Gupta (21BCS007)  
- Adarsh Kumar (21BCS006)  
- Advait Manke (21BCS010)  
- K.L. Praseeda Keerthi (21BCS119)  
- Mahanthi Pranitha (21BCS124)

**Student Mentor:**  
- Vedant Bande (21BCS238)

## Table of Contents

1. [Introduction](#1-introduction)  
   1.1 [Introduction about the Fusion](#11-introduction-about-the-fusion)  
   1.2 [Purpose of the module](#12-purpose-of-the-module)  
   1.3 [Scope of the module](#13-scope-of-the-module)
2. [User/Actor Description (Characteristics)](#2-useractor-description-characteristics)  
   2.1 [Student](#21-student)  
   2.2 [Instructor](#22-instructor)
3. [Functional Requirements](#3-functional-requirements)  
   3.1 [Use Case Diagram](#31-use-case-diagram)  
   3.2 [Use Case Description](#32-use-case-description)  
   3.3 [Other Functional Requirements](#33-other-functional-requirements)  
   3.4 [Other Constraints](#34-other-constraints)  
   3.4.1 [User Interfaces](#341-user-interfaces)  
   3.4.2 [Software (Tech) Stack Used](#342-software-tech-stack-used)
4. [Non-Functional Requirements](#4-non-functional-requirements)  
5. [Module Dependencies with Other Fusion Modules](#5-module-dependencies-with-other-fusion-modules)  
   5.1 [UI Level](#51-ui-level)  
   5.2 [DB Level Dependencies](#52-db-level-dependencies)  
   5.3 [Module Level Dependencies](#53-module-level-dependencies)

## 1. Introduction

### 1.1 Introduction About the Fusion – A Brief Description:

FusionIIIT is a student-driven initiative that aims to provide a holistic solution for the seamless integration and automation of diverse functions within PDPM Indian Institute of Information Technology, Design and Manufacturing, Jabalpur. It is crafted with precision using Flutter and powered by the Django Web framework. FusionIIIT encompasses everything from efficient administration management to academic prowess and miscellaneous departmental tasks. It is like a digital wizard that takes care of everything, from organizing the administrative stuff to making academics smoother. It jumps into various departments and sections, making sure every corner of campus life runs smoothly.  
In the admin side, it handles the complicated paperwork and processes. For academics, it brings a digital touch, making learning and managing courses easier. But it doesn't stop there; FusionIIIT is like a friendly companion for all the different parts of the campus, making sure everything works well.  
In simpler terms, FusionIIIT is not just a tool – it's a helpful friend, making life at PDPM IIITDM Jabalpur more organized and enjoyable for everyone.

### 1.2 Purpose of the Module:

The purpose of the module course management is to provide details for instructors to upload course-related materials, assign tasks, and make announcements. The application also assesses the assignments and projects assigned to students and recommends optimal grades for each student. Students can view their performance, course content, submit assignments, and ask questions.

### 1.3 Scope of the Module:

The product scope of this software is to provide a user-friendly and intuitive platform for educational institutions. Lecturers can assign various tasks and view student participation both individually and for the entire course.

---

## 2. User/Actor Description (Characteristics)

### 2.1 Student:

The student actor in the course management module represents individuals who are enrolled in a course and intend to participate in the learning process by engaging with the course content, completing assignments, and taking quizzes. The course management module provides a digital platform for students to access course materials and interact with their instructors and peers.  
**Role:** The student's role is to start learning by logging in, accessing course materials, submitting assignments, taking quizzes, and engaging with course content in the digital realm.  
**Specific Functionalities:**
- Access course materials.
- Submit assignments.
- View performance in previous Assignments.
- View course content and details.
- Download content.

### 2.2 Instructor:

The instructor in the course management module represents individuals who are responsible for teaching a course and intend to manage the learning process by engaging with the course content, assigning assignments, and creating quizzes. The course management module provides a digital platform for lecturers to upload course materials, interact with students, and evaluate their performance.  
**Role:** The instructor, upon logging in, manages courses by uploading materials, creating quizzes, evaluating student work, and reviewing performance data.  
**Specific Functionalities:**
- Upload Content
- Add Assignments
- Evaluate Assignments
- View performances

## 3. Functional Requirements

### 3.1 Use Case Diagram
![Use Case Diagram](../../Diagrams/AC3%20V2.png)

### 3.2 Use Case Description:

##### 3.2.1 View Course Content

| **UC ID**        | UC#1                    |
|------------------|-------------------------|
| **Use Case Name**| View Course Content      |
| **Description**  | The "View Course Content" use case allows both instructors and students to view the content of a course, including videos, lectures, readings, and assignments. |
| **Actor**        | Student                 |
| **Precondition** | 1. The student must be logged-in. 2. Student should have registered in that particular course. |
| **Main Flow**    | 1. The user logs in to the system. <br> 2. The user navigates to the "Courses" tab. <br> 3. The user selects the desired course from the list of available courses. <br> 4. The system displays the course content. <br> 5. The user can view and interact with the course content as permitted by their role. |
| **Post Conditions** | The user has successfully viewed the course content. The system has updated any necessary logs or records. |
| **Alternate Flow**  | AF1: User is not registered for the course.<br> AF2: Technical error during content retrieval or display. |
| **Sub Flow**        | NIL |
| **Global Alternate Flow** | GA1: User cancels the procedure.<br> GA2: System error. |

---

##### 3.2.2 Submit Assignment

| **UC ID**        | UC#2                    |
|------------------|-------------------------|
| **Use Case Name**| Submit Assignment        |
| **Description**  | Student can solve the assignment that is given, submit it, and can check previous assignments. |
| **Actor**        | Student                 |
| **Precondition** | 1. The student must be logged-in. <br> 2. Student should have registered in that particular course. <br> 3. The assignment should be open. |
| **Main Flow**    | 1. Student enters the desired course.<br> 2. Student clicks on "Assignment".<br> 3. The system displays assignments with deadlines.<br> 4. Student views previous assignments and submits the current one. <br> 5. Submission is taken in PDF or DOCS format.<br> 6. Click "Submit".<br> 7. System confirms submission. |
| **Post Conditions** | The student successfully submits the assignment. |
| **Alternate Flow**  | NIL |
| **Sub Flow**        | NIL |
| **Global Alternate Flow** | GA1: Student can cancel the assignment submission. |

---

##### 3.2.3 View Progress

| **UC ID**        | UC#3                    |
|------------------|-------------------------|
| **Use Case Name**| View Progress            |
| **Description**  | The "View Progress" use case allows a student to view their progress in a course, including their marks and attendance. |
| **Actor**        | Student                 |
| **Precondition** | 1. The student must be logged-in. <br> 2. Student should have registered in that particular course. <br> 3. Marks and attendance data should be uploaded by the instructor. |
| **Main Flow**    | 1. Student navigates to "Courses".<br> 2. The system displays registered courses.<br> 3. Student selects a course.<br> 4. Student clicks on "View Progress".<br> 5. System retrieves and displays marks and attendance. |
| **Post Conditions** | The student successfully views their progress. |
| **Alternate Flow**  | A1: Marks or attendance data not available.<br> A2: Technical error while retrieving progress data. |
| **Sub Flow**        | S1: View detailed marks.<br> S2: View attendance details. |
| **Global Alternate Flow** | GA1: Student cancels the procedure. |

---

##### 3.2.4 Download Content

| **UC ID**        | UC#4                    |
|------------------|-------------------------|
| **Use Case Name**| Download Content         |
| **Description**  | The "Download Content" use case allows a student to download course content materials for a registered course. |
| **Actor**        | Student                 |
| **Precondition** | 1. The student must be logged-in.<br> 2. Course content must have been uploaded by the instructor. |
| **Main Flow**    | 1. Student navigates to the desired course.<br> 2. Student clicks on "Content".<br> 3. System displays available content files.<br> 4. Student selects files to download.<br> 5. Student clicks "Download".<br> 6. System initiates download. |
| **Post Conditions** | The content files have been downloaded. |
| **Alternate Flow**  | A1: File not found.<br> A2: File corrupted.<br> A3: Insufficient storage. |
| **Sub Flow**        | NIL |
| **Global Alternate Flow** | GA1: Student cancels the download.<br> GA2: System error. |

---

##### 3.2.5 Manage Courses

| **UC ID**        | UC#5                    |
|------------------|-------------------------|
| **Use Case Name**| Manage Courses           |
| **Description**  | The "Manage Course" use case empowers instructors to administer various aspects of their courses, including adding assignments, managing content, making announcements, and more. |
| **Actor**        | Instructor               |
| **Precondition** | 1. The instructor must be logged-in. <br> 2. The course must exist in the system. |
| **Main Flow**    | 1. Instructor navigates to "Courses".<br> 2. Instructor selects "Manage Course".<br> 3. System displays available courses.<br> 4. Instructor selects a course.<br> 5. System displays course management interface.<br> 6. Instructor performs desired management tasks. |
| **Post Conditions** | Instructor successfully manages the course. |
| **Alternate Flow**  | A1: Course not found. |
| **Sub Flow**        | NIL |
| **Global Alternate Flow** | GA1: Instructor cancels the procedure. |

---

##### 3.2.6 Manage Evaluation

| **UC ID**        | UC#6                    |
|------------------|-------------------------|
| **Use Case Name**| Manage Evaluation        |
| **Description**  | The "Manage Evaluations" use case allows instructors to administer the assessment process for their courses. |
| **Actor**        | Instructor               |
| **Precondition** | 1. The instructor must be logged-in. <br> 2. The course must exist within the system. <br> 3. Students must have submitted assignments. |
| **Main Flow**    | 1. Instructor navigates to "Courses".<br> 2. Instructor selects a course and clicks on "Manage Evaluations".<br> 3. System displays evaluation interface.<br> 4. Instructor manages assignments and evaluations. |
| **Post Conditions** | Instructor successfully completes evaluation tasks. |
| **Alternate Flow**  | NIL |
| **Sub Flow**        | NIL |
| **Global Alternate Flow** | NIL |



### 3.4.1 User Interfaces

- **Flutter framework:** UI development must adhere to Flutter's guidelines and best practices.
- **Cross-platform compatibility:** UI elements must render consistently across Android, iOS, and potentially web.
- **State management:** Efficient management of UI state and data flow using appropriate Flutter techniques (e.g., Provider, BLoC, MobX).
- **Navigation:** Clear and intuitive navigation patterns tailored for mobile experiences.
- **Device-specific features:** Leverage device features like cameras, GPS, or sensors as needed for specific use cases.

### 3.4.2 Software (Tech) Stack Used

- **Frontend:** Flutter (Dart programming language)
- **Backend:** Django (Python), PostgreSQL
- **API communication:** RESTful APIs for data exchange between frontend and backend.
- **Libraries and frameworks:** Potential use of additional libraries for:
  - **Authentication:** (e.g., Django REST framework authentication)

### 3.4.3 Business Rules

- **Enrollment deadlines** (enforced within Django backend logic)
- **Assignment deadlines** (enforced within Django backend logic)
- **Grading policies** (implemented within grading and feedback functionalities)
- **Attendance tracking** (stored and managed in the PostgreSQL database)
- **Communication channels** (integrated into app or provided as external links)
- **User roles and permissions** (handled by Django's authentication and authorization system)

---

## 4. Non-Functional Requirements

### 4.1 Performance

The system ensures fast page loading, rapid response to user interactions, and scalability to accommodate increased users and courses without performance slowdown.

### 4.2 Scalability

The system should scale effortlessly to handle an increasing number of users and courses without compromising performance.

### 4.3 Availability

The system ensures uninterrupted accessibility 24/7, with regular backups for student data and materials, along with established disaster recovery plans for major failures.

### 4.4 Security

The system prioritizes robust user authentication, strong password policies, encrypted sensitive data, frequent security updates, and strict adherence to data privacy regulations.

### 4.5 Usability

The system boasts an intuitive interface for easy learning, provides clear instructions with helpful guidance, and offers accessible online help, tutorials, and support resources for both students and instructors.

---

## 5. Module Dependencies with Other Fusion Modules

### 5.1 UI Level

- Not dependent on other modules

### 5.2 DB Level Dependencies

- Dependent on course list, student list.

### 5.3 Module Level Dependencies

- Dependent on The Program and Curriculum module for providing the approved list of courses.
