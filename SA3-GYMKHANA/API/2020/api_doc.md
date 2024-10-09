# SA-3 Gymkhana Module (Web) API Report Assignment – 02

### Mentor:  
**Vijaypal Singh Rathor**

### Team:  
- **Anurag Goswami** - 21BCS028 [MENTOR]  
- **Shobhit Kushwaha** - 21BCS194  
- **Rishabh Sharma** - 21BCS174  
- **Rohit Raj** - 21BCS178  
- **Rohan Parmar** - 21BCS176  
- **Pullivarthi Mahesh** - 21BCS168  

---

## Use Cases Left to Be Implemented According to Use Case Model

|   |   |
|---|---|
|   |   |
|   |   |
|   |   |
|   |   |
|   |   |
|   |   |
|   |   |

---

## Overview

**Fusion ERP** is an online web service portal that provides a centralized platform for accessing, collecting, and managing various services related to an institute's operations, especially concerning the student body. The services include: 
- Course Registration and Management 
- Mess Committee 
- Gymkhana 
- Examination 
- Hostel Management 
- Placement Cell 
- Primary Health Centre (PHC) 
- Other departments supporting student activities.

---

## Purpose of Gymkhana Web Module

The Gymkhana web module is part of the online web service portal responsible for the following:

1. Viewing details of all club activities, including their calendar, current coordinators, and members.
2. Submitting applications for new clubs and applying for membership in existing clubs through detailed forms.
3. Users (students and faculty) can view ongoing or upcoming club sessions and events.
4. Accessing public details related to current and previous club members.
5. Participating in elections and requesting nominations for club head figures.

---

## Scope of the Module Functionalities

- Hold Elections
- Ask for Nominations
- View Club Details
- View Member Records
- Form New Clubs
- Apply for Membership in Clubs
- Appoint Club Coordinators
- Allocate Budgets to Clubs
- Create and View Club Sessions and Events

### Actors:
- Dean
- Counsellor
- Convener
- Club Coordinator
- Student

---

## Use Case Diagram
![Use Case Diagram](./images/bn5qmxd4.png)

---

## API Status Report

### 1. **API:** [http://127.0.0.1:8000/gymkhana/api/voting_polls](http://127.0.0.1:8000/gymkhana/api/voting_polls)

- **Status:** Not working
- **Reasons:**
  - CSRF Token Failure.
  - CSRF Token not sent in request headers from the frontend.
  - Resource may be accessible only by superusers (club admins) or token expiry time may be too short.
- **Status Code:** 401 Unauthorized Access
![Status 401](./images/uerzfsgt.png)

---

### 2. **API:** [http://127.0.0.1:8000/gymkhana/api/new_club](http://127.0.0.1:8000/gymkhana/api/new_club)

- **Status:** Not working
- **Reasons:**
  - CSRF Token Failure.
  - CSRF Token not sent in request headers from the frontend.
  - Resource may be accessible only by superusers (club admins) or token expiry time may be too short.
- **Status Code:** 401 Unauthorized Access
![Status 401](./images/c0ove2d0.png)
![Status 401](./images/glc1r33d.png)

---

### 3. **API:** [http://127.0.0.1:8000/gymkhana/clubname](http://127.0.0.1:8000/gymkhana/clubname)

- **Status:** Not working
- **Reasons:**
  - CSRF Token Failure.
  - CSRF Token not sent in request headers from the frontend.
  - Resource may be accessible only by superusers (club admins) or token expiry time may be too short.
- **Status Code:** 401 Unauthorized Access
![Status 401](./images/ovm2fgwz.png)

---

### 4. **API:** [http://127.0.0.1:8000/gymkhana](http://127.0.0.1:8000/gymkhana)

- **Status:** Working
- **Status Code:** 200 Success
![Status 200](./images/t0bcowav.png)
![Status 200](./images/fr0knvyr.png)

---

### 5. **API:** [http://127.0.0.1:8000/gymkhana/delete_requests](http://127.0.0.1:8000/gymkhana/delete_requests)

- **Status:** Not working
- **Reasons:**
  - API Functions not implemented.
  - Code block handling the request is not implemented.
- **Status Code:** 404 Not Found
![Status 404](./images/ermw4drk.png)

---

### 6. **API:** [http://127.0.0.1:8000/gymkhana/form_avail](http://127.0.0.1:8000/gymkhana/form_avail)

- **Status:** Not working
- **Reasons:**
  - API Functions not implemented.
  - Code block handling the request is not implemented.
- **Status Code:** 404 Not Found
![Status 404](./images/exsiazff.png)
![Status 404](./images/qpch415a.png)

---

### 7. **API:** [http://127.0.0.1:8000/gymkhana/registration_form](http://127.0.0.1:8000/gymkhana/registration_form)

