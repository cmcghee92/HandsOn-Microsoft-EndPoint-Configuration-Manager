Task 1: Configure the Active Directory System Discovery method
1. Click the Administration workspace, expand Hierarchy Configuration, and then click Discovery Methods.

2. In the results pane, double-click Active Directory System Discovery. Select the Enable Active Directory System Discovery check box.

3. Click New.

In the Active Directory Container dialog box, click Browse.

In the Select New Container dialog box, click the Toronto Clients container, and then click OK.

Verify that the Recursively search Active Directory child containers check box is selected, and then click OK.

Repeat steps 3 through 6 for Toronto Servers, Sydney Clients, and Sydney Servers.

On the Polling Schedule tab, click Schedule, configure the recurrence to take place every 5 days, and then click OK.

Verify that the Enable delta discovery check box is selected and that the interval is configured as 5 minutes, and then click OK.

Right-click Active Directory System Discovery, and then click Run Full Discovery Now.

When Configuration Manager displays the Do you want to run full discovery as soon as possible? message, click Yes.

Task 2: Configure the Active Directory User Discovery method
On LON-CFG, in the Microsoft Endpoint Configuration Manager console, click the Administration workspace, and then expand Hierarchy Configuration.

Click the Discovery Methods node, and then double-click Active Directory User Discovery.

In the Active Directory User Discovery Properties dialog box, verify that the Enable Active Directory User Discovery check box is selected.

Click New, and then click Browse.

In the Select New Container dialog box, click the Adatum container, and then click OK.

Verify that the Recursively search Active Directory child containers check box is selected, and then click OK.

On the Polling Schedule tab, click Schedule, configure the recurrence to take place every 3 days, and then click OK.

Verify that the Enable delta discovery check box is selected with an interval of 5 minutes.

On the Active Directory Attributes tab, in the Available attributes list, scroll down and click the department attribute, click Add, and then click OK.

Right-click Active Directory User Discovery, and then click Run Full Discovery Now.

When Configuration Manager displays the Do you want to run full discovery as soon as possible? message, click Yes.

Task 3: Examine the discovered resources
Click the Assets and Compliance workspace.

In the Assets and Compliance workspace, click the Devices node.

In the results pane, right-click TOR-CL2, and then click Properties.

Note: Notice that the client was discovered by using the SMS_AD_SYSTEM_DISCOVERY_AGENT component and that it resides in the Toronto Clients OU.

Click Close.

Click the Administration workspace, expand the Hierarchy Configuration node, and then click the Active Directory Forests node.

In the preview pane, click the Domains tab. Notice that the Adatum.com domain has been discovered.

Click the Discovery Status tab, and then verify that the discovery has succeeded.

Click the Publishing Status tab, and verify that the publishing has succeeded.

In the results pane, right-click Adatum.com, and then click Show Active Directory Sites. Notice that three sites have been discovered: AdatumHQ, Sydney, and Toronto. Click Back.

In the results pane, right-click Adatum.com, and then click Show IP Subnets. Notice that three IP subnets have been discovered:

172.16.0.0/24

172.16.1.0/24

172.16.2.0/24