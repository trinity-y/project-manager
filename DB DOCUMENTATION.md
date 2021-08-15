# **DB DOCUMENTATION**

### **key description:**

1. all keys will start with a prefix indicating the type of info:<br/>
   - task
   - meeting
   - serverInfo 
2. this prefix will then be followed by the server ID, so tasks stay in each server.
3. then, the key will be followed by an item number.
   - EXCEPTION: serverInfo, which will have no item number



**example:**

task598743951, with task being the prefix, 59874395 being the serverID, and 1 being the task #.



### **value description:**

***\*task:\**** tasktitle, taskdesc, duedate, and person all separated by commas

   e.g: task598743951 = task 1,do the task,2021-08-13,person#1234



***\*meeting:\**** meetingtitle, meetinglink, meetingdate, person all sepearated by commas

   e.g: meeting598743951 = meeting 1,google.ca,2021-08-13,person#1234



***\*serverinfo:\**** no. of tasks followed by the no. of meetings, separated by a comma.

​	e.g: serverInfo59874395  = 0,0