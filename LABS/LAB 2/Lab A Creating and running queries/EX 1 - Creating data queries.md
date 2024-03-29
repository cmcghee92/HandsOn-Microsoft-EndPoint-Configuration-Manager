Scenario

You have been asked to publish applications based on the Marketing, Production, and Research departments at A. Datum Corporation. You must build and test queries to find the users by department so that you can use these queries to create collections.

The main tasks for this exercise are as follows:

Create a query for Marketing users.
Create a query for Sales or Research users.
Run the user data queries.
Task 1: Create a query for Marketing users
Switch to LON-CFG and send the CTRL+ALT+DEL command and log in as ADATUM\AdatumAdmin with the password Pa55w.rd.

On the taskbar, click the Configuration Manager console icon.

Click the Monitoring workspace, and then click Queries.

Right-click the Queries node, and then click Create Query.

In the Create Query Wizard, on the General page, in the Name box, type Marketing Users, and then click Import Query Statement.

In the Browse Query dialog box, in the Queries box, click All Users, and then click OK.

In the Create Query Wizard, on the General page, click Edit Query Statement, and then click the Criteria tab.

In the Marketing Users Query Statement Properties dialog box, click New

In the Criterion Properties dialog box, click Select.

In the Select Attribute dialog box, in the Attribute class drop-down list, click User Resource.

In the Attribute drop-down list, click User Group Name, and then click OK.

In the Criterion Properties dialog box, verify that in the Operator box, the is equal to option is selected.

In the Value box, use the Value button to browse to ADATUM\Marketing, and then click OK twice.

In the Marketing Users Query Statement Properties dialog box, click OK.

In the Create Query Wizard, on the General page, click Next.

On the Summary page, click Next, and then on the Completion page, click Close.

Task 2: Create a query for Sales or Research users
Right-click the Queries node, and then click Create Query.

In the Create Query Wizard, on the General page, in the Name box, type Sales or Research Users, and then click Import Query Statement.

In the Browse Query dialog box, in the Queries box, click All Users, and then click OK.

In the Create Query Wizard, on the General page, click Edit Query Statement, and then click the Criteria tab.

In the Sales or Research Users Query Statement Properties dialog box, click New.

In the Criterion Properties dialog box, click the Criterion Type drop-down list, and then select List of values.

Click Select.

In the Select Attribute dialog box, in the Attribute class list, click User Resource.

In the Attribute list, click User Group Name, and then click OK.

In the Criterion Properties dialog box, verify that in the Operator box, the is in option is selected.

In the Value to add box, type ADATUM\Sales, and then click Add.

In the Value to add box, type ADATUM\Research, click Add, and then click OK.

In the Sales or Research Users Query Statement Properties dialog box, click OK.

In the Create Query Wizard, on the General page, click Next.

On the Summary page, click Next.

On the Completion page, click Close.

Task 3: Run the user data queries
Right-click the Marketing Users query, and then click Run.

Review the results, which should include 52 users.

Click the Queries node, right-click the Sales or Research Users query, and then click Run.

Review the results, which should include 80 users.

Results: After this exercise, you should have created and tested data queries in Configuration Manager.