- **Status:** Not working
- **Status Code:** 500 Internal Server Error
- **Reasons:**
  - Database is empty; form requires fields like Coordinator & Coordinator Roll Numbers to be fetched from the database.
  - Cannot manually enter club details due to strict Primary Key Constraints.
![Status 500](./images/v2qc0lmz.png)

---

### 8. **API:** [http://127.0.0.1:8000/gymkhana/new_club](http://127.0.0.1:8000/gymkhana/new_club)

- **Status:** Not working
- **Status Code:** 500 Internal Server Error
- **Reasons:**
  - Database is empty; form requires fields like Coordinator & Coordinator Roll Numbers to be fetched from the database.
  - Cannot manually enter club details due to strict Primary Key Constraints.
![Status 500](./images/iw5qtyip.png)
![Status 500](./images/ux1oycaz.png)


9\. API - <u>http://127.0.0.1:8000/gymkhana/approve</u>

> Status – Cannot determine as of now
>
> Status Code – 500 Internal Server Error
>
> Reasons –
>
> 1\. Cannot check because we cannot apply for club registration as the
> form for club registration is not working.

<img src="./images/tgs4bdmi.png"
style="width:6.27806in;height:3.07153in" />

10\. API - <u>http://127.0.0.1:8000/gymkhana/reject</u>

> Status – Cannot determine as of now
>
> Status Code – 500 Internal Server Error
>
> Reasons –

<img src="./images/bxnfz1wh.png"
style="width:6.27861in;height:2.90555in" />

> 1\. Cannot check because we cannot apply for club registration as the
> form for club registration is not working.

11\. API -http://127.0.0.1:8000/gymkhana/new_session/

> Status – Not working

Reasons –

> 1\. API Functions not implemented
>
> 2\. Code block handling the particular request is not implemented.
>
> Status Code – 403 forbidden

<img src="./images/elqhdqt0.png"
style="width:6.25514in;height:2.00972in" /><img src="./images/mle5yywj.png"
style="width:6.25597in;height:2.01944in" />

12\. API -http://127.0.0.1:8000/gymkhana/new_session/

> Status – Not working

Reasons –

> 1\. API Functions not implemented
>
> 2\. Code block handling the particular request is not implemented.
>
> Status Code – 403 forbidden

<img src="./images/jeyonnuu.png"
style="width:6.25542in;height:2.05486in" /><img src="./images/5ne5czyc.png"
style="width:6.26347in;height:1.69444in" />

13\. API -http://127.0.0.1:8000/gymkhana/event_report/

> Status – Not working

Reasons –

> Status – Cannot determine as of now
>
> Status Code – 500 Internal Server Error

<img src="./images/ivmq121w.png"
style="width:6.34958in;height:1.83819in" /><img src="./images/chdxb4vf.png"
style="width:6.17931in;height:2.34028in" />

It is redirecting to gymkahana link …..

14\. API -http://127.0.0.1:8000/gymkhana/club_event_report/

> Status – Not working

Reasons –

> Status – Cannot determine as of now

<img src="./images/xufedrz5.png"
style="width:6.2368in;height:2.94347in" />

> Status Code – 500 Internal Server Error

It is redirecting to gymkahana link …..

15\. API -http://127.0.0.1:8000/gymkhana/change_head/

> Status – Not working

Reasons –

> 1\. API Functions not implemented
>
> 2.Code block handling the particular request is not implemented

<img src="./images/ym0wvtkj.png"
style="width:6.26375in;height:2.01944in" /><img src="./images/4ikot2zk.png"
style="width:6.21347in;height:1.77708in" />

16\.

API -http://127.0.0.1:8000/gymkhana/club_budget/

> Status – Not working

Reasons –

> Status – Cannot determine as of now
>
> Status Code – 500 Internal Server Error

<img src="./images/5h1cjwaj.png"
style="width:6.22694in;height:2.96736in" />

Function is created such that if request is not post then

It is redirecting to gymkahana link …..

17\. API -http://127.0.0.1:8000/gymkhana/club_event_report/

> Status – Not working

Reasons –

> Status – Cannot determine as of now
>
> Status Code – 500 Internal Server Error

<img src="./images/dgrfshsd.png"
style="width:6.26431in;height:1.86944in" /><img src="./images/5m1wlreb.png"
style="width:6.18958in;height:0.90764in" />

Function is created such that if request is not post then

It is redirecting to gymkahana link …..

18\. API -http://127.0.0.1:8000/gymkhana/club_event_report/

> Status – Not working

Reasons –

> Status – Cannot determine as of now
>
> Status Code – 500 Internal Server Error

<img src="./images/egyjjrry.png"
style="width:6.27542in;height:2.60555in" /><img src="./images/gqnporu1.png"
style="width:6.23972in;height:0.87847in" />

Function is created such that if request is not post then

It is redirecting to gymkahana link …..

