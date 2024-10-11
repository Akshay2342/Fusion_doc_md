**Module Name - OS3** – **web \_notifications Faculty Mentor – Dr. Neelam Dayal**

**Student Mentor – Sudhanshu Patil(21bcs209)**

**Database Documentation of [** OS3 – web notifications**] 4.0**

**Overview of the Module:**

Notify the User about relevant events, such as interactions with their content and updates from others students and faculty. For every module there will be different type of notifications according to the unique needs and activities associated with each individual module.

- View notification
- Delete notification
- Make announcement
- Mark as read
- Mark as unread

**SRS: [https://drive.google.com/file/d/1tfBk8F1_bgLN68eDFhznlMFbS5u1owCB/view?usp=s haring](https://drive.google.com/file/d/1tfBk8F1_bgLN68eDFhznlMFbS5u1owCB/view?usp=sharing)**

1. **ER Diagram (to be created using draw.io): [ER Diagram**](https://drive.google.com/file/d/1TYsMXQbP7nvFQ0lj9dBwEdmPlpmIS-YD/view?usp=sharing)**
1. **Database Schema Info (in the Google sheet): [Database Schema**](https://docs.google.com/spreadsheets/d/17lIl4pC3DOH7_vfMSTPSIP5UptSBacl6/edit?usp=sharing&ouid=102720302826588816157&rtpof=true&sd=true)![](Aspose.Words.b9953cfc-8252-44a6-93e4-52fba2a67378.001.png)**
1. **Changes required in the currently implemented Tables:-**

1\. notifications\_notification

- No changes
4. **Data Availability for API and Functional Testing D.1 Mention the tables that are already populated**
- Id
- level
- unread
- verb
- timestamp
- public
- action\_object\_id
- recipient\_id
- deleted
- emailed
- data
- actor\_content\_type\_id

**D.2 Mention the tables required to be populated**

- description
- target\_content\_type\_id

**D.3 Mention any difficulties faced by your team regarding populating any table (if any)**

- It is difficult to understand the purpose of the attributes as there are multiple attributes which nearly have the same meaning and it will create a confusion to see the format of data in the database
