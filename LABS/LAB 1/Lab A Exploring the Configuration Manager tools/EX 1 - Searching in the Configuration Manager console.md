# Exercise 1: Searching in the Configuration Manager console 

Scenario

In this exercise, you will examine the search functions. The search features in the Configuration Manager console enable you to perform local and global searches.

The main tasks for this exercise are as follows:

Using console filters.
Using search criteria.
Create and save a local node search.
Create and save a global search.
Use saved searches.
Task 1: Using console filters
Switch to LON-CFG and send the CTRL+ALT+DEL command and log in as ADATUM\AdatumAdmin with the password Pa55w.rd.

On the taskbar, click the Configuration Manager console icon.

In the Configuration Manager console, in the Assets and Compliance workspace, click the Users node.

Note: At the top of the results pane, the Users indicator shows that there are 282 items in the results pane.

In the search bar, type ch, and then click Search.

The Users indicator shows that there are 26 items.

Task 2: Using search criteria
Click the Devices node.

Note: At the top of the results pane, the Devices indicator shows that 8 items are in the results pane.

Click the Add Criteria link. Note the available criteria for devices.

Click Name.

In the AND Name row, in the Enter valid characters text box, type LON, and then click Search.

Verify that the Devices indicator now shows that there are 7 items.

Click the Add Criteria link.

Scroll down, then click Operating System.

In the AND Operating System row, in the Enter valid characters text box,type Server, and then click Search.

Note: Note that the results contain four servers LON-DC1, LON-SVR1, LON-SVR2, and LON-CFG.

In the AND Operating System row, delete Server, and in the Enter valid characters text box, type Windows, and then click Search.

Note: The results show that all the LON computers run a Windows operating system.

Task 3: Create and save a local node search
In the Configuration Manager console, click the Assets and Compliance workspace.

Click User Collections.

Double-click All Users. This runs a local node search automatically, and displays all the members of the collection.

Next to the Search button, click Add Criteria, select the Name check box, and then click Add.

In the AND Name row, click contains, and then note the options available for refining the search.

Click starts with, type Adatum\T in the Enter valid characters text box, and then click Search. The results are now limited to the Adatum users whose names begin with T.

On the ribbon, in the Save group, click Save Current Search.

In the Configuration Manager dialog box, type T users, and then click OK.

Task 4: Create and save a global search
Select the Overview node, and on the ribbon, click All Objects.

In the Search text box, type Configuration Manager, and then click Search.

Note: Notice the different Object Types and Workspaces that the search returns.

On the ribbon, in the Save group, click Save Current Search.

In the Configuration Manager dialog box, in the Search name field, type Configuration Manager Objects, and then click OK.

Close the Configuration Manager console.

Task 5: Use saved searches
On the taskbar, click the Configuration Manager console icon.

Note: You should notice that the sticky nodes from your previous searches were closed when the console was closed.

On the ribbon, click Saved Searches. This displays a drop-down list of the saved searches categories.

Note: The only available option is global searches: Manage Searches for All Objects.

In the Configuration Manager console, click the Assets and Compliance workspace.

Click the User Collections node.

Click Saved Searches, and click Manage Searches for Current Node. Note that no searches are available, and click Cancel.

Double-click the All Users collection.

On the ribbon, click the Home tab.

Click Saved Searches, and click Manage Searches for Current Node. Note that the T users search is available, and click Cancel.

Click the Device Collections node.

On the ribbon, click Saved Searches, and then click Manage Searches for All Objects.

Click the Configuration Manager Objects search, and click OK.

Note: This displays the same results as before.

Results: At the end of this exercise, you should have performed both local node and global searches. You also should have refined the local node search and saved the custom local node search for future use. Finally, you should have observed the differences between saving a global search and saving a local node search. You can view the expected results in the lab answer key.