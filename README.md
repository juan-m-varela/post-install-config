<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Configure osTicket, post-installation](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)
- HeidiSQL
- osTicket

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

<p>
<img src="https://i.imgur.com/XwhtKqH.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
First, we need to access the Admin Panel from the information we input from last tutorial. The link for the help desk login page for employees and admins is: http://localhost/osTicket/scp/login.php.

Once you are logged in, click "Admin Panel" at the top of the page.


</p>
<br />

<p>
<img src="https://i.imgur.com/5Qs6MDB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Navigate to the "Agents" blade, then click "Roles", then click "Add New", then type "Supreme Admin" in the Name: field, then go to the "Permissions" tab, then check all the boxes in each of the sections, then click "Add Role"
</p>
<br />

<p>
<img src="https://i.imgur.com/ZFBkt1G.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Configuring Departments...

Navigate to the "Agents" blade, then click "Departments", then click "Add New", then type "System Administrators" in the Name: field, then click "Create Dept"
</p>
<br />
