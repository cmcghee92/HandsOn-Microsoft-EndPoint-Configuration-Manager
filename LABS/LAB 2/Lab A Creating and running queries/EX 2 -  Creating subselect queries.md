cenario

You must create a query to identify all users who are not in the Marketing department so that you can select only these users for certain applications without including the Marketing department.

The main tasks for this exercise are as follows:

Create a query for users who are in the Marketing department.
Create a query for users who are not in the Marketing department.
Prepare for the next lab.
Task 1: Create a query for users who are in the Marketing department
Right-click the Queries node, and then click Create Query.

In the Create Query Wizard, on the General page, in the Name box, type All Marketing Users.

In the Object Type drop-down list, click User Resource, and then click Edit Query Statement.

In the All Marketing Users Query Statement Properties dialog box, on the General tab, click New

In the Result Properties dialog box, click Select.

In the Select Attribute dialog box, in the Attribute drop-down list, click Unique User Name, and then click OK.

In the Result Properties dialog box, click OK.

In the All Marketing Users Query Statement Properties dialog box, click the Criteria tab, and then click New

In the Criterion Properties dialog box, click Select.

In the Select Attribute dialog box, in the Attribute Class list, click User Resource.

In the Attribute list, click User Group Name, and then click OK.

In the Criterion Properties dialog box, verify that in the Operator box, the is equal to option is selected.

In the Value box, type ADATUM\Marketing, and then click OK.

In the All Marketing Users Query Statement Properties dialog box, click OK.

In the Create Query Wizard, on the General page, click Next.

On the Summary page, click Next.

On the Completion page, click Close.

Task 2: Create a query for users who are not in the Marketing department
Right-click the Queries node, and then click Create Query.

In the Create Query Wizard, on the General page, in the Name box, type Users Not in the Marketing Group, and then click Import Query Statement.

In the Browse Query dialog box, in the Queries box, click All Users, and then click OK.

In the Create Query Wizard, on the General page, click Edit Query Statement, and then click the Criteria tab.

In the Users Not in the Marketing Group Query Statement Properties dialog box, click New

In the Criterion Properties dialog box, in the Criterion Type drop-down list, click SubSelected values, and then click Select.

In the Select Attribute dialog box, in the Attribute class list, click User Resource.

In the Attribute list, click Unique User Name, and then click OK.

In the Criterion Properties dialog box, in the Operator list, select is not in.

Click Browse, browse to and select the All Marketing Users query, and then click OK.

In the Criterion Properties dialog box, click OK.

In the Users Not in the Marketing Group Query Statement Properties dialog box, click OK.

In the Create Query Wizard, on the General page, click Next.

On the Summary page, click Next.

On the Completion page, click Close.

Right-click the Users Not in the Marketing Group query, and then click Run.

Review the results, which should include 203 users.

Minimize the Configuration Manager console.

Results: After this exercise, you should have created and tested a subselected data query in Configuration Manager.