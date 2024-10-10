<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>


osTicket - Post Installation Configuration

This tutorial outlines the post-installation process of the open-source help desk ticketing system, osTicket.

Environments and Technologies Used

	•	Microsoft Azure (Virtual Machines/Compute)
	•	Remote Desktop
	•	Internet Information Services (IIS)
	•	osTicket

Operating Systems Used

	•	Windows 10

Prerequisites --> <a href="https://github.com/simeonhawkins/osticket-prereqs"> osTicket-PreReqs </a>


	•	Be connected to the Windows VM via RDP.
	•	Logged into osTicket.

Objectives

In this tutorial, we will configure departments, teams, and users, and set up Service Level Agreements (SLAs) to simulate a help desk environment for our fictional support team.

Post-Installation Setup

Step 1: Configure Roles

<p align="center">
<img src="https://user-images.githubusercontent.com/128980344/232943697-18bb8084-f80c-41b3-9fa8-9e9588d7a4a2.png" height="80%" width="80%" alt="Configuring Roles"/>
</p>


	•	In the Admin Panel, navigate to Agents > Roles and add a new role.
	•	Name the role Head Admin and check all permissions under Tasks, Tickets, and Knowledgebase.

<p align="center">
<img src="https://user-images.githubusercontent.com/128980344/232943763-671290f1-45b1-495d-95db-c549f581cbb0.png" height="80%" width="80%" alt="Creating New Role"/>
</p>


Step 2: Set Up Departments

<p align="center">
<img src="https://user-images.githubusercontent.com/128980344/232943823-a03758e4-e326-435c-96bf-7403fadee06f.png" height="80%" width="80%" alt="Departments Setup"/>
</p>


	•	Go to Agents > Departments and add a new department named System Administrators.
	•	Create another department named Network Department.

<p align="center">
<img src="https://user-images.githubusercontent.com/128980344/232943944-6b09cea3-5d02-47f3-93fd-c70c17b15663.png" height="80%" width="80%" alt="Adding Departments"/>
</p>


Step 3: Create Teams

<p align="center">
<img src="https://user-images.githubusercontent.com/128980344/232943985-0f236a9f-385b-471f-b083-0061670c6d6e.png" height="80%" width="80%" alt="Creating Teams"/>
</p>


	•	Navigate to Agents > Teams and create a new team named Level 1 Support.
	•	Add another team named Level 2 Support.

Step 4: Allow Public Ticket Creation

<p align="center">
<img src="https://user-images.githubusercontent.com/128980344/232944022-4d6c4ada-5a80-4b01-a2b2-f98134d35270.png" height="80%" width="80%" alt="Allowing Public Ticket Creation"/>
</p>


	•	Go to Settings > Users > Settings.
	•	Under Authentication Settings, uncheck Registration Required to allow anyone to create a ticket.

<p align="center">
<img src="https://user-images.githubusercontent.com/128980344/232944060-efd81c4e-5fe1-451a-a830-c1079278d7f1.png" height="80%" width="80%" alt="User Settings"/>
</p>


Step 5: Add Agents

	•	Go to Agents > Add New Agent.

Create the following agents:

	1.	Jessica Vaner
	•	Email: JessV@osTicket.com
	•	Username: Jess_Vaner
	•	Password: Password12321
	•	Department: System Administrators
	•	Role: Head Admin
	•	Team: Level 2 Support

<p align="center">
<img src="https://user-images.githubusercontent.com/128980344/232944095-f17f7227-e48d-4288-b995-eeec162e8b29.png" height="80%" width="80%" alt="Creating Agent Jessica"/>
</p>


	2.	David Bale
	•	Email: DavidB@osTicket.com
	•	Username: David_Bale
	•	Password: Password12321
	•	Department: Network Department
	•	Role: Head Admin
	•	Team: Level 2 Support

<p align="center">
<img src="https://user-images.githubusercontent.com/128980344/232944406-918432bd-6d6b-42d1-a19b-3d4f5c32eb9d.png" height="80%" width="80%" alt="Creating Agent David"/>
</p>


Step 6: Create Users

	•	Switch to the Agent Panel.
	•	Go to Users > Add User.

Create the following users:

	1.	Greg Dosto
	•	Email: GregD@osTicket.com
	2.	Pele Toll
	•	Email: PeleT@osTicket.com

<p align="center">
<img src="https://user-images.githubusercontent.com/128980344/232944649-9004a251-6c26-4a4e-bb77-58a69cdfa3ed.png" height="80%" width="80%" alt="Adding Users"/>
</p>


Step 7: Configure SLAs (Service Level Agreements)

	•	Go to Manage > SLA and add three new SLA plans:

	1.	Sev-A (High Severity: Server Down)
	•	Schedule: 24/7
	•	Grace Period: 1 hour
	2.	Sev-B (Medium Severity: Long Loading Time)
	•	Schedule: 24/7
	•	Grace Period: 5 hours
	3.	Sev-C (Low Severity: Computer Running Slow)
	•	Schedule: Mon-Fri 8 AM - 5 PM
	•	Grace Period: 8 hours

<p align="center">
<img src="https://user-images.githubusercontent.com/128980344/232944690-75867d4b-3907-4e89-85c4-f5043872f81d.png" height="80%" width="80%" alt="SLA Configuration"/>
</p>


Step 8: Set Up Help Topics

	•	Go to Manage > Help Topics and add three topics:

	1.	Severe Outage
	2.	Connection Issue
	3.	Password Reset

<p align="center">
<img src="https://user-images.githubusercontent.com/128980344/232944699-bc0e55c1-7d57-4964-a0ac-c1360605b86d.png" height="80%" width="80%" alt="Help Topics"/>
</p>


Summary

This concludes the post-installation setup for osTicket. You are now read for the --> <a href="https://github.com/simeonhawkins/ticket-lifecycle"> NEXT STEP </a>
