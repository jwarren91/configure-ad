<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>On-premises Active Directory Deployed in the Cloud (Azure)</h1>
This tutorial outlines the implementation of on-premises Active Directory within Azure Virtual Machines.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- Setup Resources in Azure
- Install Active Directory
- Creade an admin and normal user account in Active Directory
    - Joint client 1 to the domain
- Setup remote desktop for non-admin users on Client 1

<h2>Deployment and Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/VLJOGNL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Set up two virtual machines in Azure. One virtual machine will be your Domain Controller and the other will be your "client".
</p>
<br />

<p>
<img src="https://i.imgur.com/Yv4SW1o.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Install active directory in your Domain Controller (DC-1) Virtual Machine
</p>
<br />

<p>
<img src="https://i.imgur.com/2tOObf4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Created admin in active directory "Jane_admin" was the example. Used the command to ask "whoami" to verify that teh admin was created properly.
</p>
<br />

<p>
<img src="https://i.imgur.com/4GNoxN2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Here is where I set up remote desktop for "users" in powershell ISE as an admin. I gave them all passwords as well.
</p>
<br />
