**Module Name** - GAD 3 (Complaint MODULE) **Student Mentor** - Hardik Pratap Singh(21BCS090)

**API Documentation of GAD3 - Complaint Module Please mention all the APIs used in the module below**

1. **user/detail/complain\_id/** - Already implemented
   1. parameters: complaint id
   1. description: Get details of a particular complaint
1. **newcomplain/** - Already implemented
   1. Parameters: none
   1. Description: Lodge a new complaint
1. **studentcomplain/** - Already implemented
   1. Parameters: none
   1. Description: View complaints of the currently logged-in user
1. **updatecomplain/complain\_id/** - Already implemented
   1. Parameters: complaint id
   1. Description: update a particular complaint
1. **removecomplain/complain\_id** - Already implemented
   1. Parameters: complaint id
   1. Description: delete a particular complaint
1. **workers/** - Already implemented
   1. Parameters: none
   1. Description: get a list of workers
1. **addworker/ -** Already implemented
   1. Parameters: none
   1. Description: add a new worker
1. **removeworker/worker\_id** - Already implemented
   1. Parameters: worker id
   1. Description: delete a particular worker
1. **updateworker/worker\_id** - already implemented
1. Parameter: worker\_id
1. Description: update a particular worker’s details

10\.**caretakers/** - Already implemented

1. Parameter: none
1. Description: Get the list of caretakers

11\.**addcaretaker/** - Already implemented

1. Parameters: none
1. Description: add a new caretaker

12\.**removecaretaker/caretaker\_id**- Already implemented

1. Parameters: caretaker id
1. Description: remove a caretaker

13\.**updatecaretaker/caretaker\_id** - Already implemented

1. Parameters: caretaker id
1. Description: update a caretaker

14\.**supervisors/** - Already implemented

1. Parameters: none
1. Description: get a list of supervisors

15\.**addsupervisor/** - Already implemented

1. Parameters : none
1. Description : to add a new supervisor

16\.**removesupervisor/supervisor\_id** - Already implemented

1. Parameters: supervisor id
1. Description: remove a supervisor

**17.update supervisor/supervisor\_id -** Already implemented

1. Parameters: supervisor id
1. Description: update a particular supervisor

**Overview of the module:-** The central complaint system is designed to efficiently manage and resolve issues about electricity, hostels, and cleanliness in each campus building. The primary goal of this software is to provide a swift and effective mechanism for addressing concerns raised by individuals within the campus community, ensuring a seamless resolution process. Additionally, it serves as a communication platform, facilitating a direct connection between users and the relevant Caretaker/Supervisor for each department.

APIs:-

- **Already Implemented (**This means that API is already implemented and working as expected.**)**
- **Lodge\_Complaint**

  Lodge New Complaint

  API Index: 2

  Database - Complaint\_system\_studentcomplain

- **Track\_Status**

  Track Status of complain

  API Index : 1

  Database - Complain\_system\_studentcomplain

- **Response\_Complaint**

  Response the lodge Complain

  API Index: 4

  Database - Complain\_system\_studentcomplain

- **Change\_Status**

  Change status of lodge complaint ,after resolving the complaint

  API Index : 4

  Database - Complain\_system\_studentcomplain

- **View\_Complaint**

  View Lodge complaint

  API Index : 1,3

  Database - Complain\_system\_studentcomplain

- **Feedback**

  View Lodge complaint

  API Index : 4

  Database - Complain\_system\_studentcomplain

- **Yet to be implemented or Partially Working** (API is not implemented ) **Forward: Not Implemented**

Api has to develop from scratch using the API provided by FTS module Complaints can be forwarded to the admin by the caretaker

database - Complain\_system\_studentcomplain

**Current problems you are facing with the module or in its use cases —**

- Forward Complain Functionality

Google doc:[ API Status - GAD3](https://docs.google.com/document/d/1wd8fYVKhvaygebrva4bh33ZsFIuG8jmE6VmxOIk2biI/edit)
