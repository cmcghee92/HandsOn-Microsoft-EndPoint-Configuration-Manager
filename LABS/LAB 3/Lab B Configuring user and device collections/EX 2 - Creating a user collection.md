# Exercise 2: Creating a user collection
    Scenario
    
    You must create a user collection that contains all of the IT Staff. 
    For your new collection, you decide to create an include collections rule to include the members of the IT OU.
    
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
