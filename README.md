<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>Configuring On-Premises Active Directory within Azure VMs</h1>
The objective of this project is to deploy and configure Active Directory Domain Services (AD DS) on a Windows Server Virtual Machine hosted in Microsoft Azure. This setup enables centralized management of users, computers, groups, and network resources in a domain environment.<br />



<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

Step 1: Deploy the Azure Virtual Machine

Create a Windows Server Virtual Machine in Microsoft Azure and connect to it using Remote Desktop (RDP).

Step 2: Install Active Directory Domain Services

Use Server Manager to install the Active Directory Domain Services (AD DS) role on the Windows Server.

Step 3: Configure the Domain Controller

Promote the server to a Domain Controller by creating a new Active Directory forest and configuring the domain settings.

Step 4: Verify the Active Directory Environment

Open Active Directory Users and Computers (ADUC) to verify the domain, create test users or organizational units (OUs), and confirm the domain is functioning correctly.

<h2>Deployment and Configuration Steps</h2>

<p>
<img width="1536" height="1024" alt="CD5DD651-7623-4E0F-B8B6-6675630A4D56" src="https://github.com/user-attachments/assets/a0774523-b798-41a1-bbcb-a6f75053085b" />

</p>
<p>
Step 1: Create and Prepare the Azure Virtual Machine

1. Create a Windows Server Virtual Machine in Microsoft Azure.
2. Assign a static private IP address.
3. Connect to the VM using Remote Desktop (RDP).
</p>
<br />

<p>
<img width="996" height="675" alt="Screenshot 2026-07-04 at 3 40 21 PM" src="https://github.com/user-attachments/assets/a7ca7b1b-f671-4c5d-b63c-0d50748580a2" />

</p>
<p>
Step 2: Install Active Directory Domain Services (AD DS)

1. Open Server Manager.
2. Select Add Roles and Features.
3. Install the Active Directory Domain Services (AD DS) role.
4. Restart the server if prompted.
</p>
<br />

<p>
<img width="1105" height="642" alt="Screenshot 2026-07-04 at 3 40 45 PM" src="https://github.com/user-attachments/assets/f78c527b-fbf2-4dfc-b54d-ed37343a93d5" />


<p>
Step 3: Promote the Server to a Domain Controller

1. Click Promote this server to a domain controller.
2. Select Add a new forest.
3. Enter the domain name (e.g., company.local).
4. Configure the DSRM password.
5. Complete the installation and restart the server.
<br />

<img width="1025" height="684" alt="Screenshot 2026-07-04 at 3 41 36 PM" src="https://github.com/user-attachments/assets/f4f62cd8-4731-4c09-8e68-338fb072b15a" />


<p>
Step 4: Verify the Active Directory Configuration

1. Open Active Directory Users and Computers (ADUC).
2. Verify that the new domain has been created.
3. Create a test Organizational Unit (OU) and user account.
4. Confirm that Active Directory is functioning correctly.
<br />
