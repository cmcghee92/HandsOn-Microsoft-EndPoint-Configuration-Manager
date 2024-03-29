# Exercise 5: Reviewing log files by using the Configuration Manager Trace tool

Scenario

All the Configuration Manager components generate logs files in a standard text file format. You can read these log files in a traditional text reader such as Notepad. However, the Configuration Manager Trace Log tool provides some unique features that make it easier to read a log file. In this exercise, you will explore some of these features, and review the relationship of the log file to the status messages that you reviewed earlier.

The main task for this exercise is as follows:

Use the Configuration Manager Trace Log tool.


## Task 1: Use the Configuration Manager Trace Log tool
1. On the taskbar, click the File Explorer icon.

2. Navigate to the C:\Program Files\Microsoft Configuration Manager\tools folder.

3. Right-click cmtrace.exe, and click Pin to Taskbar.

4. On the taskbar, click the Configuration Manager Trace Log Tool icon.

5. In the Configuration Manager Trace Log Tool, click File, and then click Open.

6. Scroll down, click the Policypv.log file, and then click Open.

7. Click Tools, and click Highlight. In the Highlight text box, type 5104, and then click OK.

8. Click Tools, and click Find. In the Find text box, type the Process ID that you recorded earlier, and then click Find.

9. To find the next entry, press the F3 key, and repeat until there are no more new responses.

10. Scroll up until you see the previous highlighted entry. Note the number of entries between the two milestones.

    ```
    Question: How does the number of events between milestones compare to the number of events shown in the status message viewer? 

    Answer: Typically, there are more entries in the log file than in the status message viewer.

11. Click Tools, and click Filter.

12. In the Filter Settings dialog box, select the Filter when the Entry Text check box.

13. In the Filter when the Entry Text drop-down list box, click contains.

14. In the text box next to the Filter when the Entry Text drop-down list box, type the Process ID that you recorded earlier, and then click OK.

15. Close the Configuration Manager Trace Log tool.

Results: At the end of this exercise, you should have used the Configuration Manager Trace Log tool to review a component log file.
