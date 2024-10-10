**Module Name** – GAD – 5  (DASHBOARD MODULE)  **Student Mentor** – Pranjal Jha  (21BCS161)

**API Documentation of GAD-5  - DASHBOARD Module** 

**Overview of the module:-** 

The purpose of the project entitled as DASHBOARD is to provide an intuitive and efficient platform for different user roles to access and manage their profiles, navigate to specific modules, and receive notifications from various departments.  

- Access Dashboard.  
- View Profile. 
- Navigate to Modules
- View Administrative Profile. 
- Receive Notifications. **APIs in the module** 
1. /accounts/login/- Already implemented 
   1. Parameters required – login , password 
   1. Description - Login takes {login and password }as parameters and returns the details of the user for the dashboard. 
1. /notifications/api/unread\_list – Yet to be implemented  
1. /accounts/logout/ - Already implemented 
1. Parameters required - csrfmiddlewaretoken 
1. Description - Logout takes {csrfmiddlewaretoken}  as parameters and redirect to the login page . 

APIs:- 

- **Already Implemented (**This means that API is already implemented and working as expected.**)** 
- *login -  UC#1* 
- Index of api’s used -  1 
- Description - Login takes {login and password }as parameters and returns the details of the user for the dashboard. 
- Database – auth\_user,globals\_designation 
- *logout -  UC#3* 
- Index of api’s used -  3 
- Description - Logout takes {csrfmiddlewaretoken}  as parameters and redirect to the login page. 
- Database – auth\_user 
- **Yet to be implemented or Partially Working** (API is not implemented so yet to be implemented or API is partially working i.e it has breakage.)** 
- *notification -  UC#2* 
- Index of api’s used -  2 
- Description -Function of this endpoint to fetch all the notification s across all the modules and show in the dashboard. 
- Database – Yet to be decide 

**Current problems you are facing with the module or in its use cases —** 

- NA 

**APIs in the mobile module** 

1\. /api/auth/login/- Already implemented 

1. Parameters required – login , password 
1. Description - Login takes {login and password }as parameters and returns the details of the user for the dashboard. 

2\.notification api – Yet to be implemented  3.api/auth/logout/ - Already implemented 

1. Parameters required -  
1. Description - Logout takes { }  as parameters and redirect to the login 

page . 

4\.api/dashboard / - Already implemented 

1. Parameters required – userId 
1. Description – Getting info about position, designation of the user based 

on which other functionality will run  

APIs:- 

- **Already Implemented (**This means that API is already implemented and working as expected.**)** 
- *login -  UC#1* 
- Index of api’s used -  1 
- Description - Login takes {login and password }as parameters and returns the details of the user for the dashboard. 
- Database – auth\_user 
- *logout -  UC#3* 
- Index of api’s used -  3 
- Description - Logout takes { }  as parameters and redirect to the login page. 
- Database – auth\_user 
- *dashboard -  UC#4* 
- Index of api’s used -  4 
- Description - Getting info about position, designation of the user based on which other functionality will run. 
- Database – auth\_users, globals\_designation 
- **Yet to be implemented or Partially Working** (API is not implemented so yet to be implemented or API is partially working i.e it has breakage.)** 
- *notification -  UC#2* 
- Index of api’s used -  2 
- Description -Function of this endpoint to fetch all the notification s across all the modules and show in the dashboard. 
- Database – Yet to be decide 

**Current problems you are facing with the module or in its use cases —** 

- NA 

Google Drive Link - https://docs.google.com/document/d/1REn6oT77pC3- fXn0PJB\_IPOolEfzNZOyXYULqSnxq-Y/edit?addon\_store 
