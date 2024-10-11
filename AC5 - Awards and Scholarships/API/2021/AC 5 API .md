Fusion ERP 

**API Implementation Analysis**

For 

**Awards and Scholarships Module (AC5 - APP)** 

Team mentor - **Dr. Ayan Seal**

Prepared by - 

1. Abhishek Muwal (21BCS005) 
1. Ajay Sharma (21BCS014) 
1. Aryan Atri (21BCS036) 
1. Deepak Meena (21BCS071) 
1. Sukram (21BCS212) 

Team Lead – Soham Bakul Sarode  

INDEX

1. *student\_view* (‘student\_view/$') 
1. *convener\_view* (‘convener\_view/$’) 
1. *staff\_view* (‘staff\_view/$’) 
1. *stats* (‘stats/$’) 
1. *convenerCatalogue* (‘convenerCatalogue/$’) 
1. *getWinners* (‘getWinners/$’) 
1. *get\_MCM\_Flag* (‘get\_MCM\_Flag/$’) 
1. *getConvocationFlag* (‘getConvocationFlag/$’) 
1. *getContent* (‘getContent/$’) 
1. *updateEndDate*(‘updateEndDate/$’) 

API Analysis

Module overview:-

- The **Award and Scholarship Portal** is designed to serve as a comprehensive platform for students at IIITDMJ. Through this portal, all students can access information regarding various convocation medals, awards, and scholarships. 
- Eligible students have the opportunity to submit applications for these honors. 
- The portal ensures that students receive timely notifications regarding application deadlines and the necessary procedures. This automated system aims to provide a streamlined and efficient alternative to the current manual application process. 

Api Counts:- Already made APIs - [count], Yet to be made API - [count] (estimated).

Implemented -

A general **user** can perform the following tasks - 

- **Browse Catalog**: Allows students to explore available courses and programs. 
- **View SPACS Member Details**: Access information about members of SPACS. 
  - **View Previous Award Winners**: Review details about past award recipients. 
1. *student\_view* (‘student\_view/$') - extends **user** 
- **Apply for MCM Scholarships and Convocation Medals**: Submit 

applications for academic honors. 

- **View Application Status**: Check the status of submitted scholarship and 

medal applications. 

2. *convener\_view* (‘convener\_view/$’) - extends **user** 
- **Invite Applications**: Allows the convener to invite applications for MCM scholarships and convocation medals. 
- **View Recent Invite Application Status**: Check the status of recently invited applications. 
- **Update End Date**: Modify the end date for the application invitation period. 
- **View Submitted Applications**: Access details of MCM and convocation medal applications submitted by students. 
- **View Files**: Examine files attached to applications for further evaluation. 
- **Accept or Reject Applications**: Provide the convener with the option to accept or reject submitted applications. 
3. *staff\_view* (‘staff\_view/$’) - extends **user** 
- **View Submitted Applications**: Access details of MCM and convocation medal applications submitted by students. 
- **View Files**: Examine files attached to applications for further evaluation. 
- **Verify or Reject Applications**: Provide the spacs assistant with the option to verify or reject submitted applications. 
4. *stats* (‘stats/$’) 
- The *stats* API allows users to retrieve information about previous award winners. 
5. *convenerCatalogue* (‘convenerCatalogue/$’) 
- Handles managing and retrieving catalog information for awards and scholarships. 
- It handles both updating the catalog content when a POST request is received and retrieving the catalog content when a GET request is made. 
6. *getWinners* (‘getWinners/$’) 
- The function is designed to retrieve information about winners of a specific award for a given batch year and program. It handles the retrieval of related student information, populates the context dictionary, and returns a JSON response indicating the success or failure of the operation along with the winner details if successful. 
7. *getContent* (‘getContent/$’) 
- Retrieve content for a specified award from the Award\_and\_scholarship model. - Returns a JSON response containing the result status and, if successful, the content of the award's catalog. 
8. *updateEndDate*(‘updateEndDate/$’) 
- Update the deadline for a form opened by SPACS (Space Programming and Advisory Committee) convener or assistant 

Partially Implemented -

1. *get\_MCM\_Flag* (‘get\_MCM\_Flag/$’) 
- Retrieves MCM\_flag information. 
- Issue: Response indicates a failure with a downloaded text file and mcm\_flag set to false. 
2. *getConvocationFlag* (‘getConvocationFlag/$’) 
- Retrieves convocation\_flag information. 
- Issue: Response indicates a failure with a downloaded text file and mcm\_flag set to false. 

Use cases:

1. **Browse\_catalogue** 

Description:User of the system can browse the available medals/scholarships categorically api: *#1, #2 , #3* 

2. **View\_staff\_details** 

Description:Users of the system can view administration in charge of the system, and other related staff details. This is required so student may contact authority to ask query regarding any of medals/scholarship api:*#1, #2, #3* 

3. **view\_previous\_winners** 

Description:Users can view previous year’s winners for various convocation medals and MCM Scholarship api:*#1, #2, #3* 

4. **apply\_for\_convocation\_medals** 

Description:The student can apply for Convocation Medals by filling out a form and uploading necessary documents. api:*#1* 

5. **apply\_for\_mcm\_scholarship** 

Description:The student can apply for MCM scholarship by filling out a form and uploading necessary documents. api:*#1* 

6. **track\_application\_status** 

Description:Students view application status for each of the applied medals/scholarships. api:*#1* 

7. **process\_verified\_applications** 

Description:The actor is able to browse the awards/scholarships applications. While browsing he also gets a facility to sort them according to CPI, Income etc.This feature provides in depth statistics about the applicants. api:*#2* 

8. **manage\_catalogue** 

Description:The actor can make changes to the application procedure and also scrap the existing awards/prizes/scholarship. api:*#5* 

9. **invite\_applications** 

*Description*:He can invite the applications for the MCM scholarship or awards (if necessary) for all the students who satisfy the criteria as mentioned in SPACS manual. api:*#2* 

10. **process\_submitted\_applications** 

Description:The actor is able to browse the awards/scholarships applications. While browsing he also gets a facility to sort them according to CPI, Income etc.This feature provides in -depth statistics about the applicants. 

api:*#3* 

This is prepared in web but no endpoints for app.


