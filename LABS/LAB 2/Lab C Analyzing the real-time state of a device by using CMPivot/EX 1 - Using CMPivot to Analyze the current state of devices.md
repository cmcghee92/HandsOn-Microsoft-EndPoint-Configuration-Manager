Scenario

Your security manager needs to know the machines on which a specific user is listed as a local administrator. You decide to use CMPivot to analyze and determine the results. You are also having issues with some of your client computers and need to determine which services are in a stopped state. You will use CMPivot to determine the results for these issues also.

Exercise 1: Using CMPivot to Analyze the current state of devices
Scenario

You need to use CMPivot to find the user who is listed as the local administrator for all the client computers in the collection. You also need to run a CMPivot query to identify the services that are stopped, and then determine the results.

The main tasks for this exercise are as follows:

Create a CMPivot query to analyze local administrative users.
Create a collection based on the CMPivot query results.
Create a user on LON-CL1.
Rerun the CMPivot query to analyze local administrative users.
Export the CMPivot query results to a CSV file.
Run a CMPivot query to identify stopped services.
Prepare for the next module.
Task 1: Create a CMPivot query to analyze local administrative users
On LON-CFG, if the Configuration Manager console is not already open, on the taskbar, click the Configuration Manager Console icon.

Click the Asset and Compliance workspace, and then click Device Collections.

In the center panel, right-click All Desktop and Server Clients, and then click Start CMPivot.

In the CMPivot (All Desktop and Server Clients) window, click the Query tab.

On the Query tab, in the text box, type Administrators.

Click the Run Query button.

Review the results.

Task 2: Create a collection based on the CMPivot query results
In CMPivot, select the Query Summary tab.

Next to the Offline row, click 1.

In the Offline Devices window, make a note of the reason for the failure.

Click Create Collection.

In the Create Device Collection Wizard, on the General page, in the Name box, type Test collection using CMPivot query.

Click Next.

On the Membership Rules page, clear the Schedule a full update on this collection check box.

Click Summary.

On the Summary page, click Next.

On the Completed page, click Close.

Close the CMPivot (All Desktop and Server Clients) window.

Task 3: Create a user on LON-CL1
Switch to LON-CL1 and send the CTRL+ALT+DEL command and log in as ADATUM\AdatumAdmin with the password Pa55w.rd.

On LON-CL1, click Start and then type Computer Management.

Click Computer Management.

In the Computer Management window, expand Local Users and Groups.

Right-click Users, and then select New User.

In the New User window, in the User name text box, type Bill.

In the Password text box, type Pa55w.rd.

In the Confirm Password text box, type Pa55w.rd.

Click Create.

Click Close.

Select Users, and then verify that the user account Bill is listed under it.

Right-click Bill, and then select Properties.

Click the Member Of tab.

Click Add....

In the Select Groups window, in the Enter the object names to select text box, type Administrators.

Click OK twice.

Task 4: Rerun the CMPivot query to analyze local administrative users
Switch to LON-CFG, if the Configuration Manager console is not already open, on the taskbar, click the Configuration Manager Console icon.

Click the Asset and Compliance workspace, and then click Device Collections.

In the center panel, right-click All Desktop and Server Clients, and then click Start CMPivot.

In the CMPivot (All Desktop and Server Clients) window, click the Query tab.

On the Query tab, in the text box, type Administrators.

Click the Run Query button.

Review the results.

Notice that the user Bill is listed on LON-CL1.

Task 5: Export the CMPivot query results to a CSV file
In the CMPivot (All Desktop and Server Clients) window, on the Query tab, click Export, and then click Results To File.

In the Export to File window, under Quick access links, click Desktop.

In the File name text box, type List of who is in the local Administrator group, and then click Save.

On the computer's desktop, double-click the List of who is in the local Administrator group.csv file.

In the How do you want to open this file? window, select Notepad, and then click OK.

Notice these results are the same as the results listed in the CMPivot results pane.

Close Notepad.

Task 6: Run a CMPivot query to identify stopped services
In the CMPivot (All Desktop and Server Clients) window, on the Query tab, replace the existing text with Services | where State == 'Stopped'

Note: Make sure that "where" is in lowercase.

Click the Run Query button.

Review the results.

Replace existing text with Services | where State == 'Stopped' | summarize count() by Caption

Click the Run Query button.

Review the results.

On the Query Results tab, next to the Application Identity row, click 1.

Review results in both the query box and the results area.

Results: After this exercise, you should have created a CMPivot query to find all users who are listed as a local administrator for all the client computers in the collection. You should have also created a collection of all the client computers based on a CMPivot query, exported the results of users within the local Administrators group, run a query for services that are stopped, and reviewed a count list of all the stopped services.