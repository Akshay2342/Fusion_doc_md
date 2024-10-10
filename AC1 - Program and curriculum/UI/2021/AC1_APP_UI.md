## Assignment - 3  Figma Profiles for AC1:
### Programme and Curriculum (Mobile Application)
#### Team Members:
- Arpan Karjee 21BCS032  
- Kanchandeep Kaur 21BCS107  
- Mayuk Sarkar 21BCS132  
- Shiya Shivani 21BCS193  
- Uditi Das 21BCS232  
- **Mentor**: Abhikumar Gupta 21BCS089

### Module Description:
The primary goals of this application revolve around facilitating the addition of new programs and overseeing the curriculum management process for various academic offerings provided by the Institute. The application aims to empower each program to efficiently update and manage its curriculum, specifically catering to different batches within the program. Through this platform, programs can seamlessly introduce new courses and enhance the educational content for improved academic experiences across multiple batches.

The application's scope encompasses the comprehensive range of programs and their respective curriculums offered by the Institute. Users are provided with the capability to seamlessly access and review the curriculum and program requirements relevant to their academic pursuits. Through the application, users can effortlessly navigate and explore the specific curriculum details associated with each program, gaining a clear understanding of the educational components required for successful completion of their chosen academic paths.

### Use Case Diagram:
This image shows all the users with their respective use cases.

![Use Case Diagram](../../Diagrams/usecase.png)

### 3.2 Use Case

## 2. Actors:

### 2.1 User (general):
A general user who can browse the programme and curriculum catalogs to view the available courses and their details.

#### Specific Functionalities:
1. **Browse_programme_catalog**: The user can view the list of programmes offered by the academic institution, along with their details such as duration, eligibility, fees, etc.
2. **Browse_curriculum_catalog**: The user can view the list of curricula for each programme, along with their details such as courses, credits, prerequisites, etc.

The image of the actor and its use cases are described in the above image.  
Link of Figma: It is a general user, so there are no corresponding pages for this user.

### 2.2 Faculty:
A faculty member who can propose new courses or update existing ones, and also approve or forward the proposals to the next level of authority.

#### Specific Functionalities:
1. **Update_course_proposal**: The faculty can modify the details of an existing course proposal, such as title, description, objectives, outcomes, syllabus, etc.
2. **Add_new_course_proposal**: The faculty can create a new course proposal by filling in the required details, such as title, description, objectives, outcomes, syllabus, etc.

