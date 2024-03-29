# Exercise 1: Using CMPivot to Analyze the current state of devices

Scenario

Your security manager needs to know the machines on which a specific user is listed as a local administrator. You decide to use CMPivot to analyze and determine the results. You are also having issues with some of your client computers and need to determine which services are in a stopped state. You will use CMPivot to determine the results for these issues also.

# Exercise 1: Using CMPivot to Analyze the current state of devices
Scenario

You need to use CMPivot to find the user who is listed as the local administrator for all the client computers in the collection. You also need to run a CMPivot query to identify the services that are stopped, and then determine the results.

The main tasks for this exercise are as follows:

Create a CMPivot query to analyze local administrative users.

Create a collection based on the CMPivot query results.

Create a user on LON-CL1.

Rerun the CMPivot query to analyze local administrative users.

Export the CMPivot query results to a CSV file.

Run a CMPivot query to identify stopped services.

## Task 1: Create a CMPivot query to analyze local administrative users
1. On LON-CFG, if the Configuration Manager console is not already open, on the taskbar, click the Configuration Manager Console icon.
2. Click the Asset and Compliance workspace, and then click Device Collections.
3. In the center panel, right-click All Desktop and Server Clients, and then click Start CMPivot.
4. In the CMPivot (All Desktop and Server Clients) window, click the Query tab.
5. On the Query tab, in the text box, type Administrators.
6. Click the Run Query button.
7. Review the results.

## Task 2: Create a collection based on the CMPivot query results
1. In CMPivot, select the Query Summary tab.
2. Next to the Offline row, click 1.
3. In the Offline Devices window, make a note of the reason for the failure.
4. Click Create Collection.
5. In the Create Device Collection Wizard, on the General page, in the Name box, type Test collection using CMPivot query.
6. Click Next.
7. On the Membership Rules page, clear the Schedule a full update on this collection check box.
8. Click Summary.
9. On the Summary page, click Next.
10. On the Completed page, click Close.
11. Close the CMPivot (All Desktop and Server Clients) window.

## Task 3: Create a user on LON-CL1
1. Switch to LON-CL1 and send the CTRL+ALT+DEL command and log in as ADATUM\AdatumAdmin with the password Pa55w.rd.
2. On LON-CL1, click Start and then type Computer Management.
3. Click Computer Management.
4. In the Computer Management window, expand Local Users and Groups.
5. Right-click Users, and then select New User.
6. In the New User window, in the User name text box, type Bill.
7. In the Password text box, type Pa55w.rd.
8. In the Confirm Password text box, type Pa55w.rd.
9. Click Create.
10. Click Close.
11. Select Users, and then verify that the user account Bill is listed under it.
12. Right-click Bill, and then select Properties.
13. Click the Member Of tab.
14. Click Add....
15. In the Select Groups window, in the Enter the object names to select text box, type Administrators.
16. Click OK twice.

## Task 4: Rerun the CMPivot query to analyze local administrative users
1. Switch to LON-CFG, if the Configuration Manager console is not already open, on the taskbar, click the Configuration Manager Console icon.
2. Click the Asset and Compliance workspace, and then click Device Collections.
3. In the center panel, right-click All Desktop and Server Clients, and then click Start CMPivot.
4. In the CMPivot (All Desktop and Server Clients) window, click the Query tab.
5. On the Query tab, in the text box, type Administrators.
6. Click the Run Query button.
7. Review the results.
    Notice that the user Bill is listed on LON-CL1.

## Task 5: Export the CMPivot query results to a CSV file
1. In the CMPivot (All Desktop and Server Clients) window, on the Query tab, click Export, and then click Results To File.
2. In the Export to File window, under Quick access links, click Desktop.
3. In the File name text box, type List of who is in the local Administrator group, and then click Save.
4. On the computer's desktop, double-click the List of who is in the local Administrator group.csv file.
5. In the How do you want to open this file? window, select Notepad, and then click OK.
    Notice these results are the same as the results listed in the CMPivot results pane.
6. Close Notepad.

## Task 6: Run a CMPivot query to identify stopped services
1. In the CMPivot (All Desktop and Server Clients) window, on the Query tab, replace the existing text with Services | where State == 'Stopped'

    Note: Make sure that "where" is in lowercase.

2. Click the Run Query button.
3. Review the results.
4. Replace existing text with Services | where State == 'Stopped' | summarize count() by Caption
5. Click the Run Query button.
6. Review the results.
7. On the Query Results tab, next to the Application Identity row, click 1.
8. Review results in both the query box and the results area.

Results: After this exercise, you should have created a CMPivot query to find all users who are listed as a local administrator for all the client computers in the collection. You should have also created a collection of all the client computers based on a CMPivot query, exported the results of users within the local Administrators group, run a query for services that are stopped, and reviewed a count list of all the stopped services.
