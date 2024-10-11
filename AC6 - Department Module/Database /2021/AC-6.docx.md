**Module Name - Department**

**Faculty Mentor - Dr. Pritee Khanna**

**Student Mentor - Varun Sundeep Singh(21BCS237) Team -**

**Anoop Kumar(21BCS026)**

**Alok Kumar(21BCS018)**

**Ankit Singh(21BCS024)**

**Dharavath Vinod(21BCS076)**

**Vishal Parihar(21BCS244)**

**Database Documentation of [ AC6 - DEPARTMENT ] 4.0**

**Overview of the Module:**

The purpose of the module is to showcase all available departments, faculty and resources available in this institute, along with the ability to view various announcements made by the faculty and staff members.

The department view will display information regarding the department and facilities offered in the concerned department student details, faculty details, alumni details, and published announcements if any. The actors in this module are Student, Faculty and Staff.

**SRS:**

1. **ER Diagram (to be created using draw.io): [ER_Department**](https://drive.google.com/file/d/1R9Eqdu1zwO9aVOcANrerL7bOq9gjoMYL/view)**
1. **Database Schema Info (in the Google sheet): [Department Database Info**](https://docs.google.com/spreadsheets/d/1F1ZwnPJga40VgInpQ13APgLfGQqmtW65-JlhT4SDmEE/edit#gid=0)**
1. **Mention all the changes required in the currently implemented Tables:-**

**(These changes will be done in this current version 4.0)**

1\.)department\_announcements

- Table name
  - Change: change to
  - Justification: bad naming convention
- Id
  - Change: name change to id
  - Justification: does not follow naming convention
- ann\_date
  - Change: name change to announcement\_date
  - Justification: readability improvement
- maker\_id\_id
1) Change: name change to announcement\_maker\_id
1) Justification: readability improvement

2\.)department\_specialrequest

- Complete table
1) Change: Remove the table
1) Justification: Functionality not required.
4. **Data Availability for API and Functional Testing D.1 Mention the tables that are already populated**
- department\_announcements

**D.2 Mention the tables required to be populated**

- None

**D.3 Mention any difficulties faced by your team regarding populating any table (if any)**

- view\_faculty\_details API which utilizes EIS module throws an error for IDs which are not integer as some IDs are string.
