# **Module Name - Purchase and Store**

**Faculty Mentor**: Dr. Durgesh Singh  
**Student Mentor**: Mr. Siddharth Tandon (21BCS200)

---

## **Database Documentation of [GAD-6 - Purchase and Store] 4.0**

---

### **Overview of the Module**

- **SRS**:  
  [SRS Link](https://drive.google.com/file/d/1o6GN8lzYsG22QPhQidlkZKFLqLaAhQfI/view?usp=drive_link)

---

### **A. ER Diagram**  
Created using draw.io  
[ER Diagram](https://drive.google.com/file/d/18lrA4hUj913Ir9QdB24UWXG6D52zA3ud/view)

---

### **B. Database Schema Info**  
Available in the Google Sheet:  
[Database Schema for GAD-6](https://docs.google.com/spreadsheets/d/136ha-y73jrIciTNwYA5yw1uNdJs1ipKx6vcQ6c9le_4/edit?usp=sharing)

---

### **C. Changes Required in the Currently Implemented Tables**
These changes will be applied in version 4.0.

1. **StockEntry Table**
   - **dept**
     - **Change**: This attribute needs to be added.
     - **Justification**:  
       This attribute will help identify the department/section to which the stock belongs. It will assist in the following API functions:
       - `view_global_stock`
       - `add_global_stock`
       - `perform_global_transfer`
       - `view_global_transfer_execution`
       - `view_dept_stock`
       - `add_dept_stock`
       - `perform_dept_transfer`
       - `view_dept_transfer_execution`

   - **to_dept**
     - **Change**: This attribute needs to be added.
     - **Justification**:  
       This will help identify the department/section to which the stock belonged before the stock transfer. It will assist in:
       - `perform_global_transfer`
       - `view_global_transfer_execution`
       - `perform_dept_transfer`
       - `view_dept_transfer_execution`

   - **transfer**
     - **Change**: This attribute needs to be added.
     - **Justification**:  
       This attribute will help identify whether the stock has been transferred or not. It will assist in:
       - `perform_global_transfer`
       - `view_global_transfer_execution`
       - `perform_dept_transfer`
       - `view_dept_transfer_execution`

2. **IndentFile Table**
   - **department**
     - **Change**: This attribute needs to be added.
     - **Justification**:  
       The `IndentFile` should have an attribute to identify the department/section to which the indent belongs. This will allow the indent to be forwarded to the next actor for approval or rejection.

---

### **D. Data Availability for API and Functional Testing**

#### **D.1. Mention the Tables That Are Already Populated**
- No specific tables mentioned as already populated.

#### **D.2. Mention the Tables Required to Be Populated**
- **IndentFile**
- **StockEntry**

#### **D.3. Mention Any Difficulties Faced by Your Team Regarding Populating Any Table (if any)**
- No specific difficulties mentioned yet.

