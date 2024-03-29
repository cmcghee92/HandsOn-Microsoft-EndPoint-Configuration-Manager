# Exercise 2: Creating subselect queries

Scenario

You must create a query to identify all users who are not in the Marketing department so that you can select only these users for certain applications without including the Marketing department.

The main tasks for this exercise are as follows:

Create a query for users who are in the Marketing department.

Create a query for users who are not in the Marketing department.

## Task 1: Create a query for users who are in the Marketing department
1. Right-click the **Queries** node, and then click **Create Query**.

2. In the Create Query Wizard, on the General page, in the **Name** box, type **All Marketing Users**.

3. In the Object Type drop-down list, click **User Resource**, and then click **Edit Query Statement**.

4. In the** All Marketing Users** Query Statement Properties dialog box, on the General tab, click **New**

5. In the Result Properties dialog box, click **Select**.

6. In the Select Attribute dialog box, in the Attribute drop-down list, click **Unique User Name**, and then click **OK**.

7. In the Result Properties dialog box, click **OK**.

8. In the **All Marketing Users** Query Statement Properties dialog box, click the **Criteria** tab, and then click **New**

9. In the Criterion Properties dialog box, click **Select**.

10. In the Select Attribute dialog box, in the Attribute Class list, click **User Resource**.

11. In the Attribute list, click **User Group Name**, and then click **OK**.

12. In the Criterion Properties dialog box, verify that in the **Operator box**, the **is equal to** option is **selected**.

13. In the Value box, type **ADATUM\Marketing**, and then click **OK**.

14. In the **All Marketing Users** Query Statement Properties dialog box, click **OK**.

15. In the Create Query Wizard, on the General page, click **Next**.

16. On the Summary page, click **Next**.

17. On the Completion page, click **Close**.

## Task 2: Create a query for users who are not in the Marketing department
1. Right-click the **Queries node**, and then click **Create Query**.

2. In the Create Query Wizard, on the General page, in the Name box, type **Users Not in the Marketing Group**, and then click **Import Query Statement**.

3. In the Browse Query dialog box, in the Queries box, click **All Users**, and then click **OK**.

4. In the Create Query Wizard, on the General page, click **Edit Query Statement**, and then click the **Criteria** tab.

5. In the Users Not in the Marketing Group Query Statement Properties dialog box, click **New**

6. In the Criterion Properties dialog box, in the Criterion Type drop-down list, click **SubSelected values**, and then click **Select**.

7. In the Select Attribute dialog box, in the Attribute class list, click **User Resource**.

8. In the Attribute list, click **Unique User Name**, and then click **OK**.

9. In the Criterion Properties dialog box, in the **Operator list**, select **is not in**.

10. Click **Browse**, browse to and **select** the **All Marketing Users** query, and then click **OK**.

11. In the Criterion Properties dialog box, click **OK**.

12. In the Users Not in the Marketing Group Query Statement Properties dialog box, click **OK**.

13. In the Create Query Wizard, on the General page, click **Next**.

14. On the Summary page, click **Next**.

15. On the Completion page, click **Close**.

16. Right-click the Users Not in the Marketing Group query, and then click **Run**.

17. Review the results, which should include 203 users.

18. Minimize the Configuration Manager console.

Results: After this exercise, you should have created and tested a subselected data query in Configuration Manager.
