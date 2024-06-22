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
<img src="https://docs.osticket.com/en/latest/_static/images/osticket-supsys-black-white.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
After installing osTicket, the following configurations will help you set up the system for optimal performance and usability.

<h2>Step 1: Log in to the Admin Panel</h2>

1. Access the Admin Panel:
   - Open a web browser and navigate to your <a href="http://localhost/osTicket/scp/login.php">osTicket URL</a> within your Virual Machine by Azure
   - Log in using the admin credentials you set during installation.
</p>
<br />

<p>
<img src="https://eu-images.contentstack.com/v3/assets/blt69509c9116440be8/blt1aaa63824f407eb6/65f33037317981040a17a463/Team_RRHHEG.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
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
<img src="https://media.sproutsocial.com/uploads/2021/08/email-marketing-featured-image.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
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
<img src="https://blogin.co/uploads/images/teams-users.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
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
<img src="https://www.nycastings.com/wp-content/uploads/2017/08/shutterstock_477756436.jpg" height="70%" width="70%" alt="Disk Sanitization Steps"/>
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
<img src="https://kateraidt.com/wp-content/uploads/2018/12/hand-792920_1920.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<h2>Step 6: Configure Help Topics</h2>

1. Help Topics:
   - Go to Admin Panel > Manage > Help Topics.
   - Click on Add New Help Topic.
   - Enter the help topic name and configure any additional settings (e.g., auto-response).
   - Click Create Help Topic.
     <p>
   EXAMPLE:
     <p>
     Business Critical Outage
        <p>
     Personal Computer Issues
           <p>
     Equipment Request
              <p>
     Password Reset
</p>
<br />

<p>
<img src="https://d3h0owdjgzys62.cloudfront.net/images/9395/live_cover_art/thumb2x/conditional_ticket_v2_3.png" height="40%" width="40%" alt="Disk Sanitization Steps"/>
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
<img src="https://infraon.io/blog/wp-content/uploads/2023/02/Service-Level-Agreement-SLA-Learn-About-it-in-2023.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<h2>Step 8: Set Up Service Level Agreements (SLAs)</h2>

1. SLAs:
   - Go to Admin Panel > Manage > SLA Plans.
   - Click on Add New SLA Plan.
   - Enter the SLA name, grace period, and business hours.
   - Assign the SLA to specific help topics or departments.
   - Click Create SLA Plan.
     <p>
### Example : IT Support SLA
   <p>
Sev-A (1 hour, 24/7)
<p>
Sev-B (4 hours, 24/7)
   <p>
Sev-C (8 hours, business hours)
<p>

#### **Agreement Overview**
- **Parties Involved**: This SLA is between [Company Name] and [Client Name].
- **Effective Date**: [Start Date]
- **Review Date**: [Review Date]

#### **Service Description**
- **Service**: IT support and maintenance services.
- **Scope**: Includes hardware and software support, network management, and cybersecurity services.

#### **Performance Metrics**
- **Availability**: 99.9% uptime during business hours (9 AM - 6 PM, Monday to Friday).
- **Response Time**: Initial response within 30 minutes for critical issues, within 2 hours for high-priority issues, and within 4 hours for normal issues.
- **Resolution Time**: Critical issues resolved within 4 hours, high-priority issues within 8 hours, and normal issues within 24 hours.

#### **Responsibilities**
- **Service Provider**: Ensure all systems are operational, provide regular updates, and maintain security protocols.
- **Client**: Provide access to necessary systems and information, report issues promptly, and follow provided guidelines.

#### **Penalties**
- **Service Credits**: If uptime falls below 99.9%, the client is entitled to service credits amounting to 5% of the monthly fee for each percentage point below the target.


</p>
<br />

<p>
<img src="https://www.oxfordwebstudio.com/user/pages/06.da-li-znate/sta-je-autoresponder/sta-je-autoresponder.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
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
