# Operator-Notepad

There are 2 files: 
•	OperatorNotepadApp_20200912000411.zip is the Exported app package.
•	OperatorNotepadAppProvisioner_20200911235826 (1).zip is a Power Automate flow to create the necessary lists that are used by the app.

To set it all up:
1.	Download OperatorNotepadApp_20200912000411.zip and  OperatorNotepadAppProvisioner_20200911235826 (1).zip
2.	Go to flow.microsoft.com
3.	Import the OperatorNotepadAppProvisioner_20200911235826 (1).zip into Power Automate
4.	Make sure the flow is turned on and click Run. Enter the URL of the SharePoint site you want to deploy the lists to when prompted.
5.	Go to make.powerapps.com
6.	Click on the Apps tabs on the left hand rail
7.	Click 'Import Canvas App' in the ribbon and browse to the OperatorNotepadApp_20200912000411.zip
8.	Open the app in edit mode.
9.	Click the data connections tab and delete all of the SharePoint Data Connections in the app
10.	Search for SharePoint and add in the new SharePoint lists in your tenant that you just provisioned 
  A.	Managers
  B.	Notes
  C.	Stations

This is my first attempt at sharing any of my projects. Feel free to give me questions and comments.
