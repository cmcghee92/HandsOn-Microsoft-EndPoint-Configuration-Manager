# Exercise 1
## Task 1: Create the Toronto Windows 11 Workstations collection

1. If the Microsoft Endpoint Configuration Manager (Configuration Manager) console is not already open, on LON-CFG, on the taskbar, click the Configuration Manager Console icon in the Taskbar.

2. In the Microsoft Endpoint Configuration Manager console, click the Assets and Compliance workspace, and then click the Device Collections node. Notice that several default collections that exist.

3. Right-click Device Collections, and then click Create Device Collection.

4. In the Create Device Collection Wizard, in the Name box, type Toronto Windows 11 Workstations.

5. In the Comment box, type Based upon the Active Directory Toronto Clients organizational unit, and then click Browse.

6. In the Select Collection dialog box, ensure that Device Collections is selected, select the All Systems collection, and then click OK.

7. In the Create Device Collection Wizard, click Next.

8. On the Membership Rules page, click the Add Rule list, and then click Query Rule.

9. In the Query Rule Properties dialog box, in the Name box, type Toronto Windows 11 Workstations.

10. In the Query Rule Properties dialog box, ensure that System Resource is listed, and then click Edit Query Statement.

11. In the Query Statement Properties dialog box, click the Criteria tab.

12. On the Criteria page, click New.

13. In the Criterion Properties dialog box, in the Criterion Type box, ensure that Simple value is selected, and then click Select.

14. In the Select Attribute dialog box, configure the following options, and then click OK:

    Attribute class: System Resource
    
    Alias as:
    
    Attribute: System OU Name

15, In the Criterion Properties dialog box, ensure that the Operator value is set to is equal to, and then in the Value box, type ADATUM.COM/TORONTO CLIENTS

16. To close the Criterion Properties dialog box, click OK.

17. To close the Query Statement Properties dialog box, click OK.

18. To close the Query Rule Properties dialog box, click OK.

19. In the Create Device Collection Wizard, on the Membership Rules page, ensure that both Use incremental updates for this collection and Schedule a full update on this collection are selected, and then click Next.

20. On the Summary page, click Next.

21. On the Completion page, click Close.

22. Ensure that the Device Collections node is selected, and then in the results pane, select the Toronto Windows 11 Workstations collection.

23. To refresh the collection, press F5, and then double-click the Toronto Windows 11 Workstations collection.

24. Verify that TOR-CL1 and TOR-CL2 display.

    Note: You might need to refresh the console to view the results.

    Results: After this exercise, you should have created device collections based on an Active Directory OU and on queries.

# Exercise 2: Creating a user collection
    Scenario
    
    You must create a user collection that contains all of the IT Staff. For your new collection, you decide to create an include collections rule to include the members of the IT OU.
    
    The main task for this exercise is as follows:
    
    Create the IT Staff collection.
## Task 1: Create the Toronto Users collection
1. If the Configuration Manager console is not already open, on LON-CFG, on the taskbar, click the Configuration Manager Console icon in the Taskbar.

In the Microsoft Endpoint Configuration Manager console, click the Assets and Compliance workspace, and then click the User Collections node. Notice that several default collections already exist.

Right-click User Collections, and then click Create User Collection.

In the Create User Collection Wizard, in the Name box, type IT Staff.

In the Comment box, type All IT Staff Globally, and then click Browse.

In the Select Collections dialog box, ensure that User Collections is selected, select the All Users collection, and then click OK.

In the Create User Collection Wizard, click Next.

On the Membership Rules page, click Add Rule, and then click Query Rule.

In the Name box, type IT Staff, and then click Edit Query Statement.

In the Query Statement Properties dialog box, click Criteria, and then click New.

In the Criterion Properties dialog box, click Select.

In the Select Attribute dialog box, in the Attribute class list, click User Resource.

In the Attribute list, click User OU Name, and then click OK.

Verify that the Operator displays is equal to, and then click Value.

In the Values dialog box, click ADATUM.COM/IT, and then click OK four times.

On the Membership Rules page, click Next twice, and then click Close.

In the list of user collections, click IT Staff, and then on the ribbon, click Update Membership.

In the Configuration Manager dialog box, click Yes.

With the User Collections node selected, in the results pane, double-click the IT Staff collection.

Verify that only the 27 IT Staff are in the collection.
