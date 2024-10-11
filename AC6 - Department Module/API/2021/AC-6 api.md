**APIStatus**

**of**

**Department Module (AC6 Mobile)**

Faculty Mentor: Dr. Pritee Khanna Mentor: Varun Sundeep Singh(21BCS237)

Team Members:

Anoop Kumar(21BCS026) Alok Kumar(21BCS018) Ankit Singh(21BCS024) Dharavath Vinod(21BCS076) Vishal Parihar(21BCS244)

**Module Name** - Department AC6

**Student Mentor** - Varun Sundeep Singh(21BCS237)

**Please mention all the APIs used in the module below**

1\.{/} name = dep [Implemented]

- Parameters : none
- Description : make and browse announcements

2\.{facView/} name = faculty\_view [Implemented]

- Parameters : request
- Description : request contains metadata about the requested page

3\.{staffView/} name = staff\_view [Implemented]

- Parameters : request
- Description : request contains metadata about the requested page

4\.{All\_Students/bid} name = all\_students [Badly Implemented]

- Parameters : request , bid
- Description : request contains metadata about the requested page , bid stores key for batches

5\.{approved/} name = approved [Implemented] \*\*(to be removed)

- Parameters : request
- Description : request contains metadata about the requested page ; approve requests

6\.{deny/} name = deny [Implemented] \*\*(to be removed)

- Parameters : request
- Description : request contains metadata about the requested page ; deny requests

7\.{alumni/} name = alumni [Yet to be Implemented]

- Parameters : none
- Description : list of alumni filtered on the basis of their department

**Overview of the module:-**

The purpose of the module is to showcase all available departments, faculty and resources available in this institute, along with the ability to view various announcements made by the faculty and staff members. The department view will display information regarding the department and facilities offered in the concerned department student details, faculty details, alumni details, and published announcements if any.

The actors in this module are Student, Faculty and Staff.

APIs:-

**Already Implemented**

- **browse\_announcements :**
- *API Index 1* :
- The browse\_announcements function is designed to facilitate the browsing of announcements department-wise, as made by various faculties and administrators.
- Database - **department\_announcements** table is used to store all announcements and their information.
- **view\_department\_details :**
- API index 1 :
- Displays information regarding a particular department fetched from **department\_notification.**
- Database - globals\_department\_info table is used to fetch information regarding the department.
- **view\_faculty\_details** :
- API index 1
- Displays information regarding a particular department fetched from **department\_notification.**
- Database - globals\_department\_info table is used to fetch information regarding the department.
- **view\_students\_details**:
- API Index 4 :
- Fetches a list of all students according to their department and year (bid).
- Database - **globals\_extrainfo** table is used to fetch a list of students filtered on the basis of department and year and branch.
- **make\_announcemen**t:
- API index 2:
- facView opens faculty view through which a faculty is able to make announcements and view all requests made to him.
- Database- **department\_announcements and department\_specialrequest** tables are used to fetch announcements and requests made to the faculty.
- **make\_announcement** :
- API index 3 :
- staffView opens the staff view through which a staff member is able to make announcements..
- Database- **department\_announcements** is used .

**Yet to be Implemented**

- **view\_alumni\_details :**
- API index 7 :
- It should open a list of alumni filtered on the basis of their department.The implementation should be as follows :
  - Upon clicking on the tab it should display sections for department after which it should display a list of alumni which should contain a link to alumni’s profile similar to how view\_faculty\_details work.
- Database- this data should be taken from the placement module when implemented.

**Current problems with the module / use cases —**

- [view\_faculty\_details] : the list of faculties is fetched but some of the links are invalid as their ID should be integer but they are string. The data type of all faculty ID needs to be changed into the same input type as the function displaying their details.
- [All\_students/bid] : implementation of this API is very repetitive which could be further optimized. Every possible case is listed inside an if-else conditional statement which is highly optimizable.
- [view\_department\_details] : this function for faculty does not exist and needs to be implemented.
- DRF/Serialiser not implemented . The Serializer converts complex data types, supports validation, handles nested relationships, and integrates seamlessly with Django models. In production, DRF accelerates API development, provides authentication and permission features, supports versioning, and generates user-friendly documentation. The Serializer ensures efficient data conversion and validation, contributing to the rapid and reliable development of APIs in Django applications.
- Bad naming conventions

Document link:

[API Status AC6 Mobile App](https://docs.google.com/document/d/1HO_7TOPpjRAkQ-dGLJMWp3wTBxN8G0ftfmbGwGZcF1M/)