19\. . API -http://127.0.0.1:8000/gymkhana/date_sessions/

> Status – working

Reasons –

<img src="./images/jpfqrprp.png"
style="width:6.2025in;height:0.91111in" />

> Status – Cannot determine as of now
>
> Status Code – 200 OK

20\. API -http://127.0.0.1:8000/gymkhana/delete_evenets/

> Status – Not working

Reasons –

> Status – Cannot determine as of now
>
> Status Code – 500 Internal Server Error

<img src="./images/wjtlddjw.png"
style="width:6.23583in;height:2.28333in" /><img src="./images/c1v3yn3s.png"
style="width:6.25056in;height:1.48958in" />

21.21.

<img src="./images/ggjau0ev.png"
style="width:6.26736in;height:3.525in" />

API :- http://127.0.0.1:8000/gymkhana/delete_events/

Status – Not working

Reasons –

> Status – Cannot determine as of now
>
> Status Code – 500 Internal Server Error

22:

<img src="./images/cvayancn.png"
style="width:6.26736in;height:3.52486in" />

API :- <u>http://127.0.0.1:8000/gymkhana/edit_event/</u>

> Status – Not working

Reasons –

> Status – Cannot determine as of now
>
> Status Code – 404 Not Found

23\.

<img src="./images/2kokebnu.png"
style="width:6.19028in;height:3.89556in" />

API -
<u>http://127.0.0.1:8000/gymkhana/ismzktaj9lojd3n3iikjhlkxki54wfn7/editsession/</u>

> Status – Not working

Reasons –

> Status – Cannot determine as of now
>
> Status Code – 404 Not Found

24:-

<img src="./images/ydhgqnk4.png"
style="width:6.23889in;height:2.83305in" />

API - http://127.0.0.1:8000/gymkhana/delete_membeífoím/

> Status – Not working

Reasons –

CSRF Token expires as soon as we login and does not provide
authorization

> Status Code – 403 forbidden

25\.

<img src="./images/luyksdg1.png"
style="width:6.23333in;height:3.42472in" />

API:- http://127.0.0.1:8000/gymkhana/voting_poll/

Status – Not working Reasons –

CSRF verification failed. Request aborted

CSRF Token expires as soon as we login and does not provide
authorization

Status Code – 403 forbidden

26\.

<img src="./images/phc4ac0i.png"
style="width:6.20972in;height:2.54569in" />

API :- http://127.0.0.1:8000/gymkhana/delete_poll/ Status – Not working

Reasons –

API Functions not implemented

Status Code – 404 Page Not Found

27\.

<img src="./images/2fa04kzi.png"
style="width:6.27986in;height:2.78264in" />

API - http://127.0.0.1:8000/gymkhana/íegistíation_foím/ Status – Not
working

> Reasons –
>
> Authentication credentials were not provided. Status Code – 401
> Unauthorized access

28\.

API:- http://127.0.0.1:8000/gymkhana/delete_íequests/

<img src="./images/13pglvd1.png"
style="width:6.25778in;height:2.35694in" />

Status – Not working Reasons –

CSRF verification failed. Request aborted Status Code – 403 forbidden

29\.

API :- http://127.0.0.1:8000/gymkhana/club_membeíship/

<img src="./images/yl23ifru.png"
style="width:6.21597in;height:3.15389in" />

Status – Not working Reasons –

CSRF verification failed. Request aborted

CSRF Token expires as soon as we login and does not provide
authorization

Status Code – 403 forbidden

30\.

API :- http://127.0.0.1:8000/gymkhana/session_details

<img src="./images/wmmu5y1q.png"
style="width:6.26667in;height:3.52486in" />

Status – Not working Reasons –

CSRF verification failed. Request aborted

CSRF Token expires as soon as we login and does not provide
authorization

Status Code – 401 Unauthorized

31\.

<img src="./images/i45frxco.png"
style="width:6.26667in;height:3.52486in" />

API :- http://127.0.0.1:8000/gymkhana/event_info

Status – Not working Reasons –

CSRF verification failed. Request aborted

Request not hitting the controllers and aborting from views

Status Code – 401 Unauthorized

32\.

<img src="./images/2krznbgr.png"
style="width:6.26667in;height:3.52458in" />

API :- http://127.0.0.1:8000/gymkhana/club_budgetinfo

Status – Not working Reasons –

CSRF verification failed. Request aborted

Request not hitting the controllers and aborting from views

Status Code – 401 Unauthorized

33\.

<img src="./images/ylz3n1sy.png"
style="width:6.26805in;height:3.52486in" />

API :- http://127.0.0.1:8000/gymkhana/club_appíove

Status – Working Status Code – 200

34\.

<img src="./images/5rdlhfzs.png"
style="width:6.26805in;height:3.52486in" />

API :- http://127.0.0.1:8000/gymkhana/club_íeject

