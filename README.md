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

Step 1: Log in to the Admin Panel
</p>
Step 2: Configure Basic Settings
</p>
Step 3: Set Up Email
</p>
Step 4: Create Departments and Teams
</p>
Step 5: Create and Assign Agents
</p>
Step 6: Configure Help Topics
</p>
Step 7: Customize Ticket Fields and Forms
</p>
Step 8: Set Up Service Level Agreements (SLAs)
</p>
Step 9: Configure Auto-Responder and Alerts
</p>
Step 10: Perform System Backup


<h2>Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
After installing osTicket, the following configurations will help you set up the system for optimal performance and usability.

<h2>Step 1: Log in to the Admin Panel</h2>

1. Access the Admin Panel:
   - Open a web browser and navigate to your osTicket URL, typically `http://your-server-ip/osticket/scp`.
   - Log in using the admin credentials you set during installation.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<h2>Step 2: Configure Basic Settings</h2>

1. Navigate to Settings:
   - Go to the Admin Panel and click on the Settings tab.

2. Update Company Information:
   - System Settings: Update the company name, default email address, and system log settings.
   - General Settings: Set your helpdesk name, default department, and default priority.

3. Save Changes:
   - Click Save Changes to apply the new settings.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<h2>Step 3: Set Up Email</h2>

1. Configure Email Settings:
   - Go to Admin Panel > Emails > Settings.

2. Outgoing Email:
   - Add your SMTP details to enable outgoing email notifications.

3. Incoming Email:
   - Configure IMAP or POP settings to fetch emails from your support inbox.

4. New Email Address:
   - Add a new email address for your support team under Emails > Emails > Add New Email.
   - Fill in the required details and configure the mail fetching settings.

5. Save and Test:
   - Save your changes and test the email configuration to ensure it’s working correctly.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<h2>Step 4: Create Departments and Teams</h2>

1. Departments:
   - Navigate to Admin Panel > Agents > Departments.
   - Click on Add New Department.
   - Enter the department name, description, and email address (if different from the default).
   - Click Create Department.

2. Teams:
   - Navigate to Admin Panel > Agents > Teams.
   - Click on Add New Team.
   - Enter the team name and assign agents to the team.
   - Click Create Team.

</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<h2>Step 5: Create and Assign Agents</h2>

1. Create Agents:
   - Go to Admin Panel > Agents > Add New Agent.
   - Enter the agent’s details (name, email, username, etc.).
   - Assign the agent to the appropriate department and team.
   - Set the agent’s role and permissions.
   - Click Create Agent.

2. Agent Roles and Permissions:
   - Navigate to Admin Panel > Agents > Roles.
   - Create new roles or modify existing ones to define permissions for different agent levels.

</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<h2>Step 6: Configure Help Topics</h2>

1. Help Topics:
   - Go to Admin Panel > Manage > Help Topics.
   - Click on Add New Help Topic.
   - Enter the help topic name and configure any additional settings (e.g., auto-response).
   - Click Create Help Topic.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<h2>Step 7: Customize Ticket Fields and Forms</h2>

1. Ticket Fields:
   - Navigate to Admin Panel > Manage > Forms.
   - Click on the **Ticket Details** form to customize the fields that appear on the ticket creation form.
   - Add, remove, or modify fields as necessary.

2.Custom Forms:
   - Create custom forms if you need additional information from users when they submit tickets.
   - Click on Add Custom Form, enter form details, and add fields.
   - Save the form and link it to the help topics if needed.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<h2>Step 8: Set Up Service Level Agreements (SLAs)</h2>

1. SLAs:
   - Go to Admin Panel > Manage > SLA Plans.
   - Click on Add New SLA Plan.
   - Enter the SLA name, grace period, and business hours.
   - Assign the SLA to specific help topics or departments.
   - Click Create SLA Plan.

</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<h2>Step 9: Configure Auto-Responder and Alerts</h2>

1. Auto-Responder:
   - Navigate to Admin Panel > Settings > Autoresponder.
   - Enable/disable auto-responder for new tickets and ticket replies.
   - Customize the messages as needed.
   - Save your changes.

2. Alerts and Notices:
   - Go to Admin Panel > Settings > Alerts and Notices.
   - Configure the alerts for agents and users for various ticket events (e.g., new ticket, overdue ticket).
   - Save your changes.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<h2>Step 10: Perform System Backup</h2>

1. Backup Database:
   - Regularly backup your MySQL database using tools like phpMyAdmin or the `mysqldump` command.
 
2. Backup Files:
   - Ensure to back up the `osticket` directory and any uploaded files.
</p>
<br />

<h2>Conclusion:<h2>
By following these steps, you will have a fully configured osTicket system, ready to manage support tickets efficiently. Customize further based on your organization's specific needs and workflow requirements. This post-installation configuration ensures that your osTicket setup is tailored for optimal performance and usability.
