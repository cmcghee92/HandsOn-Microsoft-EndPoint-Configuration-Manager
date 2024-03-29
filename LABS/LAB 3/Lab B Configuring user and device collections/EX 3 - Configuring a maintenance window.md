# Exercise 3: Configuring a maintenance window
Scenario

Your final task is to ensure that Toronto deployments can occur only during the hours of 8 P.M. and 4 A.M. each day. You will configure a maintenance window to accomplish this task.

The main task for this exercise is as follows:

Configure a maintenance window for Toronto Windows 11 workstations.
Prepare for the next module.
## Task 1: Configure a maintenance window for Toronto Windows 10 workstations
1. If the Configuration Manager console is not already open, on LON-CFG, on the taskbar, click the Configuration Manager Console icon in the taskbar.

2. In the Microsoft Endpoint Configuration Manager console, click the Assets and Compliance workspace, and then click the Device Collections node.

3. Right-click the Toronto Windows 11 Workstations node, and then click Properties.

4. In the Toronto Windows 11 Workstations Properties dialog box, click the Maintenance Windows tab.

5. On the Maintenance Windows page, click New.

6. In the Schedule dialog box, in the Name box, type Deployment Window.

7. Configure the schedule as follows, and then click OK:

    Start: 8 P.M.

    End: 4 A.M.

    Recurrence pattern: Daily

8. On the General tab, in the Comment box, type Maintenance Windows: 8 P.M. to 4 A.M.

9. In the Toronto Windows 10 Workstations Properties dialog box, click OK.

Results: At the end of this exercise, you should have created a maintenance window.