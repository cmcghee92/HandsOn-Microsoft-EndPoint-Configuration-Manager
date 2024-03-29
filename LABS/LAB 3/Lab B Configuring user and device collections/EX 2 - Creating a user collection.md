# Exercise 2: Creating a user collection
    Scenario
    
    You must create a user collection that contains all of the IT Staff. 
    For your new collection, you decide to create an include collections rule to include the members of the IT OU.
    
    The main task for this exercise is as follows:
    
    Create the IT Staff collection.
## Task 1: Create the Toronto Users collection
1. If the Configuration Manager console is not already open, on LON-CFG, on the taskbar, click the Configuration Manager Console icon in the Taskbar.

2. In the Microsoft Endpoint Configuration Manager console, click the Assets and Compliance workspace, and then click the User Collections node. Notice that several default collections already exist.

3. Right-click User Collections, and then click Create User Collection.

4. In the Create User Collection Wizard, in the Name box, type IT Staff.

5. In the Comment box, type All IT Staff Globally, and then click Browse.

6. In the Select Collections dialog box, ensure that User Collections is selected, select the All Users collection, and then click OK.

7. In the Create User Collection Wizard, click Next.

8. On the Membership Rules page, click Add Rule, and then click Query Rule.

9. In the Name box, type IT Staff, and then click Edit Query Statement.

10. In the Query Statement Properties dialog box, click Criteria, and then click New.

11. In the Criterion Properties dialog box, click Select.

12. In the Select Attribute dialog box, in the Attribute class list, click User Resource.

13. In the Attribute list, click User OU Name, and then click OK.

15. Verify that the Operator displays is equal to, and then click Value.

16. In the Values dialog box, click ADATUM.COM/IT, and then click OK four times.

17. On the Membership Rules page, click Next twice, and then click Close.

18. In the list of user collections, click IT Staff, and then on the ribbon, click Update Membership.

19. In the Configuration Manager dialog box, click Yes.

20. With the User Collections node selected, in the results pane, double-click the IT Staff collection.

21. Verify that only the 27 IT Staff are in the collection.