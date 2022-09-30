
---
title: "Teams AddIn Installation in Outlook Desktop Client"
date: 2022-09-30

content:

Challenge: Teams add in is not visible from the outlook meeting invite

Resolution steps:

Reference:  https://learn.microsoft.com/en-us/MicrosoftTeams/troubleshoot/meetings/resolve-teams-meeting-add-in-issues

Check the status of the add-in in Outlook:
If you still don't see the Teams Meeting add-in, make sure it's enabled in Outlook.

In Outlook, select File > Options.

In the Outlook Options dialog box, select the Add-ins tab.

Check whether Microsoft Teams Meeting Add-in for Microsoft Office is listed in the Active Application Add-ins list.

If the add-in is not listed in the list of active applications, and you see the Teams Meeting Add-in listed in the Disabled Application Add-ins list, select Manage > COM Add-ins and then select Go…

Select the checkbox next to Microsoft Teams Meeting Add-in for Microsoft Office.

Select OK on all the dialog boxes that are open and restart Outlook.

![image](https://user-images.githubusercontent.com/5275820/193177410-a49306dc-0554-4378-88ca-539ef022e260.png)

![image](https://user-images.githubusercontent.com/5275820/193177548-4d348faf-019a-4d85-85ec-37333ea6e990.png)

Above steps didnt work to add the addin. So, I have the follow the manual process

Follow the steps mentioned under "Fix the issue manually" in the reference page:

Command used:
%SystemRoot%\System32\regsvr32.exe /n /i:user %LocalAppData%\Microsoft\TeamsMeetingAddin\1.0.21063.3\x64\Microsoft.Teams.AddinLoader.dll

![image](https://user-images.githubusercontent.com/5275820/193173990-f6b8ad70-ea94-4a5a-824a-8c7ec5f0669f.png)
---
