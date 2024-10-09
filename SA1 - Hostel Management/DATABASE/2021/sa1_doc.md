# Fusion ERP

## Database Documentation of  
### SA1 - Hostel Management 4.0

---

### Module Name: SA-1_Hostel Management
**Faculty Mentor:** Dr. Vijaypal Singh Rathor  
**Student Mentor:** Deven Nehete (21BCS144)

---

## Overview of the Module

The **Hostel Management module** is an integral part of our project, catering to students, caretakers, and wardens.  

For **students**, it offers streamlined functionalities like:
- Requesting guest rooms
- Managing allotted rooms
- Registering complaints
- Accessing notices

**Caretakers** can efficiently handle tasks such as:
- Approving leave
- Managing inventory
- Overseeing student-related information

**Wardens** have central oversight, managing:
- Guard shifts
- Notice boards
- Room assignments
- Generating relevant reports

The module aims to enhance hostel administration by providing role-specific features, fostering efficient communication, and simplifying various management tasks. The implementation includes secure API endpoints to ensure a user-friendly and organized hostel management system.

**Main Actors:**  
- Student  
- Warden  
- Caretaker  
- Super Admin  

---

### Important Links

- **SRS Document:** [View SRS](https://docs.google.com/document/d/1A61b0hwB2ZueUbpyadJo38HNc4TSlm5bdOkrjfIgtSI/edit)  
- **ER Diagram:** [View ER Diagram](https://drive.google.com/file/d/15236s9zFE6XwPiCxfUev5SNTsXuIPvRp/view?usp=drive_link)  
- **Database Schema Info:** [View Schema](https://docs.google.com/spreadsheets/d/1lEYs4ftbAvHYfYuI432x-bnjfoBrlhCy/edit?usp=drive_link&ouid=109045340837729900356&rtpof=true&sd=true)  

---

### Changes Required in the Current Database Tables

1. **`hallroom` Table**
   - **Roll No.**  
     - **Change:** Add a new column for roll number  
     - **Justification:** A new table `studentinfo` has been added to fetch data regarding the student’s hostel and room allotment.
   - **Student Name**  
     - **Change:** Add a new column for student name  
     - **Justification:** Fetch data for the `studentinfo` table.

2. **`hostelallotment` Table**
   - **Assigned Caretaker**  
     - **Change:** Add a new column for assigned caretaker  
     - **Justification:** A new use case `manageCaretaker` has been introduced.
   - **Assigned Warden**  
     - **Change:** Add a new column for assigned warden  
     - **Justification:** A new use case `manageWarden` has been introduced.

---

## Data Availability for API and Functional Testing

### D.1 Tables Already Populated:
- `hallroom`
- `hall`
- `hallcaretaker`
- `Staffschedule`
- `Hostelnoticeboard`
- `workerReport`

### D.2 Tables Required to be Populated:
- `GuestRoomBooking`
- `hallwarden`
- `guestroomdetails`
- `Studentattendance`
- `RegisterComplaint`
- `Hostelfines`
- `Hostelleave`
- `Hostelinventory`
- `Studentinfo`
- `Guardshift`

---

## Team Members

- **21BCS144 -** Deven Nehete (Lead)  
- **21BCS123 -** Mahadevu Sai Ravi Kishor Naidu  
- **21BCS138 -** Saurabh Nagpure  
- **21BCS165 -** Priya Murmu  
- **21BCS198 -** Shuvam Patra  
- **21BCS221 -** Jyotsna Telgote
