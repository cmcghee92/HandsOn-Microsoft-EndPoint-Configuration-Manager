# Exercise 5: Reviewing log files by using the Configuration Manager Trace tool

Scenario

All the Configuration Manager components generate logs files in a standard text file format. You can read these log files in a traditional text reader such as Notepad. However, the Configuration Manager Trace Log tool provides some unique features that make it easier to read a log file. In this exercise, you will explore some of these features, and review the relationship of the log file to the status messages that you reviewed earlier.

The main task for this exercise is as follows:

Use the Configuration Manager Trace Log tool.
Prepare for the next module.
Task 1: Use the Configuration Manager Trace Log tool
On the taskbar, click the File Explorer icon.

Navigate to the C:\Program Files\Microsoft Configuration Manager\tools folder.

Right-click cmtrace.exe, and click Pin to Taskbar.

On the taskbar, click the Configuration Manager Trace Log Tool icon.

In the Configuration Manager Trace Log Tool, click File, and then click Open.

Scroll down, click the Policypv.log file, and then click Open.

Click Tools, and click Highlight. In the Highlight text box, type 5104, and then click OK.

Click Tools, and click Find. In the Find text box, type the Process ID that you recorded earlier, and then click Find.

To find the next entry, press the F3 key, and repeat until there are no more new responses.

Scroll up until you see the previous highlighted entry. Note the number of entries between the two milestones.

Question: How does the number of events between milestones compare to the number of events shown in the status message viewer?

Answer: Typically, there are more entries in the log file than in the status message viewer.

Click Tools, and click Filter.

In the Filter Settings dialog box, select the Filter when the Entry Text check box.

In the Filter when the Entry Text drop-down list box, click contains.

In the text box next to the Filter when the Entry Text drop-down list box, type the Process ID that you recorded earlier, and then click OK.

Close the Configuration Manager Trace Log tool.

Results: At the end of this exercise, you should have used the Configuration Manager Trace Log tool to review a component log file.
