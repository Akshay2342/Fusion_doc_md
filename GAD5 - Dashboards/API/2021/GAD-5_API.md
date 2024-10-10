# Module Name – GAD – 5 (DASHBOARD MODULE)
**Student Mentor** – Pranjal Jha (21BCS161)

## API Documentation of GAD-5 - DASHBOARD Module

### Overview of the module

The purpose of the project entitled as DASHBOARD is to provide an intuitive and efficient platform for different user roles to access and manage their profiles, navigate to specific modules, and receive notifications from various departments.  

- Access Dashboard  
- View Profile  
- Navigate to Modules  
- View Administrative Profile  
- Receive Notifications  

### APIs in the module

1. **/accounts/login/** - Already implemented  
   - **Parameters required** – login, password  
   - **Description** - Login takes `{login and password}` as parameters and returns the details of the user for the dashboard.  

2. **/notifications/api/unread_list** – Yet to be implemented  

3. **/accounts/logout/** - Already implemented  
   - **Parameters required** - csrfmiddlewaretoken  
   - **Description** - Logout takes `{csrfmiddlewaretoken}` as parameters and redirects to the login page.  

### APIs

#### Already Implemented 
*(This means that API is already implemented and working as expected.)* 

- **login - UC#1**  
  - **Index of APIs used** - 1  
  - **Description** - Login takes `{login and password}` as parameters and returns the details of the user for the dashboard.  
  - **Database** – auth_user, globals_designation  

- **logout - UC#3**  
  - **Index of APIs used** - 3  
  - **Description** - Logout takes `{csrfmiddlewaretoken}` as parameters and redirects to the login page.  
  - **Database** – auth_user  

#### Yet to be implemented or Partially Working
*(API is not implemented so yet to be implemented or API is partially working i.e., it has breakage.)* 

- **notification - UC#2**  
  - **Index of APIs used** - 2  
  - **Description** - Function of this endpoint to fetch all the notifications across all the modules and show in the dashboard.  
  - **Database** – Yet to be decided  

### Current Problems You Are Facing with the Module or in Its Use Cases 

- NA  

## APIs in the Mobile Module

1. **/api/auth/login/** - Already implemented  
   - **Parameters required** – login, password  
   - **Description** - Login takes `{login and password}` as parameters and returns the details of the user for the dashboard.  

2. **notification api** – Yet to be implemented  

3. **/api/auth/logout/** - Already implemented  
   - **Parameters required** -  
   - **Description** - Logout takes `{}` as parameters and redirects to the login page.  

4. **/api/dashboard/** - Already implemented  
   - **Parameters required** – userId  
   - **Description** - Getting info about position, designation of the user based on which other functionality will run.  

### APIs

#### Already Implemented 
*(This means that API is already implemented and working as expected.)* 

- **login - UC#1**  
  - **Index of APIs used** - 1  
  - **Description** - Login takes `{login and password}` as parameters and returns the details of the user for the dashboard.  
  - **Database** – auth_user  

- **logout - UC#3**  
  - **Index of APIs used** - 3  
  - **Description** - Logout takes `{}` as parameters and redirects to the login page.  
  - **Database** – auth_user  

- **dashboard - UC#4**  
  - **Index of APIs used** - 4  
  - **Description** - Getting info about position, designation of the user based on which other functionality will run.  
  - **Database** – auth_users, globals_designation  

#### Yet to be implemented or Partially Working
*(API is not implemented so yet to be implemented or API is partially working i.e., it has breakage.)* 

- **notification - UC#2**  
  - **Index of APIs used** - 2  
  - **Description** - Function of this endpoint to fetch all the notifications across all the modules and show in the dashboard.  
  - **Database** – Yet to be decided  

### Current Problems You Are Facing with the Module or in Its Use Cases 

- NA  

### Google Drive Link
[Google Drive Link](https://docs.google.com/document/d/1REn6oT77pC3-fXn0PJB_IPOolEfzNZOyXYULqSnxq-Y/edit?addon_store)
