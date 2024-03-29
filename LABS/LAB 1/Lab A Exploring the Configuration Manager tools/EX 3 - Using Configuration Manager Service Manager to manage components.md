# Exercise 3: Using Configuration Manager Service Manager to manage components

Scenario

Configuration Manager Service Manager enables you to control the different services and threads that make up a Configuration Manager site system. You might find that the generated log files are too small, or you might want to change the location to which Configuration Manager saves the log files. Additionally, you might find it beneficial to stop or start a service while troubleshooting a problem. In this exercise, you will explore the options available in the Configuration Manager Service Manager.

The main tasks for this exercise are as follows:

Configure the log file size for a single component.
Manage Configuration Manager components.
## Task 1: Configure the log file size for a single component
1. Click the Monitoring workspace, and expand the System Status folder.

2. Click the Component Status node.

3. On the ribbon, click the Home tab, click the Start drop-down list box, and then click Configuration Manager Service Manager.

4. Click to expand S01, and click **Components**.
5. In the right pane, scroll down, right-click **SMS_POLICY_PROVIDER**, and then click Logging.
6. In the Configuration Manager Component Logging - Single Component dialog box, set the Log Size (MB): scroll box to 5.
7. From the Log filename field, write down the name of the log file that displays.
8. To close the Configuration Manager Component Logging - Single Component dialog box, click **OK**.

##Task 2: Manage Configuration Manager components
1. Right-click SMS_POLICY_PROVIDER, and click **Select All**.

2. Right-click one of the selected components, and click **Query**.
3. To dismiss the Configuration Manager Service Manager dialog box, click **OK**. You can dismiss the messages about error communicating with components. This message indicates that some components are not configured, which is expected.

4. Scroll through the list of services, and note that some services are not running. To remove the highlighting, click **SMS_POLICY_PROVIDER**.

5. Right-click SMS_POLICY_PROVIDER, and click **Stop**. Note that the status display does not change.

6. Right-click SMS_POLICY_PROVIDER, and click **Query**.

7. Right-click SMS_POLICY_PROVIDER, and click **Start**.

8. Right-click SMS_POLICY_PROVIDER, and click **Query**.

9. Close the Configuration Manager Service Manager.

Results: At the end of this exercise, you should have used Configuration Manager Service Manager to manage Configuration Manager components by adjusting the log file sizes, and stopping and starting components.
