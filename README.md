<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />



<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Item 1: Configure Roles 
- Item 2: Configure Departments
- Item 3: Configure Teams 
- Item 4: Configure Agents (Workers) 
- Item 5: Configure User (Customers)
- Item 6: Configure SLA
- Item 7: Configure Help Topics 

<h2>Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/zmBvL7W.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/kqtpQao.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Configured Roles: Roles are the permissions granted to Agents per Department that they have access to. Each Role has a set of permissions that can be checked/unchecked for agents given that Role in association with a Department they have access to. An unlimited number of roles can be created and assigned to Agents with access to various departments.
Admin Panel -> Agents -> Roles <br>
Supreme Admin 
</p>
<br />

<p>
<img src="https://i.imgur.com/lK2bn32.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/5FjD77V.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Using Admin Account click add department tab to create a new department.System Admi
Since tickets are routed through Departments in the help desk, there are many settings that can be set for each Department.
Admin Panel -> Agents -> Departments
System Admins 
</p>
<br />

<p>
<img src="https://i.imgur.com/TTZcu23.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
How to Create Teams In Your Help Desk

Teams allow you to pull Agents from different Departments and organize them to handle a specific issue or user via a Help Topic or Ticket Filter.

Having Agents from different Departments assigned to a Team will supersede the parameters of the Agents’ Department rules. For example, you can create a Help Topic associated with a particular product you produce, and assign it to a Team of specialist Agents from different Departments.

To create a Team in your Admin Panel, locate the Agents tab, and click on Teams. Then click Add New Team on the right, and fill out the appropriate information. Then you will be able to add Agents to the team by clicking on their name from your list of Agents and checking the corresponding box next to the Team name you wish to add them at the bottom of the page.

A Team can have an appointed leader who can receive Alerts & Notices separate from other team members. In order to set a Team Leader you can choose an Agent from the Team Lead dropdown when creating a Team or Editing an existing Team.

Create Teams: Admin Panel -> Agents -> Teams 
</p>
<br />

<p>
<img src="https://i.imgur.com/dZTbVsU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/tuPGOxz.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Agents are given access to the help desk with the intent to respond and resolve the tickets. When adding an Agent to the help desk, they will need to be assigned to a Primary Department and given a Primary Role for the Tickets/Tasks routed to that department. Agents can be given Extended Access to additional departments of the help desk as well as assigned different Roles to those departments; this can be configured in the Access tab of the Agent’s Profile.

Configure Agents: Admin Panel -> Agents -> Add New 
1. Jeremaih Finnissee
2. Melissa Finnissee 
</p>
<br />

<p>
<img src="https://i.imgur.com/V9uecd9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p> Added two new users <br>
1. John Mellow <br>
2. Kelly Bellows
</p>
<p>
Users can now create an account and log-in to create a ticket or check a ticket’s status. As always with osTicket, users or ticket creators are associated with their email address as the unique identifier of each user. The User Directory, located on the Agent Panel, allows agents to search tickets by user as well as create Organizations to associate the user to. Agents can be configured as internal Account Managers for tickets created by users of an Organization. 
</p>
<br />

<p>
<img src="https://i.imgur.com/PeLtUqN.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
SLA Plans or Service Level Agreements, are unlimited in osTicket. The purpose of the SLA Plan is to provide a length of time in which the help desk Administrator expects tickets to be closed.

Configure SLA: Admin Panel -> Manage -> SLA 
SEV - A (1hr, 24/7)
SEV - B (4hr, 24/7)
SEV - C (8hr, business hours)
</p>
<br />

<p>
<img src="https://i.imgur.com/fHXjT4V.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

</p>
<p>
Help Topics will help streamline your end-user’s help desk experience to ensure proper assignment and prompt response to the ticket. Create as many Help Topics as needed and can even nest Help Topics within each other for further breakdown (For example, Human Resources and Human Resources/Payroll.)

Help Topics will determine what Department the ticket is routed to which will determine which Agents have access to the ticket. The Help Topic also can determine other configurations of the ticket, such as the ticket’s SLA (or Service Level Agreement) and priority of a ticket, i.e. Emergency to Low.

There are two places where the Help Topic must be selected on New Tickets; the client portal and new tickets created internally by staff. When Users select the Help Topic, they are not aware of the configurations in place for that Help Topic.

Admin Panel > Manage > Help Topics > Add New Help Topic
</p>
<br />
