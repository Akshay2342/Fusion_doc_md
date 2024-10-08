` `**Assignment - 4  Database Documentation for AC1:** 

` `**Programme and Curriculum  (Mobile Application)**

` `**Team Members:**

- ` `Arpan Karjee 21BCS032
- ` `Kanchandeep Kaur 21BCS107
- ` `Mayuk Sarkar 21BCS132
- ` `Shiya Shivani 21BCS193
- ` `Uditi Das 21BCS232

` `**Mentor :** Abhi Kumar Gupta 21BCS089

**Faculty Mentor - Dr. Vinod Kumar Jain (Head CSE)**




**Overview of the Module:** 

The Overview of PROGRAMME AND CURRICULUM module is to provide addition of new programmes and effective management of various curriculum for different programmes offered in the institute. Each programme could update its curriculum for each batch. The scope of the application covers the entire Programmes and its curriculums offered by the Institute where the user can view their desired curriculum, programme, discipline,courses and batch.

The primary goals of this application revolve around facilitating the addition of new programs and overseeing the curriculum management process for various academic offerings provided by the Institute. The application aims to empower each program to efficiently update and manage its curriculum, specifically catering to different batches within the program. Through this platform, programs can seamlessly introduce new courses and enhance the educational content for improved academic experiences across multiple batches. 

` `● Curriculum Management.

` `● Forwarding of course proposal forms.

● Addition and updation of courses

**SRS:** [**SRS DOCUMENT**](https://docs.google.com/document/d/1uqycWBcVJW0fLlSBgWd_xWl7C0EdnNQY/edit?usp=sharing&ouid=114355705916451598178&rtpof=true&sd=true)


**A. ER Diagram (to be created using draw.io):  [ER Diagram**](https://app.diagrams.net/#G1F8YbIE91DcVfRC5bEs_1bstLXulcfqXQ)**


**B. Database Schema Info (in the Google sheet): [Database Schema of AC-1 Programme and Curriculumn](https://docs.google.com/spreadsheets/d/1YEpbQHbRwxqxqRFjluLj18uyDRRwGiGD/edit#gid=1785439798)** 



**C. Changes required in the currently implemented Tables:-**

**1.)  programme\_curriculum\_course\_prerequesite\_courses**

**●      from\_course\_id**

**a)  Change:** Combining both the attributes into single attribute list\_of\_course\_id

**b)  Justification:**  We need the list of course\_id instead of interval kind of course\_id’s.

**●      to\_course\_id**

` `**a)  Change:** Combining both the attributes into single attribute list\_of\_course\_id

` `**b) Justification:** We need the list of course\_id instead of interval kind of course\_id’s.


**D. Data Availability for API and Functional Testing**

**D.1	Mention the tables that are already populated**

- curriculum
- programme\_curriculum\_batch
- programme\_curriculum\_course
- programme\_curriculum\_course\_disciplines
- programme\_curriculum\_course\_prerequesite\_courses
- programme\_curriculum\_courseslot\_courses
- programme\_curriculum\_courseslot
- programme\_curriculum\_curriculum
- programme\_curriculum\_discipline
- programme\_curriculum\_discipline\_programmes
- programme\_curriculum\_programme
- programme\_curriculum\_semester

  All the above-mentioned tables are working for the web application , but for mobile applications since there are no serializers, so we are working on building serializers and making changes in the views so that  all the required data can be populated in the mobile application also .

**D.2	Mention the tables required to be populated**

- course\_proposal\_form

**D.3**    No Problems Faced.