Status – Working Status Code – 200

35\.

API :- http://127.0.0.1:8000/gymkhana/api/login

Status – Not working Reasons –

CSRF verification failed. Request aborted TTL is only 600ms

<img src="./images/h43v0ijn.png"
style="width:6.26667in;height:3.52486in" />Status Code – 401
Unauthorized

36\.

API :- http://127.0.0.1:8000/gymkhana/api/clubdetails

Status – Not working Reasons –

CSRF verification failed. Request aborted TTL is only 600ms

<img src="./images/obnahc1a.png"
style="width:6.13736in;height:3.45139in" />Status Code – 401
Unauthorized

<img src="./images/5jnflqfr.png"
style="width:6.26736in;height:3.52472in" />

37\. API :- http://127.0.0.1:8000/gymkhana/api/Fest_budget

> Status – Not working Reasons –
>
> CSRF verification failed. Request aborted TTL is only 600ms
>
> Status Code – 401 Unauthorized

38\. API :-http://127.0.0.1:8000/gymkhana/api/club_íepoít

Status – Not working Reasons –

CSRF verification failed. Request aborted TTL is only 600ms

<img src="./images/ymnubtal.png"
style="width:6.26667in;height:3.52486in" />Status Code – 401
Unauthorized

39\. API :-http://127.0.0.1:8000/gymkhana/api/íegisteíation_foím

Status – Not working Reasons –

Api not hitting the controllers .As shown in vs code terminal “test” is
not being printed.

<img src="./images/bib0bpxw.png"
style="width:6.26667in;height:3.52486in" />Status Code – 401
Unauthorized

<img src="./images/uoe3gja0.png"
style="width:6.26555in;height:3.52431in" />

40\. API - http://localhost:8000/gymkhana/club_membership/

> Status – Not working
>
> Reasons –
>
> 1\. API Functions not implemented
>
> 2\. Code block handling the particular request is not implemented.
>
> <img src="./images/eqz0fxr4.png"
> style="width:6.26555in;height:3.41458in" /><img src="./images/ajku23tv.png"
> style="width:6.26667in;height:3.52486in" />Status Code – 403 Forbidden

41\. API - http://localhost:8000/gymkhana/faculty_data/

> Status – Not working
>
> Reasons -
>
> 1\. Missing key request. 2. Incorrect key name.
>
> <img src="./images/1dhgad5l.png"
> style="width:5.81806in;height:3.16944in" /><img src="./images/e2dkqa21.png"
> style="width:6.2625in;height:3.52958in" />Status Code – 500 Internal
> Server Error

42\. API - http://localhost:8000/gymkhana/faculty_data/

> Status – Not working
>
> Reasons –
>
> 1\. API Functions not implemented
>
> 2\. Code block handling the particular request is not implemented. 3.
> Missing key request.
>
> <img src="./images/2kjhda40.png"
> style="width:6.25972in;height:3.39986in" /><img src="./images/4uh3irmh.png"
> style="width:6.26667in;height:3.52486in" />Status Code – 403 Forbidden

43\. API - http://localhost:8000/gymkhana/get_venue/

> Status – Not working
>
> Reasons –
>
> 1\. There is a typo in the attribute or method name, or if the code
> assumes the existence of an attribute that hasn't been initialized or
> provided.
>
> 2\. If the structure of an object is expected to remain constant, but
> it dynamically changes during runtime

<img src="./images/fq22hhlp.png"
style="width:5.27167in;height:2.86944in" /><img src="./images/guvdioeg.png"
style="width:6.13736in;height:3.45139in" />Status Code – 403 Forbidden

44\. API - http:localhost:8000/gymkhana/core_team/

> Status – Not working
>
> Reasons –
>
> 1\. CSRFTokenFailure.
>
> 2\. The CSRF Token is not sent in the request headers from the
> frontend while making the request.
>
> 3\. Either the resource is only accessible by superusers (club admins)
> or the expiry time of token is very less.

<img src="./images/i1xda1uf.png"
style="width:6.26667in;height:3.52486in" />Status Code – 403 Forbidden

45\. API - http:localhost:8000/gymkhana/festbudget/

> Status – Not working
>
> Reasons –
>
> 1\. CSRFTokenFailure.
>
> 2\. The CSRF Token is not sent in the request headers from the
> frontend while making the request.
>
> 3\. Either the resource is only accessible by superusers (club admins)
> or the expiry time of token is very less.
>
> 4\. Database is empty.

<img src="./images/c3v4nqzl.png"
style="width:6.26667in;height:3.52472in" />Status Code – 403 Forbidden

46\. API - <u>http://localhost:8000/gymkhana/?P\<poll_id</u>\> Status –
Not working

> Reasons –
>
> 1\. Insufficient data to check this api. 2. Database is empty

Status Code – Can’t determine
