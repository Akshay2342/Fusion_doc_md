Module Name-OS3\_NOTIFICATIONS\_WEB Student Mentor – SUDHANSHU PATIL (21BCS209) 

**API used in the module**  

There are no actual APIs implemented here in this module. 

Notifications are dispatched by invoking functions within the views of the notification module from various modules. Each module triggers the function by passing the necessary parameters, resulting in the delivery of the corresponding message. The URLs have been hard coded and requests are being rendered 

**Overview of the module:-**  

Notify the User about relevant events, such as interactions with their content and updates from others students and faculty. For every module there will be different type of notifications according to the unique needs and activities associated with each individual module. 

- View notification 
- Delete notification 
- Make announcement 
- Mark as read 
- Mark as unread 
1. In the **file tracking module**, upon sending a notification, the sender will receive an acknowledgment notification confirming that the file has been sent successfully. Simultaneously, the recipient will be notified that the file has been received. 

*def* file\_tracking\_notif(*sender*, *recipient*,*title*): ![](Aspose.Words.c4e022b5-3536-44a1-a5c5-67dfcf77ed19.001.png)    url='filetracking:inward'

`    `module='File Tracking'

`    `*sender* = *sender*

`    `*recipient* = *recipient*

`    `verb = *title*

`    `notify.send(*sender*=*sender*, *recipient*=*recipient*, *url*=url, *module*=module, *verb*=verb) 

This notification takes sender id and recipient id and title as parameters and 

   sends a notification using the notify.send function. The notification content is determined based on the type parameter, and it includes information about the sender, recipient, URL, and module.The above function was invoked within the file tracking module file, and it forwarded the arguments that the function needs to utilize in order to dispatch the notification. 

file\_tracking\_notif(*request*.user,receiver\_id,subject)![](Aspose.Words.c4e022b5-3536-44a1-a5c5-67dfcf77ed19.002.png)

`                `messages.success(*request*,'File sent successfully') 

2. The doctor appointment form within the **health center module** is not working, while the ambulance request function is operational, and ambulance requests are directed to the compounder. After submitting feedback, it is unclear who receives 

   the notifications. Following the argument passage, the function sends a specific message corresponding to the provided type. 

   *def* healthcare\_center\_notif(*sender*, *recipient*, *type*): ![](Aspose.Words.c4e022b5-3536-44a1-a5c5-67dfcf77ed19.003.png)

   `    `url='healthcenter:healthcenter'

   `    `module='Healthcare Center'

   `    `*sender* = *sender*

   `    `*recipient* = *recipient*

   `    `verb = '' 

   `    `if *type* == 'appoint': 

   `        `verb = "Your Appointment has been booked"

   `    `if *type* == 'amb\_request': 

   `        `verb = "Your Ambulance request has been placed"

   `    `if *type* == 'Presc': 

   `        `verb = "You have been prescribed some medicine"

   `    `if *type* == 'appoint\_req': 

   `        `verb = "You have a new appointment request"

   `    `if *type* == 'amb\_req': 

   `        `verb = "You have a new ambulance request"

   ` `notify.send(*sender*=*sender*, *recipient*=*recipient*, *url*=url, *module*=module, *verb*=verb) 

3. Notifications are not functioning in the **Visitors hostel module** due to its incomplete functionality. The form details are not being transmitted to the caretaker responsible for the visitors' hostel.  

*def* visitors\_hostel\_notif(*sender*, *recipient*, *type*): ![](Aspose.Words.c4e022b5-3536-44a1-a5c5-67dfcf77ed19.004.png)

`    `url='visitorhostel:visitorhostel'

`    `module="Visitor's Hostel"

`    `*sender* = *sender*

`    `*recipient* = *recipient*

`    `verb = '' 

`    `if *type* =='booking\_confirmation': 

`        `verb='Your booking has been confirmed '

`    `elif *type* =='booking\_cancellation\_request\_accepted': 

`        `verb='Your Booking Cancellation Request has been accepted '     elif *type* =='booking\_request': 

`        `verb='New Booking Request '

`    `elif *type* =='cancellation\_request\_placed': 

`        `verb='New Booking Cancellation Request '

`    `elif *type* =='booking\_forwarded': 

`        `verb='New Forwarded Booking Request '

`    `elif *type* =='booking\_rejected': 

`        `verb='Your Booking Request has been rejected '

`    `notify.send(*sender*=*sender*, *recipient*=*recipient*, *url*=url, *module*=module, *verb*=verb) 

visitors\_hostel\_notif(*request*.user, bd.intender, ![](Aspose.Words.c4e022b5-3536-44a1-a5c5-67dfcf77ed19.005.png)'booking\_confirmation') 

`        `return HttpResponseRedirect('/visitorhostel/')     else: 

`        `return HttpResponseRedirect('/visitorhostel/') 

4. Within the **Gymkhana module**, all notifications are operational, except for the club membership form, where the selection of the club is not functioning, rendering it inactive. The co-convener can send voting poll notifications to specific batches, event notifications to all batches, and session notifications to all batches within the gymkhana module. 

   The notifications mentioned earlier can be directed to either an individual or a group, such as the entire batch of 2021.** 

   **GYMKHANA\_VOTING** 

