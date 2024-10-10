**Module Name \- File Tracking (GAD-4)**  
**Faculty Mentor \- Dr. Avinash Chandra Pandey**  
**Student Mentor \- Priyanshu Aggarwal, Vansh Mittal**	 	 	 		

 **Database Documentation of \[** GAD 4 \- File Tracking System **\] 4.0**

**Overview of the Module:** 

**SRS:** [Link](https://docs.google.com/document/u/0/d/1t1t1nLu7sUACYa1DWW3l45sC31nYY9U9IR3xQQDyhUw/edit)  
**A. ER Diagram (to be created using draw.io):  [ER Diagram](https://app.diagrams.net/?src=about#G1gN5vxqYqs67pQrPvOdHRCJUskix0LfEZ)**   
**B. Database Schema Info (in the Google sheet): [Database Schema](https://docs.google.com/spreadsheets/d/1VwzdAB8SQV-psVPPrHrowAeJNAIXNpELAfc7Kb6e7jg/edit#gid=0)**  
**C. Mention all the changes required in the currently implemented Tables:-**  
**(These changes will be done in this current version 4.0)**

1) File  
* **src\_module:-**  
1) Change: Added a new character field to the File model.  
2) Justification: This addition helps identify the module or source within the system that generated or uploaded the file. This information is valuable for:  
   * Categorizing and tracking files based on their origin.  
   * Improving search and filtering capabilities based on the source module.  
   * Understanding the context and usage of different files within the system.  
* **src\_object\_id** :-

   		      a) Change: Added a new nullable character field to the File model.  
      b) Justification:This addition allows storing an identifier for the specific        object within the source module that the file is associated with. This provides more granular tracking and linking compared to just the module name.

* **file\_extra\_JSON** :-  
  * Change : Added a new nullable JSON field to the File model.  
  * **Justification**: This addition offers a flexible way to store additional information related to the file without modifying the main model structure.

    

    

2) Tracking  
* tracking\_extra\_JSON  
1) Change: Added a new nullable JSON field to the Tracking model.  
2) Justification: This addition offers a flexible way to store additional information related to the file tracking process without modifying the main model structure.

**D. Data Availability for API and Functional Testing**

**D.1	Mention the tables that are already populated**

* File  
* Tracking

**D.2	Mention the tables required to be populated**

* None

**D.3	Mention any difficulties faced by your team regarding populating any table (if any)**  
