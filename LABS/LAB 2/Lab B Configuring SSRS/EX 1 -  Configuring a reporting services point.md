# Exercise 1: Configuring a reporting services point

Scenario

To implement a reporting services point, you first need to install and configure SSRS. The SQL team installed SSRS, but did not configure it. Therefore, you need to configure it before you can install a reporting services point. After installing the reporting services point, you should test the installation by running reports in both the Configuration Manager console and the SQL Server Reporting Services website.

The main tasks for this exercise are as follows:

Configure SSRS.
Install and configure the reporting services point role.

Test the reporting services point in the Configuration Manager console.

Test the reporting services point in the SQL Server Reporting Services website.

## Task 1: Configure SSRS
1. On **LON-CFG**, click **Start**, expand **Microsoft SQL Server Reporting Services**, and then click **Reporting Services Configuration Manager**.

2. In the Reporting Services Configuration Connection dialog box, click **Connect**.
3.  Wait for Connection 
4. In Reporting Services Configuration Manager:**LON-CFG\SSRS**, click the** Service Account** node.

5. Under Report Server Service Account, verify that the Virtual Service Account account is being used.

6. Click the **Web Service URL** node, and review the default settings. Observe the settings already configured for Configuration Manager reporting.

7. On the Database page and note the database being used.

8. In Reporting Services Configuration Manager:**LON-CFG\SSRS,** click the **Web Portal URL** node. Verify the URL is functioning by clicking on the link.

9. Click the **URL**, and then verify that the SQL Server Reporting Services Home page appears.

10. Close Microsoft Edge.

11. In Reporting Services Configuration Manager:**LON-CFG\MSSQLSERVER**, click **Exit**.

## Task 2: Install and configure the reporting services point role
1. Restore the Configuration Manager console.

2. Click the **Administration** workspace, and then expand **Site Configuration**.

3. Click **Servers and Site Systems Roles**.

4. Right-click **\\LON-CFG.Adatum.com**, and then click **Add Site System Roles**.

5. In the Add Site System Roles Wizard, on the General page, click **Next**.

6. On the Proxy page, click **Next**.

7. On the System Role Selection page, note that the Reporting services point is unavailable as this has already been configured in the lab environment.

8. Click **Cancel**.

9. Under Site System Roles, right click the **Reporting services point** and select Properties.

    Note the settings used, the configration is a very simple process.

10. Open File Explorer, and then navigate to and open the **C:\Program Files\Microsoft Configuration Manager\Logs\srsrpsetup.log** file.

    This emulates how to you would monitor the reporting services point installation by using the srsrpsetup.log file.

## Task 3: Test the reporting services point in the Configuration Manager console
1. In the **Monitoring** workspace, expand **Reporting**, and then click **Reports**.

    Note: You might have to refresh the console until all reports display. You can also monitor the C:\Program Files\Microsoft Configuration Manager\Logs\srsrp.log file for status on the deployed reports. It will      take several minutes for the reports to be deployed.

2. Expand Reports, and then click **Users**.
3. Right-click the **Users** in a specific domain report, and then click **Run**.
4. In the Users in a specific domain window, click **Values**.
5. In the Parameter Value dialog box, click **ADATUM**, and then click **OK**.
6. In the Users in a specific domain window, click View Report.
7. Close the Users in a specific domain window, and then minimize the Configuration Manager console.

## Task 4: Test the reporting services point in the SQL Server Reporting Services website
1. Open Microsoft Edge. In the address bar, type http://LON-CFG/Reports, and then press Enter.
2. Click the **ConfigMgr_S01** link, and click the **Users** folder.
3. Click the **Count users by domain report**.View the results, and then close Internet Explorer.

Results: After this exercise, you should have installed and configured a reporting services point and tested it by opening reports in both the Configuration Manager console and the SQL Server Reporting Services (SSRS) website.