`  `*def* gymkhana\_voting(*sender*, *recipient*, *type*, *title*, *desc*): ![](Aspose.Words.c4e022b5-3536-44a1-a5c5-67dfcf77ed19.006.png)    url = 'gymkhana:gymkhana'

`    `module = 'Gymkhana Module'

`    `*sender* = *sender*

`    `*recipient* = *recipient*

`    `*title* = *title*

`    `*desc* = *desc* 

`    `verb = "" 

`    `if *type* == 'voting\_open': 

`        `verb = "Voting is open for {}".format(*title*) 

`    `notify.send(*sender*=*sender*, 

`                `*recipient*=*recipient*, 

`                `*url*=url,

`                `*module*=module,

`                `*verb*=verb,

`                `*description*=*desc* 

`                `) 

**GYMKHANA\_SESSION** 

`     `*def* gymkhana\_session(*sender*, *recipient*, *type*, *club*, *desc*, *venue*): ![](Aspose.Words.c4e022b5-3536-44a1-a5c5-67dfcf77ed19.007.png)    url = 'gymkhana:gymkhana'

`    `module = 'Gymkhana Module'

`    `sender = sender

`    `recipient = recipient

`    `desc = desc 

`    `verb = "" 

`    `if type == 'new\_session': 

`       `verb = "A session by {} Club will be organised in {}".format(club, venue)

`    `notify.send(*sender*=sender,

`                `*recipient*=recipient,                 *url*=url,

`                `*module*=module,

`                `*verb*=verb,

`                `*description*=desc 

`                `) 

**GYMKHANA\_SESSION** 

*def* gymkhana\_event(*sender*, *recipient*, *type*, *club*, *event\_name*, *desc*, ![](Aspose.Words.c4e022b5-3536-44a1-a5c5-67dfcf77ed19.008.png)*venue*): 

`    `url = 'gymkhana:gymkhana'

`    `module = 'Gymkhana Module'

`    `*sender* = *sender*

`    `*recipient* = *recipient*

`    `*desc* = *desc* 

`    `verb = "" 

`   `if type == 'new\_event': 

`   `verb = "{} event by {} Club will be organised in{}".format(event\_name,club,venue)

`    `notify.send(*sender*=sender,

`                `*recipient*=recipient,                 *url*=url,

`                `*module*=module,

`                `*verb*=verb,

`                `*description*=desc 

`    `) 

5. In the **research procedures module**, the patent form is not working, so it is currently non-functional in generating notifications. Similarly, within the other academic procedures module, both the leave module and assistant claimship module forms have notification functions defined, but they are not working. These are currently not active for generating notifications 
5. In the **complaint system module**, once a student submits a complaint, a notification will be forwarded to the designated caretaker assigned to handle that 

   specific complaint. 

7. Within the **mess module**, notifications will be accessible upon submission of feedback, requests for changes in the mess menu, and leave or vacation requests from the staff. Additionally, when a student is added to the mess committee, they will receive a notification informing them of their new role.  
7. In **Department module** the publication of an announcement by the department head, notifications will be sent to both the department's students and the head of the department. These notifications will be accessible in the announcements section. 

**mark-as-read-and-redirect/()/**  this URL marks a notification as read and redirects the user based on the notification's data.  

urlpatterns = [ ![](Aspose.Words.c4e022b5-3536-44a1-a5c5-67dfcf77ed19.009.png)

`        `pattern(*r*'^mark-as-read-and-redirect/(?P<slug>\d+)/$', views.mark\_as\_read\_and\_redirect, *name*='mark\_as\_read\_and\_redirect'),     ] + urlpatterns

The above URL uses make use of  the mark\_as\_read\_and\_redirect function 

If the notification is related to the "Complaint System" module, it redirects the user to a specific URL with additional parameters. Otherwise, it redirects the user to a general URL provided in the notification's data. 

*def* mark\_as\_read\_and\_redirect(*request*, *slug*=None): ![](Aspose.Words.c4e022b5-3536-44a1-a5c5-67dfcf77ed19.010.png)

`    `notification\_id = slug2id(*slug*) 

`    `notification = get\_object\_or\_404( 

`        `Notification, *recipient*=*request*.user, *id*=notification\_id)

`    `notification.mark\_as\_read()

`    `if(notification.data['module'] == 'Complaint System'):      

`        `complaint\_id=notification.description

`        `return HttpResponseRedirect(reverse(notification.data['url'],*kwargs*={'detailcomp\_id1 ':complaint\_id}))

`    `else: 

`        `return HttpResponseRedirect(reverse(notification.data['url'])) 

**Current problems you are facing with the module or in its use cases —** 

- **View notification**: Determining the recipient's credentials is proving challenging, making it somewhat difficult to verify the successful delivery of notifications. 
- **delete notification**: This Use Case is not currently implemented 

  https://docs.google.com/document/d/1RmU9u\_wzTndrFj0oJnj58qF9fVSRyhOK/edit? usp=sharing&ouid=102720302826588816157&rtpof=true&sd=true 
