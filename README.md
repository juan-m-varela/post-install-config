<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />


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
Configuring Roles...

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

<p>
<img src="https://i.imgur.com/47w7g49.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Configuring Teams...

Navigate to the "Agents" blade, then click "Teams", then click "Add New", then type "Level II Support" into the Name: field, then click "Create Team"
</p>
<br />

<p>
<img src="https://i.imgur.com/lScbrGh.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Configuring Agents (workers)...

Navigate to the "Agents" blade, then click "Agents", then click "Add New", then type in "Jane Doe" into the Name: field, then enter an email address, then enter a user name, then click "Set Password"

After you click "Set Password", uncheck the box stating "Send the agent a password reset email", then uncheck the box stating "Require password change at next login", then enter "Password1" into the "New Password" field, then click "Set"
**Write down this information for later**

Then click the "Access" tab, then select "System Administrators" from the Primary Department tab, then select the "Supreme Admin" from the Role tab, then, select "Support" from the Extended Access tab, then click "All Access" then click "Permissions" and make sure every box is checked.

Then click the "Teams" tab, click "--Select Team--" then select "Level I Support", then click "Add", then add "Level II Support" as well, then click "Create"

</p>
<br />

<p>
<img src="https://i.imgur.com/IMFOoSU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Now we're going to add another agent

Navigate to the "Agents" blade, then click "Agents", then click "Add New", then type in "John Doe" into the Name: field, then enter an email address, then enter a user name, then click "Set Password"

After you click "Set Password", uncheck the box stating "Send the agent a password reset email", then uncheck the box stating "Require password change at next login", then enter "Password1" into the "New Password" field, then click "Set"
**Write down this information for later**

Then click the "Access" tab, then select "Support" from the Primary Department tab, then select the "All Access" from the Role tab

Then click the "Teams" tab, click "--Select Team--" then select "Level I Support", then click "Create"

</p>
<br />

<p>
<img src="https://i.imgur.com/VTVVMLC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Configuring Users (customers)...

Click "Agent Panel" to switch over to the agent panel, then click on the "Users" blade, then click "User Directory", then click "Add User", then enter an email address and full name for a user, then click "Add User"

Repeat this process to add a new user named "Ken Ken" with the email "ken@helpdesk.com"
</p>
<br />

<p>
<img src="https://i.imgur.com/vF4RMJk.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Configuring SLA (Service Level Agreements)

Click "Admin Panel" in the top right, then go to the "Manage" blade, then click "SLA", then click "Add New SLA Plan"

We will add 3 plans. Enter "Sev-A" into the Name: field, then enter "1" into the Grace Period: field, then select "24/7" from the Schedule: field, then click "Add Plan"

Click "Add New SLA Plan" then enter "Sev-B" into the Name: field, then enter "4" into the Grace Period: field, then select "24/7" from the Schedule: field, then click "Add Plan"

Click "Add New SLA Plan" then enter "Sev-C" into the Name: field, then enter "8" into the Grace Period: field, then select "Monday-Friday 8am-5pm with U.S. Holidays" from the Schedule: field, then click "Add Plan"


</p>
<br />

<p>
<img src="https://i.imgur.com/fr8zboq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Configuring Help Topics...

We will configure 4 new help topics.

Navigate to the "Manage" blade, then select "Help Topics", then click "Add New Help Topic", then enter "Business Critical Outage" in the Topic: field, then click "Add Topic"

Navigate to the "Manage" blade, then select "Help Topics", then click "Add New Help Topic", then enter "Personal Computer Issues" in the Topic: field, then click "Add Topic"

Navigate to the "Manage" blade, then select "Help Topics", then click "Add New Help Topic", then enter "Equipment Request" in the Topic: field, then click "Add Topic"

Navigate to the "Manage" blade, then select "Help Topics", then click "Add New Help Topic", then enter "Password Reset" in the Topic: field, then click "Add Topic"

Congratulations you have successfully configured osTicket and now we're ready to work on mock tickets and learn the ticket lifecycle.

Let's move on: https://github.com/juan-m-varela/ticket-lifecycle

</p>
<br />
