<p align="center">
<img src="https://i.imgur.com/KzJbWRS.png" height="50%" width="50%" alt="osTicket logo"/>
</p>

<h1>osTicket - Ticket Lifecycle: Intake Through Resolution</h1>

This demonstration outlines the lifecycle of a ticket from intake to resolution within the open-source help desk ticketing system "osTicket".

_<b>NOTE:</b> This demonstration uses materials created in the previous demonstration, ["Post-Install Configuration"](https://github.com/JTYKolesar/post-install-config)._

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Ticket Lifecycle Stages</h2>

- Intake
- Assignment and Communication
- Working the Issue
- Resolution

<h2>Lifecycle Stages</h2>

<h3>&#9312; Intake</h3>

_We'll start by accessing the page where tickets can be created, as if we're an external user:_
- On the web browser (Microsoft Edge), go to the End User Ticket Page (http://localhost/osTicket/).
- Click on "Open a New Ticket".
<p align=center>
<img src="https://i.imgur.com/Udla59t.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

- Enter an Email Address and Full Name (this example uses **karen@osticket.com / Karen Karen**)
- Select any Help Topic or one that was created in the previous demo (this example uses **Business Critical Outage**).
- Type a quick Header and a short description under Issue Sumamry (anything can be typed for demonstration purposes).
- Once done, click "Create Ticket".
<p align=center>
<img src="https://i.imgur.com/40QD7AI.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/gg905UJ.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

_Create a few more tickets with varying importance for demonstration purposes:_ 
<p align=center>
<img src="https://i.imgur.com/gsYwMkX.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/Uh85P3N.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<hr>

<h3>&#9313; Assignment and Communication</h3>

_Tickets have been made! We'll now go into the Agent's perspective of their end:_
- On the web browser (Microsoft Edge), go to the Help Desk Login Page (http://localhost/osTicket/scp/login.php).
  - Log into the osTicket Help Desk using an Agent account (this example uses username **jane.doe / jane.doe@osticket.com**).
  - Once logged in, you should see the created tickets from the clients.
- Click on any available ticket (this example selects **entire mobile online banking is down**).
<p align=center>
<img src="https://i.imgur.com/IlBoq7U.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

_As an Agent, we'll observe and configure information of this ticket._

_Having the entire mobile online banking down is something that could have a major impact on the company, resulting in losing money. The severity on this should be higher and should be assigned to the departments/teams that can be responsible to resolve this issue ASAP!_
- Set Priorty from Normal to a higher level (this example uses **Emergency**).
- Assign to a higher-tier department (this example uses **System Administrators**).
- Assign a specific person(s) the responsbility to manage this ticket (this example uses the current user, **Jane Doe**).
- Modify the SLA Plan from Normal to a higher level (this example uses **SEV-A**).
<p align=center>
<img src="https://i.imgur.com/V8WJ5GJ.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/JR8XMOt.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/CvAfVuZ.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/Wk23cCI.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/QIbVd0K.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<hr>

<h3>&#9314; Working the Issue</h3>

_Observing the overview page, we can see every update happening within the Ticket Thread. As an Agent, we can communicate under Post Reply to bring status updates to anyone viewing this ticket or for conversational purposes regarding the issue at-hand._
<p align=center>
<img src="https://i.imgur.com/qtVIjs7.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

- Under Post Reply, type in a random message.
- Keep the Ticket Status to "Open (current)", assuming the issues isn't resolved.
- Click "Post Reply".
<p align=center>
<img src="https://i.imgur.com/P5tLSZ5.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/YvCnXJe.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

_Like a virtual chat or messaging system, your message will be sent and posted on the thread. The thread will constantly be updated with conversations back and forth, or status changes while working on the issue at-hand._
<hr>

<h3>&#9315; Resolution</h3>

_Let's say the issue has finally been resolved:_
- Under Post Reply, type in a random message stating a final update of the matter.
- Change the Ticket Status to "Resolved".
<p align=center>
<img src="https://i.imgur.com/e1Ac4aR.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/vkOXsXv.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

_Once a ticket is resolved, it is considered "closed", so it will disappear from the Open Tickets page._<br>
_You can find it under the "Closed" tab, where you can see how many was closed at a certain time frame._
<p align=center>
<img src="https://i.imgur.com/xw9gHmX.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

- Continue to go through the rest of the remaining tickets and use best judgement on their Priorty, assignment to departments and teams, etc.
<p align=center>
<img src="https://i.imgur.com/N68R5Y9.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<hr>

<h1><p align=center>(ﾉ^ヮ^)ﾉ*:・ﾟ✧ COMPLETE! ✧ﾟ・:*╰(^ヮ^╰)</p></h1>

<p align=right>DELETE **EVERYTHING!** IN AZURE TO SAVE CREDITS!<br>
If you don't know how to, click <a href="https://github.com/JTYKolesar/azure-start/blob/main/README.md#bonus-delete-all-resources-in-azure">HERE</a>
</p>
