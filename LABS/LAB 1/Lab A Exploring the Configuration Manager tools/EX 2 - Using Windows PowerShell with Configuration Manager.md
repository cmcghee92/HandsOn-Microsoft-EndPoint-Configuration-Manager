# Exercise 2: Using Windows PowerShell with Configuration Manager

Scenario

In this exercise, you will use Windows PowerShell to determine information about Configuration Manager devices, distribution and management points, packages, applications, sites, users, and user and device collections.

The main tasks for this exercise are as follows:

View all commands related to Configuration Manager.
View Configuration Manager information.
## Task 1: View all commands related to Configuration Manager
1. In the Configuration Manager console, in the upper-left corner, click the Down Arrow, and then click Connect via Windows PowerShell.

2. When prompted in the Windows PowerShell window, on the keyboard, press A, and then press Enter.

3. To view all of the cmdlets in the Configuration Manager module for Windows PowerShell, at the Windows PowerShell command prompt, type the following command, and then press Enter:

4. ```PowerShell
Get-Command -Module ConfigurationManager | Out-Gridview
```
5. Review the commands, and close the Get-Command - Module ConfigurationManager | Out-Gridview dialog box.

## Task 2: View Configuration Manager information
To view a list of devices, in the Windows PowerShell window, type the following command, and then press Enter:

Get-CMDevice | ft Name, ADSiteName, SiteCode, DeviceOS
To view a list of distribution points, in the Windows PowerShell window, type the following command, and then press Enter:

Get-CMDistributionpoint
To view a list of management points, in the Windows PowerShell window, type the following command, and then press Enter:

Get-CMManagementPoint | ft NetworkOSPath, RoleName, SiteCode, RoleCount
To view a list of packages, in the Windows PowerShell window, type the following command, and then press Enter:

Get-CMPackage | ft Name, Description, PkgSourcePath
To view a list of applications, in the Windows PowerShell window, type the following command, and then press Enter:

Get-CMApplication | ft LocalizedDisplayName, SourceSite
To view a list of sites, in the Windows PowerShell window, type the following command, and then press Enter:

Get-CMSite | ft SiteName, SiteCode, ServerName
To view a list of users, in the Windows PowerShell window, type the following command, and then press Enter:

Get-CMUser | ft Name, Domain
To view a list of user collections, in the Windows PowerShell window, type the following command, and then press Enter:

Get-CMUserCollection | ft Name, Comment, MemberCount
To view a list of device collections, in the Windows PowerShell window, type the following command, and then press Enter:

Get-CMDeviceCollection | ft Name, Comment, MemberCount
Close the Administrator: Windows PowerShell window.

Results: At the end of this exercise, you will have used Windows PowerShell to determine information about Configuration Manager devices, distribution and management points, packages, applications, sites, users, and user and device collections.