# Assignment - 4 Database Documentation for AC1: 
## Programme and Curriculum (Mobile Application)

**Team Members:**
- Arpan Karjee 21BCS032
- Kanchandeep Kaur 21BCS107
- Mayuk Sarkar 21BCS132
- Shiya Shivani 21BCS193
- Uditi Das 21BCS232

**Mentor:** Abhi Kumar Gupta 21BCS089  
**Faculty Mentor:** Dr. Vinod Kumar Jain (Head CSE)

## Overview of the Module: 
The Overview of PROGRAMME AND CURRICULUM module is to provide addition of new programmes and effective management of various curriculum for different programmes offered in the institute. Each programme could update its curriculum for each batch. The scope of the application covers the entire Programmes and its curriculums offered by the Institute where the user can view their desired curriculum, programme, discipline, courses and batch. The primary goals of this application revolve around facilitating the addition of new programs and overseeing the curriculum management process for various academic offerings provided by the Institute. The application aims to empower each program to efficiently update and manage its curriculum, specifically catering to different batches within the program. Through this platform, programs can seamlessly introduce new courses and enhance the educational content for improved academic experiences across multiple batches. 
- Curriculum Management.
- Forwarding of course proposal forms.
- Addition and updation of courses.

## SRS: SRS DOCUMENT

### A. [ER Diagram](https://app.diagrams.net/#G1F8YbIE91DcVfRC5bEs_1bstLXulcfqXQ)
(to be created using draw.io): ER Diagram

### B. [Database Schema Info](https://docs.google.com/spreadsheets/d/1YEpbQHbRwxqxqRFjluLj18uyDRRwGiGD/edit#gid=1785439798)
(in the Google sheet): Database Schema of AC-1 Programme and Curriculum

### C. Changes required in the currently implemented Tables:
1. **programme_curriculum_course_prerequesite_courses**
   - **from_course_id**
     - **Change:** Combining both the attributes into single attribute list_of_course_id
     - **Justification:** We need the list of course_id instead of interval kind of course_id’s.
   - **to_course_id**
     - **Change:** Combining both the attributes into single attribute list_of_course_id
     - **Justification:** We need the list of course_id instead of interval kind of course_id’s.

### D. Data Availability for API and Functional Testing

**D.1  Mention the tables that are already populated**
- curriculum
- programme_curriculum_batch
- programme_curriculum_course
- programme_curriculum_course_disciplines
- programme_curriculum_course_prerequesite_courses
- programme_curriculum_courseslot_courses
- programme_curriculum_courseslot
- programme_curriculum_curriculum
- programme_curriculum_discipline
- programme_curriculum_discipline_programmes
- programme_curriculum_programme
- programme_curriculum_semester

All the above-mentioned tables are working for the web application, but for mobile applications since there are no serializers, so we are working on building serializers and making changes in the views so that all the required data can be populated in the mobile application also.

**D.2 Mention the tables required to be populated**
- course_proposal_form

**D.3** No Problems Faced.   
