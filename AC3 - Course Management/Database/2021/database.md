# Module Name - AC3 - Course Management (Web)  
**Faculty Mentor** - Dr. Munesh Singh  
**Student Mentor** - Saurav Raj (21BCS188)  

## Database Documentation of [ AC3 - Course Management ] 4.0  

### Overview of the Module:  

**SRS:** AC-3-Course Management System-SRS  
**A. ER Diagram:** [ER Diagram](https://drive.google.com/file/d/1QccI4zwpUvrC2fQMbNgrI9n6jj4sk9YW/view)  
**B. Database Schema Info:** [Database Schema Info](https://docs.google.com/spreadsheets/d/1TtxJFzr0i6OAhG5gcIT_0zUuhYhWbpUkVTRjCDvV5Z8/edit?gid=0#gid=0)  

### C. Changes required in the currently implemented Tables:-  

**Change - Schemas removed - (10)**  
- online_cms_credentialsmodel  
- online_cms_practice  
- online_cms_practicequestion  
- online_cms_question  
- online_cms_questionbank  
- online_cms_quiz  
- online_cms_quizresult  
- online_cms_quizquestion  
- online_cms_studentanswer  
- online_cms_topics  

**Justification:** Excluded from the updated Use case Diagram  

**Change - New schemas added - (2)**  
- online_cms_gradingscheme  
- online_cms_announcements  

**Justification:** New use cases in updated Use Case Diagram  

### D. Data Availability for API and Functional Testing  

**D.1 Mention the tables that are already populated**  
- Course  
- Curriculum  
- Curriculum_Instructor  
- Register  
- academic_information_student  
- globals_extrainfo  
- Calendar  
- Timetable  
- online_cms_assignment  
- online_cms_coursedocuments  
- online_cms_forum  
- online_cms_forumreply  
- online_cms_studentassignment  
- SemesterMarks  

**D.2 Mention the tables required to be populated**  
- Student_attendance  
- online_cms_coursevideo  
- online_cms_gradingscheme  
- online_cms_announcements  

**D.3 Mention any difficulties faced by your team regarding populating any table (if any)**  
NIL  