The image of the actor and its use cases are described in the above image.  
Link of Figma: [Faculty Figma Link](https://www.figma.com/file/SqbFKe94YvetAGS8ddNDQ1/faculty_ac1_23-DONE?type=design&node-id=0-1&mode=design&t=vaidz82WiLRVSRnx-0)

### 2.3 Student:
A student who can enroll in courses can browse their courses list, but has no direct interaction with the course proposal and approval process.

1. **Browse_programme_catalog**: The student can view the list of programmes offered by the academic institution, along with their details such as duration, eligibility, fees, etc.
2. **Browse_curriculum_catalog**: The student can view the list of curricula for each programme, along with their details such as courses, credits, prerequisites, etc.

#### Specific Functionalities:
Students do not have any additional functionalities; all functionalities of students are covered in general user actors.

The image of the actor and its use cases are described in the above image.  
Link of Figma: [Student Figma Link](https://www.figma.com/file/dpgyUXoWB2MER7g6cPZVvM/student_ac1_23?type=design&node-id=0-1&mode=design&t=lr6n7B3kBAHKswub-0)

### 2.4 Academic Admin:
An academic administrator who can add, update, or delete courses, curricula, and programmes in the system, and also assign faculty members to courses.

#### Specific Functionalities:
1. **Add_new_course**: The academic admin can add a new course to the system, based on the approved course proposal.
2. **Update_course**: The academic admin can update the details of an existing course, such as title, description, objectives, outcomes, syllabus, etc.
3. **Add_curriculum**: The academic admin can add a new curriculum to the system, by specifying the courses, credits, prerequisites, etc.
4. **Update_curriculum**: The academic admin can update the details of an existing curriculum, such as courses, credits, prerequisites, etc.
5. **Add_programme**: The academic admin can add a new programme to the system, by specifying the duration, eligibility, fees, curriculum, etc.
6. **Update_programme**: The academic admin can update the details of an existing programme, such as duration, eligibility, fees, curriculum, etc.

The image of the actor and its use cases are described in the above image.  
Link of Figma: [Academic Admin Figma Link](https://www.figma.com/file/VbRnB3RlDX3VULQhzSCRWQ/AcadADMIN_ac1_23-DONE?type=design&node-id=0-1&mode=design&t=1uYJ2OehkMRDD7ao-0)

### 2.5 Department Head:
A department head who can approve or forward the course proposals to the dean of academics, and also view the status of the proposals.

#### Specific Functionalities:
1. **Approve/forward_course_proposal**: The department head can either approve or forward a course proposal to the dean of academics, depending on their role and authority.
2. **View_course_proposal_status**: The department head can view the status of each course proposal, such as pending, approved, forwarded, rejected, etc.

The image of the actor and its use cases are described in the above image.  
Link of Figma: [Department Head Figma Link](https://www.figma.com/file/6ipMUb7AnbbSgdvmqp9OiV/HEAD_ac1_23-DONE?type=design&node-id=0-1&mode=design&t=ARnXPOcKoUFWzuNG-0)

### 2.6 Dean of Academics:
A dean of academics who can give the final approval for the course proposals, and also view the status of the proposals.

#### Specific Functionalities:
1. **Approve_course_proposal**: The dean of academics can give the final approval for a course proposal, based on their role and authority.
2. **View_course_proposal_status**: The dean of academics can view the status of each course proposal, such as pending, approved, forwarded, rejected, etc.

The image of the actor and its use cases are described in the above image.  
Link of Figma: [Dean Figma Link](https://www.figma.com/file/b7MdLCE7CTkjkqj1yutQ8m/DEAN_ac1_23-DONE?type=design&node-id=0-1&mode=design&t=hZvdDQ7RjugfiqQE-0)

---

## Figma Profile Design Guidelines and Additional Considerations

### 5.1 Cross-Platform Compatibility:
Ensuring comprehensive quality assurance, our focus extends to meticulous checks for cross-platform compatibility in Figma designs. This involves thorough verification to confirm that all features seamlessly function and exhibit consistent design aesthetics across both the web and app versions. By prioritizing this aspect, we enhance accessibility and user satisfaction, delivering a uniform experience regardless of the chosen platform.

We have different Figma files for web and mobile applications, so they are compatible for both web and mobile applications.

### 5.2 Dimension Standardization:
In tandem with cross-platform considerations, dimension standardization plays a pivotal role in our design approach. We advocate for precision by mandating that all Figma designs adhere to specific dimensions. For web designs, the dimensions are set at a standardized 1920 x 1080 pixels, while mobile designs should target an approximate width of 360 pixels. This commitment to uniformity not only streamlines the development process but also fosters a cohesive visual identity, contributing significantly to an elevated and consistent user experience across diverse devices.

In all the mobile Figma pages, dimensions have been targeted with an approximate width of 360 pixels and height of 1004 pixels.

### Actor-oriented Use Case-Based Design:
- Strictly base all Figma designs on use cases of actors and maintain consistency with previous and newly added designs.
  - Each actor should have a different page in Figma.
- If the Figma profiles are already existing, make sure all the actors have their own Figma profiles and also wireframe those across all use cases for that actor.
- Figma link (only) for reference (Figma profiles created by the previous batch): [Fusion App Figma Link](https://www.figma.com/file/pzhw34xBvEK0hm5Yx4bh0P/Fusion-APP?type=design&node-id=0%3A1&mode=design&t=J0f6T5YoUiKbp17u-1)
