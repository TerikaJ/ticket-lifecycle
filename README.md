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
<img width="750" alt="Screen Shot 2024-04-05 at 5 23 08 PM" src="https://github.com/TerikaJ/ticket-lifecycle/assets/136477450/d053e2b6-d721-416e-b1a6-8121e0791968">
<img width="750" alt="Screen Shot 2024-04-05 at 5 25 20 PM" src="https://github.com/TerikaJ/ticket-lifecycle/assets/136477450/9bab1136-e791-46ce-97bc-72a19fa37021">
<img width="750" alt="Screen Shot 2024-04-05 at 5 25 58 PM" src="https://github.com/TerikaJ/ticket-lifecycle/assets/136477450/129b200c-098f-4b36-824e-560bf2858ca8">
<img width="750" alt="Screen Shot 2024-04-05 at 5 26 39 PM" src="https://github.com/TerikaJ/ticket-lifecycle/assets/136477450/6bc9d3dd-dd0a-4ca6-bbae-d11b4be8ea7a">
<img width="750" alt="Screen Shot 2024-04-05 at 5 27 01 PM" src="https://github.com/TerikaJ/ticket-lifecycle/assets/136477450/9de79dfe-7e99-4ec4-ad73-f6300c3b705b">
</p>
<hr>

<h3>&#9314; Working the Issue</h3>

_As we observe the overview page, we can see every update taking place within the Ticket Thread. As an Agent, we can communicate under Post Reply to provide status updates to anyone viewing this ticket, also for providing accountability for the resolution of the ticket._
<p align=center>
<img width="750" alt="Screen Shot 2024-04-05 at 5 30 21 PM" src="https://github.com/TerikaJ/ticket-lifecycle/assets/136477450/e638c8fd-b6a8-4724-bcb2-4fd23f19d980">
</p>

- Under Post Reply, type in a random message to the customer.
- Keep the Ticket Status "Open (current)", since the issue isn't resolved.
- Click "Post Reply".
<p align=center>
<img width="750" alt="Screen Shot 2024-04-05 at 5 32 01 PM" src="https://github.com/TerikaJ/ticket-lifecycle/assets/136477450/1174a412-477e-4295-a311-fe67a3050277">
<img width="750" alt="Screen Shot 2024-04-05 at 5 34 19 PM" src="https://github.com/TerikaJ/ticket-lifecycle/assets/136477450/39ad198f-b054-4d5d-92d0-7fe1cda251ab">
</p>

_Similar to a virtual chat or messaging system, our message will be posted onto the thread. The thread will continue to be updated with dialogue or status changes while team members are working on the ticket's resolution._
<hr>

<h3>&#9315; Resolution</h3>

_Let's say the issue has been resolved:_
- Under Post Reply, type a random message giving final update on the ticket.
- Change the Ticket Status to "Resolved".
<p align=center>
<img width="750" alt="Screen Shot 2024-04-05 at 5 37 23 PM" src="https://github.com/TerikaJ/ticket-lifecycle/assets/136477450/0a6ad4c3-a9a4-460f-9c68-6cb5f01b5458">
<img width="750" alt="Screen Shot 2024-04-05 at 5 39 20 PM" src="https://github.com/TerikaJ/ticket-lifecycle/assets/136477450/2b347fd9-6e39-4cb0-8be0-3bd42aabfeaa">
</p>

_Once a ticket is resolved, it is now "closed"; It will disappear from the Open Tickets page._<br>
_You can find it under the "Closed" tab; You can also see how many tickets were closed within a certain time frame._
<p align=center>
<img width="750" alt="Screen Shot 2024-04-05 at 5 40 39 PM" src="https://github.com/TerikaJ/ticket-lifecycle/assets/136477450/147c590d-1c91-4aa4-8a1d-146e56720678">
</p>

- Continue to navigate through the remaining tickets and utilize your best judgement on Priorty levels, assignment to departments and teams, etc.
<p align=center>
<img width="899" alt="Screen Shot 2024-04-05 at 5 45 06 PM" src="https://github.com/TerikaJ/ticket-lifecycle/assets/136477450/cffdf219-97da-4ed9-93c6-4e5d46c7ea86">
<img width="902" alt="Screen Shot 2024-04-05 at 5 45 52 PM" src="https://github.com/TerikaJ/ticket-lifecycle/assets/136477450/0fe674cb-7a08-4b72-a758-0a1ed6eec8b9">
<img width="900" alt="Screen Shot 2024-04-05 at 5 47 22 PM" src="https://github.com/TerikaJ/ticket-lifecycle/assets/136477450/8ba0619a-10a0-408c-a21f-d6149690c209">
</p>
<hr>

<h1><p align=center> DONE! Good job! </p></h1>

<h2><p align=center>The Next Demonstration:<br><a href="https://github.com/terikaj/azure-network-protocols"> Wireshark Network Traffic Inspection </a></p></h2>

<p align=right>Please delete & clean up your Azure resources when finished!<br>
If you're unsure of how to do this, please click <a href="https://github.com/terikaj/azure-begin">HERE</a>
</p>


