# Exercise 1: Searching in the Configuration Manager console 

Scenario

In this exercise, you will examine the search functions. The search features in the Configuration Manager console enable you to perform local and global searches.

The main tasks for this exercise are as follows:

Using console filters.
Using search criteria.
Create and save a local node search.
Create and save a global search.
Use saved searches.

# Task 1: Using console filters
1. Switch to LON-CFG and send the CTRL+ALT+DEL command and log in as ADATUM\AdatumAdmin with the password Pa55w.rd.

2. On the taskbar, click the Configuration Manager console icon.

3. In the Configuration Manager console, in the Assets and Compliance workspace, click the Users node.

    Note: At the top of the results pane, the Users indicator shows that there are 282 items in the results pane.

4. In the search bar, type ch, and then click Search.

5. he Users indicator shows that there are 26 items.

# Task 2: Using search criteria
1. Click the Devices node.

    Note: At the top of the results pane, the Devices indicator shows that 8 items are in the results pane.

2. Click the Add Criteria link. Note the available criteria for devices.

3. Click Name.

4. In the AND Name row, in the Enter valid characters text box, type LON, and then click Search.

5. Verify that the Devices indicator now shows that there are 7 items.

6. Click the Add Criteria link.

7. Scroll down, then click Operating System.

8. In the AND Operating System row, in the Enter valid characters text box,type Server, and then click Search.

    Note: Note that the results contain four servers LON-DC1, LON-SVR1, LON-SVR2, and LON-CFG.

9. In the AND Operating System row, delete Server, and in the Enter valid characters text box, type Windows, and then click Search.

    Note: The results show that all the LON computers run a Windows operating system.

# Task 3: Create and save a local node search

1. In the Configuration Manager console, click the Assets and Compliance workspace.

2. Click User Collections.

3. Double-click All Users. This runs a local node search automatically, and displays all the members of the collection.

4. Next to the Search button, click Add Criteria, select the Name check box, and then click Add.

6. In the AND Name row, click contains, and then note the options available for refining the search.

7. Click starts with, type Adatum\T in the Enter valid characters text box, and then click Search. The results are now limited to the Adatum users whose names begin with T.

8. On the ribbon, in the Save group, click Save Current Search.

9. In the Configuration Manager dialog box, type T users, and then click OK.

# Task 4: Create and save a global search

1. Select the Overview node, and on the ribbon, click All Objects.

2. In the Search text box, type Configuration Manager, and then click Search.

    Note: Notice the different Object Types and Workspaces that the search returns.

3. On the ribbon, in the Save group, click Save Current Search.

4. In the Configuration Manager dialog box, in the Search name field, type Configuration Manager Objects, and then click OK.

5. Close the Configuration Manager console.

# Task 5: Use saved searches
1. On the taskbar, click the Configuration Manager console icon.

    Note: You should notice that the sticky nodes from your previous searches were closed when the console was closed.

2. On the ribbon, click Saved Searches. This displays a drop-down list of the saved searches categories.

    Note: The only available option is global searches: Manage Searches for All Objects.

3. In the Configuration Manager console, click the Assets and Compliance workspace.

4. Click the User Collections node.

5. Click Saved Searches, and click Manage Searches for Current Node. Note that no searches are available, and click Cancel.

6. Double-click the All Users collection.

7. On the ribbon, click the Home tab.

8. Click Saved Searches, and click Manage Searches for Current Node. Note that the T users search is available, and click Cancel.

9. Click the Device Collections node.

10. On the ribbon, click Saved Searches, and then click Manage Searches for All Objects.

11. Click the Configuration Manager Objects search, and click OK.

    Note: This displays the same results as before.

Results: At the end of this exercise, you should have performed both local node and global searches. You also should have refined the local node search and saved the custom local node search for future use. Finally, you should have observed the differences between saving a global search and saving a local node search. You can view the expected results in the lab answer key.