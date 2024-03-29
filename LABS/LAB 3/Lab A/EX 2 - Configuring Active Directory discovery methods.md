# Exercise 2: Configuring Active Directory discovery methods
Scenario

The Active Directory administrator informed you that a new OU named Toronto Clients has been created, and it contains all of the computers located in Toronto. You need to configure the appropriate discovery methods to discover all the computers and users in the Toronto location. User discovery also must include the Active Directory department attribute. You also need to use an appropriate discovery method to help you configure boundaries and boundary groups, which these new locations will use.

The main tasks for this exercise are as follows:

Configure the Active Directory System Discovery method.
Configure the Active Directory User Discovery method.
Examine the discovered resources.
Prepare for the next lab.

## Task 1: Configure the Active Directory System Discovery method
1. Click the Administration workspace, expand Hierarchy Configuration, and then click Discovery Methods.

2. In the results pane, double-click Active Directory System Discovery. Select the Enable Active Directory System Discovery check box.

3. Click New.

4. In the Active Directory Container dialog box, click Browse.

5. In the Select New Container dialog box, click the Toronto Clients container, and then click OK.

6. Verify that the Recursively search Active Directory child containers check box is selected, and then click OK.

7. Repeat steps 3 through 6 for Toronto Servers, Sydney Clients, and Sydney Servers.

8. On the Polling Schedule tab, click Schedule, configure the recurrence to take place every 5 days, and then click OK.

9. Verify that the Enable delta discovery check box is selected and that the interval is configured as 5 minutes, and then click OK.

10. Right-click Active Directory System Discovery, and then click Run Full Discovery Now.

11. When Configuration Manager displays the Do you want to run full discovery as soon as possible? message, click Yes.

## Task 2: Configure the Active Directory User Discovery method
1. On LON-CFG, in the Microsoft Endpoint Configuration Manager console, click the Administration workspace, and then expand Hierarchy Configuration.

2. Click the Discovery Methods node, and then double-click Active Directory User Discovery.

3. In the Active Directory User Discovery Properties dialog box, verify that the Enable Active Directory User Discovery check box is selected.

4. Click New, and then click Browse.

5. In the Select New Container dialog box, click the Adatum container, and then click OK.

6. Verify that the Recursively search Active Directory child containers check box is selected, and then click OK.

7. On the Polling Schedule tab, click Schedule, configure the recurrence to take place every 3 days, and then click OK.

8. Verify that the Enable delta discovery check box is selected with an interval of 5 minutes.

9. On the Active Directory Attributes tab, in the Available attributes list, scroll down and click the department attribute, click Add, and then click OK.

10. Right-click Active Directory User Discovery, and then click Run Full Discovery Now.

11. When Configuration Manager displays the Do you want to run full discovery as soon as possible? message, click Yes.

## Task 3: Examine the discovered resources
1. Click the Assets and Compliance workspace.

2. In the Assets and Compliance workspace, click the Devices node.

3. In the results pane, right-click TOR-CL2, and then click Properties.

    Note: Notice that the client was discovered by using the SMS_AD_SYSTEM_DISCOVERY_AGENT component and that it resides in the Toronto Clients OU.

3. Click Close.

4. Click the Administration workspace, expand the Hierarchy Configuration node, and then click the Active Directory Forests node.

5. In the preview pane, click the Domains tab. Notice that the Adatum.com domain has been discovered.

6. Click the Discovery Status tab, and then verify that the discovery has succeeded.

8. Click the Publishing Status tab, and verify that the publishing has succeeded.

9. In the results pane, right-click Adatum.com, and then click Show Active Directory Sites. Notice that three sites have been discovered: AdatumHQ, Sydney, and Toronto. Click Back.

10. In the results pane, right-click Adatum.com, and then click Show IP Subnets. Notice that three IP subnets have been discovered:

    172.16.0.0/24

    172.16.1.0/24

    172.16.2.0/24