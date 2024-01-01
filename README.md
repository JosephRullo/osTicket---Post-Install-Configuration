<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Computer)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Configure Roles
- Configure Departments
- Configure Teams
- Configure Agents
- Configure Users
- Configure SLA
- Configure Help Topics

<h2>Configuration Steps</h2>

<h2>Step 1.</h2> We will begin the osTicket post intall configuration by logging on as the administrator we created in the previous install. This will bring you to the Admin Panel homepage. (Please click (https://github.com/josephrullo/osTicket-Prerequisites-and-Installation) for a full tutorial.)
<p>
<p>
<img src="https://imgur.com/26HKTmF.png" height="70%" width="70%" alt="Disk Sanitization Steps"/> <img src="https://imgur.com/dBwU7DL.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />


<h2>Step 2.</h2> Configuring Roles. Roles are the permissions granted to Agents per Department that they have access to. Each Role has a set of permissions that can be checked/unchecked for agents given that Role in association with a Department they have access to. Let's create a custom Role that we can assign to an Agent later on. From the Admin Panel homepage select the "Agents" tab -> Select "Roles" -> click on "Add New Role". Let's name this role "Supreme Admin" for this example and grant it all permissions. To do this go to the "Permissions" tab to the right and check all boxes in the Tickets/Tasks/Knowledgebase tabs. Note you can fully customize this "Role" with any specific title and permission access you may require for an agent. Optional: Add internal notes about role. Now click "Add Role".
<p>
<p>
<img src="https://imgur.com/jnPNXVS.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />

<h2>Step 3.</h2> Configuring Departments. Since tickets are routed through Departments in the help desk, there are many settings that can be set for each one. Here we will simply add a new Department with the default settings that we can adjust as neccessary later on. From the Admin Panel homepage select the "Agents" tab -> Select "Departments" -> click on "Add New Department". Let's name this Department "System Administrators" for this example. 
<p>
<p>
<img src="https://imgur.com/QWbKgcc.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />

<h2>Step 4.</h2> Configuring Teams. Teams allow you to pull Agents from different Departments and organize them to handle a specific issue or user via a Help Topic or Ticket Filter. From the Admin Panel homepage select the "Agents" tab -> Select "Teams" -> click on "Add New Team". Let's name this Team "Level II Support" for this example and leave the default settings for now.
<p>
<p>
<img src="https://imgur.com/nlFMFJv.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />

<h2>Step 5.</h2> Configuring Agents. Agents are given access to the help desk with the intent to respond and resolve the tickets. When adding an Agent to the help desk, they will need to be assigned to a Primary Department and given a Primary Role for the Tickets/Tasks routed to that department. Let's create two new Agents for this example. From the Admin Panel homepage select the "Agents" tab -> Select "Agents" -> click on "Add New Agent". Fill in the personal info fields, for this example I'll use Jane Doe and jane_doe@osTicket.com. Next create a "Username" ie. jane_doe. Click "Set Password" and uncheck the "Send agent a password reset email" so we can enter assign one directly. Uncheck "Require password change at next login" box and click "Set". With that set, we can now use the "Access" tab to assign a "Primary Department" and "Role" as discussed in previous steps. Next use the "Permissions" tab for grant or deny permissions. Finally use the "Teams" tab to add or remove them from any teams that were created. Click on "Create" when finished. I will create a second Agent named John Doe using the same steps.
<p>
<p>
<img src="https://imgur.com/1tP3l0h.png" height="70%" width="70%" alt="Disk Sanitization Steps"/> <img src="https://imgur.com/I01IN6c.png" height="70%" width="70%" alt="Disk Sanitization Steps"/> <img src="https://imgur.com/wmXSIQz.png" height="70%" width="70%" alt="Disk Sanitization Steps"/> <img src="https://imgur.com/PcYl460.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />

<h2>Step 6.</h2> Configuring User Settings. Before adding new Users, let's adjust the Authentication settings for either allowing anonymous users to create tickets or requiring them to be registered in the system before they can do so. Go to the Settings tab on the Admin Panel window -> Select Users -> In Authentication Settings check or uncheck the box labeled "Require registration and login to create tickets" according to your preference. In this example it will be checked.
<p>
<p>
<img src="https://imgur.com/GdPYIeQ.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />

<h2>Step 7.</h2> Adding New Users. Users are the ticket owners of the tickets in the help desk. When a ticket is created in the help desk, the user is associated with their email address in the User Directory of the help desk. To add a new User you must switch over to the Agent Panet by selecting it in the upper right corner. Once on the Agent Panel -> Select the User tab -> Click Add User -> Enter in their name and email. I will create two Users for this tutorial (ie. Karen A. karen@osTicket.com, Ken B. ken@osTicket.com) 
<p>
<p>
<img src="https://imgur.com/iU0HnNs.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />

<h2>Step 8.</h2> Registering Users. Since we required registration for Users to login and create tickets in Step 6, we will have to register the two we just added. Select the User and click on "Register" -> assign them a password -> click "Create Account".
<p>
<p>
<img src="https://imgur.com/mbJw419.png" height="70%" width="70%" alt="Disk Sanitization Steps"/> <img src="https://imgur.com/QEmwcgp.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />
