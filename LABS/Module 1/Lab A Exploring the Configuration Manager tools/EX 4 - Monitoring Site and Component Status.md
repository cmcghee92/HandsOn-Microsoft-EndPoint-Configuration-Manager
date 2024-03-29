# Exercise 4: Monitoring Site and Component Status

Scenario

Monitoring the Configuration Manager environment is an important daily task. In this exercise, you will use the Site Status and Component Status nodes to view status messages.

The main tasks for this exercise are as follows:

Examine the Site Status node.

View Site Status messages.

View Component Status messages.

## Task 1: Examine the Site Status node
1. Click the Site Status node.
2. Examine the Site Status node.

Note: All of the icons should have a green circle with a white check mark to indicate that they are okay. If there are any red circles with a white X (Critical), notify your instructor.

## Task 2: View Site Status messages
1. Under Site System Role, right-click the Site server role, click Show Messages, and then click All.

2. In the Status Messages: Set Viewing Period dialog box, retain the default settings, and then
click OK.

3. In Configuration Manager Status Message Viewer for , click View, and then click Filter.

4. In the Message ID: text box, type 5104, and then click OK.

5. Double-click the status message for the latest milestone from SMS_POLICY_PROVIDER.

6. Examine the status message, and write down the Process ID information.

7. To close the Status Message Details dialog box, click OK, and then close the Configuration Manager Status Message Viewer for .

## Task 3: View Component Status messages
1. Click the Component Status node, and examine the status of the components.

Note: If any of the components display a red circle with a white X, notify your instructor.

2. Right-click SMS_POLICY_PROVIDER, click Show Messages, and then click All.

I3. n the Status Messages: Set Viewing Period dialog box, retain the default settings, and then click OK.

Note the number of entries between the latest 5104 milestone and the previous 5104 milestone.

4. Double-click the latest 5104 status message, and examine the status message.

Note: This is the same status that you reviewed in the previous task.

5. To close the Status Message Details dialog box, click OK.

6. Close Configuration Manager Status Message Viewer for , and close the Configuration Manager console.

Results: At the end of this exercise, you should have examined the status messages for a site system and a component.
