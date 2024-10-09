# Module Name: SA2-Mess Management (WEB)  
**Student Mentor:** Himanshu Ranjan (21BCS101)

## API Overview

### Implemented APIs
1. **/mess/rebateApi** - Implemented
2. **/mess/menuApi** - Implemented
3. **/mess/monthlyBillApi** - Implemented
4. **/mess/messBillBaseApi** - Implemented
5. **/mess/updateSemDatesApi** - Implemented
6. **/mess/updateBillApi** - Implemented
7. **/mess/updateMonthlyBillApi** - Implemented
8. **/mess/feedbackApi** - Implemented
9. **/mess/specialRequestApi** - Implemented
10. **/mess/get_mess_students** - Implemented
11. **/mess/get_student_bill** - Implemented
12. **/mess/get_reg_records** - Implemented
13. **/mess/get_student_payment** - Implemented
14. **/mess/get_student_all_detail** - Implemented
15. **/mess/paymentsApi** - Implemented

### Not Implemented APIs
1. **/mess/registrationRequestApi** - Not implemented
2. **/mess/respondToRegistrationRequestApi** - Not implemented
3. **/mess/deregistrationRequestApi** - Not implemented

### Not Required APIs
1. **Mess Meetings Api** - Not required as no use case
2. **Mess Minutes Api** - Not required as no use case
3. **Non Veg Api** - Not required as no use case
4. **Non Veg Menu Api** - Not required as no use case
5. **Mess Info Api** - Implemented but not required as no use case

---

## Module Overview
The interface will enable students to:
- Register for the mess
- Login
- View the mess menu
- Respond to vacation food requests
- Apply for rebates
- Request special food
- Make payments
- Give feedback
- View announcements
- Request deregistration

This interface will help the mess caretaker and the mess warden to coordinate, control, and assist users in viewing past records and accessing all functionalities of the mess without needing to visit physically.

**Users of this module:**
- Registered students of the Institute (PDPM IIITDM Jabalpur)
- Mess Warden
- Mess Caretaker

**SRS Google Doc Link:** [Mess Management](https://docs.google.com/document/d/1B4MA1wB-32SvVVdqodzp35uOrVuWT9Qn1BXngnYD7l4/edit?pli=1)

---

## API Use Cases

### Already Implemented APIs
- **UC#1: View Menu** - [Uses Api **#2**]
  - Fetches menu data from the database.
  - **Database:** central_mess_menu table

- **UC#2: View Bill** - [Uses Api **#3**]
  - Students can view their monthly bill.
  - **Database:** central_mess_monthly_bill table

- **UC#3: View Payment History** - [Uses Api **#18**]
  - Students can view their payment history.
  - **Database:** central_mess_payments table

- **UC#4: Give Feedback** - [Uses Api **#11**]
  - Students can submit feedback, which is stored for future access.
  - **Database:** central_mess_feedback

- **UC#7: Apply for Rebate** - [Uses Api **#1**]
  - Students can fill the application form for rebates.
  - **Database:** central_mess_rebate table

- **UC#8: Special Food Requests** - [Uses Api **#12**]
  - Students can create special food requests.
  - **Database:** central_mess_special_request table

- **UC#9: View Feedback** - [Uses Api **#11**]
  - Mess Caretaker and Warden can view feedback from registered students.
  - **Database:** central_mess_feedback

- **UC#10: Update Menu** - [Uses Api **#2**]
  - Mess Caretaker can update the menu.
  - **Database:** central_mess_menu

- **UC#11: Respond to Rebate Request** - [Uses Api **#1**]
  - Mess Caretaker can update rebate requests.
  - **Database:** central_mess_rebate table

- **UC#12: Respond to Special Food Requests** - [Uses Api **#12**]
  - Caretaker can respond to special food requests made by students.
  - **Database:** central_mess_special_request table

- **UC#13: Update Semester Dates** - [Uses Api **#8**]
  - Mess Caretaker can update semester dates.
  - **Database:** central_mess_semdates table

- **UC#15: Manage Registration** - [Uses Api **#13, 17 & 15**]
  - Mess Caretaker and Warden can view the registration list and search for a particular student.
  - **Database:** central_mess_reg_records, central_mess_reg_main table

- **UC#16: Mess Activities** - [Uses Api **#4, #9, #10, #14**]
  - Mess Caretaker can update the base bill amount and bills for students.
  - **Database:** central_mess_monthly_bill, central_mess_billbase

### Yet to be Implemented or Partially Working
- **UC#6 & 7: Request for Registration/Deregistration** - [Uses Api **#5, 6 & 7**] - Not implemented
  - No feature is currently available for students.
  - **Database:** Students Data, Payments Data, Mess Data, Registration Data

---

## Current Problems
- Non-Veg APIs and some others, such as the mess info API and student mess committee API, need to be commented out. These were present in the old SRS but do not function well and are not included in the new SRS.

**Google Doc Link:** [API Documentation](https://docs.google.com/document/d/1uPguE5SrpJuu0UyrJPIlbXpUV0Kn3_GsGTjMSf7JNd4/edit)
