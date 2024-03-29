Task 1: Configure boundaries
Switch to LON-CFG and send the CTRL+ALT+DEL command and log in as ADATUM\AdatumAdmin with the password Pa55w.rd.

Right-click the network icon on the taskbar and select Open Network & Internet settings. Select Change adapter options. Disable and re-enable the network adapter. This ensures the network profile for the adatum.com domain is set correctly.

Repeat the above step on LON-DC1.

On the taskbar, click the Configuration Manager console icon.

In the Microsoft Endpoint Configuration Manager console, click the Administration workspace, and then expand Hierarchy Configuration.

Click Discovery Methods, and then click Active Directory Forest Discovery.

On the ribbon, click Properties.

In the Active Directory Forest Discovery Properties dialog box, select the following check boxes:

Enable Active Directory Forest Discovery

Automatically create Active Directory site boundaries when they are discovered

Note: Do not select the Automatically create IP address range boundaries for IP subnets when they are discovered check box.

To close the Active Directory Forest Discovery Properties dialog box, click OK.

When you see the Do you want to run full discovery as soon as possible? message, click Yes.

Note: Before continuing, wait approximately one minute for the discovery to complete and for boundary objects to be created.

Click the Boundaries node, and then refresh the details pane. It might take a minute or two for the results to display.

Note: Do not continue until you see the following boundaries created by the Active Directory Forest Discovery method:

Adatum HQ

Sydney

Toronto

Task 2: Configure boundary groups and relationships
Right-click Boundary Groups, and then click Create Boundary Group.

In the Name box, type London, and then click Add.

In the Add Boundaries dialog box, select AdatumHQ, and then click OK.

In the Create Boundary Group dialog box, click the References tab, and then click Add.

In the Add Site Systems dialog box, select \\LON-CFG.Adatum.com, and then click OK.

Under Site assignment, select the check box next to Use this boundary group for site assignment.

To close the Create Boundary Group dialog box, click OK.

Right-click Boundary Groups, and then click Create Boundary Group.

In the Name box, type Toronto, and then click Add.

In the Add Boundaries dialog box, select Toronto, and then click OK.

In the Create Boundary Group dialog box, click the References tab, and then click Add.

In the Add Site Systems dialog box, select \\LON-CFG.Adatum.com, and then click OK.

Under Site assignment, select the check box next to Use this boundary group for site assignment.

To close the Create Boundary Group dialog box, click OK.

Verify that Toronto now displays in the results pane.

Right-click Boundary Groups, and then click Create Boundary Group.

In the Name box, type Sydney, and then click Add.

In the Add Boundaries dialog box, select Sydney, and then click OK.

In the Create Boundary Group dialog box, click the References tab.

Under Site assignment, select the check box next to Use this boundary group for site assignment.

To close the Create Boundary Group dialog box, click OK.

Verify that Sydney now displays in the results pane.

Configure fallback
In the Administration workspace, click the Boundary Groups node.

Right-click Sydney and then click Properties.

In the Sydney Properties dialog box, click the Relationships tab, and then click Add.

In the Fallback Boundary Groups dialog box, select London.

Under Fallback times (in minutes), change the Distribution point value to 10 minutes.

Click OK to close the Fallback Boundary Groups dialog box. This will ensure that if a client cannot find a distribution point within 10 minutes, it will fall back and use the Distribution point in London.

Click OK to close the Sydney Properties dialog box.

Results: After completing this exercise, you should have created and configured boundaries and boundary groups.