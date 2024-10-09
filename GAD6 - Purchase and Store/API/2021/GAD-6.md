# **API Documentation of GAD-6 - Purchase and Store Module**

**Module Name**: GAD-6 (Purchase and Store)  
**Student Mentor**: Siddharth Tandon (21BCS200)

---

## **Overview of the Module**

This module can be used to file an indent by faculty/staff members, get the indent approved by authorities, manage stocks, and ensure a transparent system to keep track of the application status and payments involved.

An indenter is allowed to:
- Fill indent form(s)
- Get the form approved by concerned authorities (Director/Registrar)
- Initiate procurement
- Track delivery and make stock entries
- Follow the payment process for items received

---

## **APIs Used in the Module**

### 1. **Create Proposal**
- **Endpoint**: `purchase-and-store/create_proposal/request{usertype,data}` 
- **Parameters Required**: `usertype`, `data`
- **Description**:  
  Allows the employee to file an indent (create a proposal) by filling out an online form.

### 2. **Forward Request**
- **Endpoint**: `purchase-and-store/forward_request/request{usertype,data}`
- **Parameters Required**: `usertype`, `data`
- **Description**:  
  The department/section head, director, or registrar can approve and forward the indent received from their section.

### 3. **View Stock**
- **Endpoint**: `purchase-and-store/view_stock/{usertype}`
- **Parameters Required**: `usertype`
- **Description**:  
  The PS_admin or Department admin can view the stocks available in the stock maintenance system.
- **Status**: Implemented

### 4. **Add Stock**
- **Endpoint**: `purchase-and-store/add_stock/request{usertype,data}`
- **Parameters Required**: `usertype`, `data`
- **Description**:  
  The PS_admin or Department admin can add, modify, and/or delete stock information from the system.

### 5. **Generate Report**
- **Endpoint**: `purchase-and-store/generate_report/{usertype}`
- **Parameters Required**: `usertype`
- **Description**:  
  The PS_admin can view reports of all departments after stock updates, and the Department admin can view reports of their respective departments.

### 6. **Perform Transfer**
- **Endpoint**: `purchase-and-store/perform_transfer/request{usertype,data}`
- **Parameters Required**: `usertype`, `data`
- **Description**:  
  The PS_admin can transfer items to other departments, and the Department admin can transfer items to other departments or the Global administrator.

### 7. **View Transfer Execution**
- **Endpoint**: `purchase-and-store/view_transfer_execution/{usertype}`
- **Parameters Required**: `usertype`
- **Description**:  
  The PS_admin and Department admin can view data on the items/stocks that have been transferred.

---

## **APIs Status**

### **Implemented**

- **View Global Stock**
  - **Endpoint**: `purchase-and-store/stock_view/`
  - **Description**:  
    Allows the PS_admin to view the stocks available in the stock maintenance system.
  - **Database**:  
    The table `StockEntry` contains the stock details to be fetched for this transaction.

### **Partially Working or Not Implemented**

- **Add Global Stock**
  - **Endpoint**: `purchase-and-store/entry/`
  - **Description**:  
    Allows the PS_admin to add, modify, or delete stock information. Currently, the page redirects to a blank form.
  - **Expected Work**:  
    A form needs to be added with necessary fields to handle stock addition, modification, and deletion.
  - **Database**:  
    The table `StockEntry` will be used to populate the stocks.

- **Generate Global Report**
  - **Endpoint**: `purchase-and-store/generate_report/`
  - **Description**:  
    Allows the PS_admin to view reports of all departments. Currently not implemented.
  - **Expected Work**:  
    The endpoint should redirect to a page that displays report data fetched from the database after stock updates.
  - **Database**: No table implemented yet.

- **Perform Global Transfer**
  - **Endpoint**: `purchase-and-store/perform_transfer/`
  - **Description**:  
    Allows the PS_admin to transfer items between departments. Not yet implemented.
  - **Expected Work**:  
    The endpoint should provide an option to transfer items to other departments.
  - **Database**: No table implemented yet.

- **View Global Transfer Execution**
  - **Endpoint**: `purchase-and-store/view_transfer_execution/`
  - **Description**:  
    Allows the PS_admin to view transferred data. Not yet implemented.
  - **Expected Work**:  
    The endpoint should display the transfer report.
  - **Database**: No table implemented yet.

- **View Department Stock**
  - **Endpoint**: `purchase-and-store/view_stock/`
  - **Description**:  
    Allows the Department admin to view the department's available stocks. Not yet implemented.
  - **Expected Work**:  
    The endpoint should display the stock details of the department.
  - **Database**: The table `StockEntry` will be used for fetching department-specific stock details.

- **Add Department Stock**
  - **Endpoint**: `purchase-and-store/add_stock/`
  - **Description**:  
    Allows the Department admin to add, modify, or delete stock information. Not yet implemented.
  - **Expected Work**:  
    A form needs to be added for adding, modifying, and deleting stock entries.
  - **Database**: The table `StockEntry` will be used to populate department stocks.

- **Generate Department Report**
  - **Endpoint**: `purchase-and-store/generate_report/`
  - **Description**:  
    Allows the Department admin to generate reports after stock updates. Not yet implemented.
  - **Expected Work**:  
    The endpoint should redirect to a page containing department-specific stock update reports.
  - **Database**: No table implemented yet.

- **Perform Department Transfer**
  - **Endpoint**: `purchase-and-store/perform_transfer/`
  - **Description**:  
    Allows the Department admin to transfer items to other departments or the Global/PS admin. Not yet implemented.
  - **Expected Work**:  
    The endpoint should provide an option to transfer items.
  - **Database**: No table implemented yet.

- **View Department Transfer Execution**
  - **Endpoint**: `purchase-and-store/view_transfer_execution/`
  - **Description**:  
    Allows the Department admin to view transferred data between their department and others or the Global administration. Not yet implemented.
  - **Expected Work**:  
    The endpoint should display the transfer report.
  - **Database**: No table implemented yet.

- **Create Proposal**
  - **Endpoint**: `purchase-and-store/create_proposal/`
  - **Description**:  
    Allows the employee to file an indent or order request. Not yet implemented.
  - **Expected Work**:  
    The endpoint should provide a form to file an indent.
  - **Database**: The table `IndentFile` will store the filled indent data.

- **Approve/Forward Request**
  - **Endpoint**: `purchase-and-store/forward_request/`
  - **Description**:  
    Allows department heads, directors, or registrars to approve and forward the indent. Not yet implemented.
  - **Expected Work**:  
    The endpoint should display a list of received indents with options to approve and forward them.
  - **Database**: No table implemented yet.

---

## **Current Challenges**

- Clarification is needed on the role of the **Actor account_admin** and its use cases.
- The implemented APIs lack access control, allowing unauthorized access to the system.

---

**[Use Case Diagram](https://drive.google.com/file/d/1hbWGh6hf8qkIzrVlXZDLc7BT9KapfEDQ/view?usp=drive_link)**

**[Google Docs Link](https://docs.google.com/document/d/1XbOH0XzkTrZFO-KTzb5t9N-6XS5hHZzSvnJXoFVtgcE/edit?usp=sharing)**
