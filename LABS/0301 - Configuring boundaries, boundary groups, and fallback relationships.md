## Task 1: Configure boundaries

1. Switch to LON-CFG and send the CTRL+ALT+DEL command and log in as ADATUM\AdatumAdmin with the password Pa55w.rd.

2. Right-click the network icon on the taskbar and select Open Network & Internet settings. Select Change adapter options. Disable and re-enable the network adapter. This ensures the network profile for the adatum.com domain is set correctly.

3. Repeat the above step on LON-DC1.

4. On the taskbar, click the Configuration Manager console icon.

5. In the Microsoft Endpoint Configuration Manager console, click the Administration workspace, and then expand Hierarchy Configuration.

6. Click Discovery Methods, and then click Active Directory Forest Discovery.

7. On the ribbon, click Properties.

8. In the Active Directory Forest Discovery Properties dialog box, select the following check boxes:

9. Enable Active Directory Forest Discovery

10. Automatically create Active Directory site boundaries when they are discovered

  Note: Do not select the Automatically create IP address range boundaries for IP subnets when they are discovered check box.

11. To close the Active Directory Forest Discovery Properties dialog box, click OK.

12. When you see the Do you want to run full discovery as soon as possible? message, click Yes.

    Note: Before continuing, wait approximately one minute for the discovery to complete and for boundary objects to be created.

13. Click the Boundaries node, and then refresh the details pane. It might take a minute or two for the results to display.

    Note: Do not continue until you see the following boundaries created by the Active Directory Forest Discovery method:

    Adatum HQ
    
    Sydney
    
    Toronto

## Task 2: Configure boundary groups and relationships

1. Right-click Boundary Groups, and then click Create Boundary Group.

2. In the Name box, type London, and then click Add.

2. In the Add Boundaries dialog box, select AdatumHQ, and then click OK.

4. In the Create Boundary Group dialog box, click the References tab, and then click Add.

5. In the Add Site Systems dialog box, select \\LON-CFG.Adatum.com, and then click OK.

6. Under Site assignment, select the check box next to Use this boundary group for site assignment.

7. To close the Create Boundary Group dialog box, click OK.

8. Right-click Boundary Groups, and then click Create Boundary Group.

9. In the Name box, type Toronto, and then click Add.

10. In the Add Boundaries dialog box, select Toronto, and then click OK.

11. In the Create Boundary Group dialog box, click the References tab, and then click Add.

12. In the Add Site Systems dialog box, select \\LON-CFG.Adatum.com, and then click OK.

13. Under Site assignment, select the check box next to Use this boundary group for site assignment.

14. To close the Create Boundary Group dialog box, click OK.

15. Verify that Toronto now displays in the results pane.

16. Right-click Boundary Groups, and then click Create Boundary Group.

17. In the Name box, type Sydney, and then click Add.

18. In the Add Boundaries dialog box, select Sydney, and then click OK.

19. In the Create Boundary Group dialog box, click the References tab.

20. Under Site assignment, select the check box next to Use this boundary group for site assignment.

21. To close the Create Boundary Group dialog box, click OK.

22. Verify that Sydney now displays in the results pane.

 ### Configure fallback
1. In the Administration workspace, click the Boundary Groups node.

2. Right-click Sydney and then click Properties.

3. In the Sydney Properties dialog box, click the Relationships tab, and then click Add.

4. In the Fallback Boundary Groups dialog box, select London.

5. Under Fallback times (in minutes), change the Distribution point value to 10 minutes.

6. Click OK to close the Fallback Boundary Groups dialog box. This will ensure that if a client cannot find a distribution point within 10 minutes, it will fall back and use the Distribution point in London.

7. Click OK to close the Sydney Properties dialog box.

  Results: After completing this exercise, you should have created and configured boundaries and boundary groups.
