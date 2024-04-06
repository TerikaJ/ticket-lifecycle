<p align="center">
<img src="https://i.imgur.com/KzJbWRS.png" height="50%" width="50%" alt="osTicket logo"/>
</p>

<h1>osTicket - Ticket Lifecycle: Creation ---> Resolution</h1>

This demonstration outlines the lifecycle of a ticket from intake to resolution within the open-source help desk ticketing system "osTicket".

_<b>NOTE:</b> This demonstration uses materials created in the previous demonstration, ["Post-Installation Configuration"](https://github.com/terikaj/post-install-config)._

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machine)
- Microsoft Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)
- MacOS

<h2>Ticket Lifecycle Stages</h2>

- Intake - _(The creation of a ticket)_
- Assignment - _(Forwarding ticket and Customer Communication)_
- Working the Issue - _(Establishing a baseline and documenting the process)_
- Resolution - _(Closing the ticket)_

<h2>Lifecycle Stages</h2>

<h3>&#9312; Intake</h3>

_Our intake process will start by accessing the page where tickets are created; We are acting as the external user/customer:_
- Within the web browser (Microsoft Edge or Chrome), navigate to the End User Ticket Page (http://localhost/osTicket/).
- Click on "Open a New Ticket".
<p align=center>
<img width="750" alt="Screen Shot 2024-04-05 at 5 02 13 PM" src="https://github.com/TerikaJ/ticket-lifecycle/assets/136477450/4ee6057e-5ffe-463b-a1d8-aec913aa950f">
</p>

- Enter an Email Address and Full Name (this example uses **karen@osticket.com / Karen Karen**)
- Select any Help Topic or one that was created in the previous demo (this example uses **Business Critical Outage**).
- Type a quick Header and a short description under Issue Sumamry (anything can be typed for demonstration purposes).
- Once done, click "Create Ticket".
<p align=center>
<img width="750" alt="Screen Shot 2024-04-05 at 5 07 02 PM" src="https://github.com/TerikaJ/ticket-lifecycle/assets/136477450/282fc142-f51a-40b8-ada4-2da728b90506">
<img width="750" alt="Screen Shot 2024-04-05 at 5 08 42 PM" src="https://github.com/TerikaJ/ticket-lifecycle/assets/136477450/27b6805f-9d96-4a66-a668-eec8b4c7c2c7">
</p>

_Create a few more tickets with varying importance for demonstration purposes:_ 
<p align=center>
<img width="750" alt="Screen Shot 2024-04-05 at 5 11 52 PM" src="https://github.com/TerikaJ/ticket-lifecycle/assets/136477450/3e9f003c-cddf-4eda-8d4c-4399f664b02f">
<img width="750" alt="Screen Shot 2024-04-05 at 5 14 33 PM" src="https://github.com/TerikaJ/ticket-lifecycle/assets/136477450/7e4a6a6d-182c-4ead-bb76-c71d8476e311">
</p>
<hr>

<h3>&#9313; Assignment and Communication</h3>

_Tickets have been made! We'll now go into the Agent's perspective of their end:_
- On the web browser (Microsoft Edge), go to the Help Desk Login Page (http://localhost/osTicket/scp/login.php).
  - Log into the osTicket Help Desk using an Agent account (this example uses username **otuser** which is our **root** account by accident, but you can utilize **jane.doe / jane.doe@osticket.com**).
  - Once logged in, you now should see the created tickets from the customers.
- Click on any available ticket (this example selects **entire mobile online banking is down**).
<p align=center>
<img width="750" alt="Screen Shot 2024-04-05 at 5 16 03 PM" src="https://github.com/TerikaJ/ticket-lifecycle/assets/136477450/614f4174-9b69-4422-ba82-9023165774a0">
<img width="750" alt="Screen Shot 2024-04-05 at 5 17 00 PM" src="https://github.com/TerikaJ/ticket-lifecycle/assets/136477450/22054865-6822-493d-be13-e20f0645b228">
</p>

_As an Agent, we'll observe and configure information within this ticket._

_An event such as the entire mobile online banking being down is can have major impact on the company, potentially resulting in a loss of money and/or credibility. The severity on this ticket should be the highest, and will also be assigned to the departments/teams that are responsible for resolving this issue ASAP!_
- Set Priorty from Normal to the highest level (this example uses **Emergency**).
- Assign the ticket to a higher-tier department (this example uses **System Administrators**).
- Assign a specific person(s) the responsbility to manage this ticket (this example uses the current user, **Jane Doe**).
- Modify the SLA Plan from Normal to a higher level (this example uses **SEV-A**).
<p align=center>
<img width="895" alt="Screen Shot 2024-04-05 at 5 23 08 PM" src="https://github.com/TerikaJ/ticket-lifecycle/assets/136477450/d053e2b6-d721-416e-b1a6-8121e0791968">
<img width="609" alt="Screen Shot 2024-04-05 at 5 25 20 PM" src="https://github.com/TerikaJ/ticket-lifecycle/assets/136477450/9bab1136-e791-46ce-97bc-72a19fa37021">
<img width="610" alt="Screen Shot 2024-04-05 at 5 25 58 PM" src="https://github.com/TerikaJ/ticket-lifecycle/assets/136477450/129b200c-098f-4b36-824e-560bf2858ca8">
<img width="607" alt="Screen Shot 2024-04-05 at 5 26 39 PM" src="https://github.com/TerikaJ/ticket-lifecycle/assets/136477450/6bc9d3dd-dd0a-4ca6-bbae-d11b4be8ea7a">
<img width="606" alt="Screen Shot 2024-04-05 at 5 27 01 PM" src="https://github.com/TerikaJ/ticket-lifecycle/assets/136477450/9de79dfe-7e99-4ec4-ad73-f6300c3b705b">
</p>
<hr>

<h3>&#9314; Working the Issue</h3>

_As we observe the overview page, we can see every update taking place within the Ticket Thread. As an Agent, we can communicate under Post Reply to provide status updates to anyone viewing this ticket, also for providing accountability for the resolution of the ticket._
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

<h1><p align=center> Done! Good job!</p></h1>

<p align=right>Please delete & clean up your Azure resources when finished!<br>
If you're unsure of how to do this, please click <a href="https://github.com/terikaj/azure-begin">HERE</a>
</p>
