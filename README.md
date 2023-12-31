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


<h2>Step 2.</h2> Configuring Roles. Let's create a custom Role that we can assign to an Agent later on. From the Admin Panel homepage select the "Agents" tab -> Select "Roles" -> click on "Add New Role". Let's call name this role "Supreme Admin" for this example and grant it all permissions. To do this go to the "Permissions" tab to the right and check all boxes in the Tickets/Tasks/Knowledgebase tabs. Note you can fully customize this "Role" with any specific title and permission access you may require for an agent. Optional: Add internal notes about role. Now click "Add Role".
<p>
<p>
<img src="https://imgur.com/jnPNXVS.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>
</p>
<p>
</p>
<br />
