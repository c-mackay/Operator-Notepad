# Operator-Notepad
<p>&nbsp;</p>
<p>My employer recently deployed Microsoft 365 for all employees. However, the ONLY intended use for it is the company intranet. I saw a few interesting apps in the launcher and began exploring the Power Platform.</p>
<p>&nbsp;</p>
<p>I work in a manufacturing environment. This industry seems to have been left in the dark ages when it comes to modern, cloud based technology. Perhaps that can evolve.</p>
<p>&nbsp;</p>
<p>But.... I saw a way to improve upon a challenge that most similar environments face. Communication between shifts! This is an age-old struggle. Notes get mysteriously altered or "lost". This is where the idea for an app that handles it came from. Every workstation in the shop has a computer. So this was a realistic goal. But it would also work if a company used tablets.</p>
<p>&nbsp;</p>
<p>The app I came up with, Operators Notepad, seems to deal with the issues quite well. Operators can leave daily notes at whatever workstation they are assigned to. They can also look back at historical notes to get up to speed. Notes that have been saved are not editable! This is a feature, not a bug.</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>If the current User().FullName is listed in the "Managers" list, they get the ability to view notes by date, by workstation, and by individual employee. As well as add a note to an individual workstation that will show up for the operators at that workstation.</p>
<p>&nbsp;</p>
<p>Managers like this because, in the past, they had to go from workstation to workstation to read the daily notes. Now they can peruse everything from the comfort of their offices and be assured they won't miss a thing.</p>
<p>&nbsp;</p>
<p>The app uses 3 lists and a connection to Office 365 Users:</p>
<p>&nbsp;</p>
<p>If you're interested in using this, I've attached the files.</p>
<p>&nbsp;</p>
<ul>
<li><em>OperatorNotepadApp_20200912000411.zip</em> is the Exported app package.</li>
<li><em>OperatorNotepadAppProvisioner_20200911235826 (1).zip</em> is a Power Automate flow to create the necessary lists that are used by the app.</li>
</ul>
<p>To set it all up:</p>
<ol>
<li>Download&nbsp;<strong><em>OperatorNotepadApp_20200912000411.zip</em></strong> and &nbsp;<strong><em>OperatorNotepadAppProvisioner_20200911235826 (1).zip</em></strong></li>
<li>Go to flow.microsoft.com</li>
<li>Import the <strong><em>OperatorNotepadAppProvisioner_20200911235826 (1).zip</em></strong> into Power Automate</li>
<li>Make sure the flow is turned on and click Run. Enter the URL of the SharePoint site you want to deploy the lists to when prompted.</li>
<li>Go to make.powerapps.com</li>
<li>Click on the Apps tabs on the left hand rail</li>
<li>Click 'Import Canvas App' in the ribbon and browse to the <strong><em>OperatorNotepadApp_20200912000411.zip</em></strong></li>
<li>Open the app in edit mode.</li>
<li>Click the data connections tab and delete all of the SharePoint Data Connections in the app</li>
<li>Search for SharePoint and add in the new SharePoint lists in your tenant that you just provisioned</li>
<ol>
<li>Managers</li>
<li>Notes</li>
<li>Stations</li>
</ol>
</ol>
<p>This is my first attempt at sharing any of my projects. Feel free to give me questions and comments.</p>
