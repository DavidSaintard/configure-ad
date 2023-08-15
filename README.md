<p align="center">
<img src="https://i.imgur.com/gF2sOQe.png" alt="Active Directory Logo"/>
</p>

<h1>Active Directory - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites/installation of the Windows Server based Active Directory.<br />



<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Powershell

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Windows Server Installation
- Network Configuration 
- Domain Name
- DNS Server
- Administrator Account

<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/otaGGI5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Created two Virtual Machines on Azure witin the same resource group.

First VM (DC-1) being the Domain Controller on the latest Windows Server. Windows Server 2022.

Created the second VM (Client-1) on the Windows 10 server.

</p>
<br />

<p>
<img src="https://i.imgur.com/HUgxV0b.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Established Domain Controller’s NIC Private IP address to be static.

To Ensure Connectivity between the client and Domain Controller
  
Login in to Client-1 with Remote Desktop and pinged DC-1’s private IP address with ping -t.

Connectivitity failed due to ICMPv4 networking rules being disabled.

Login to the Domain Controller to configure/enable ICMPv4 in on the local windows Firewall

Check back at Client-1 to see the ping succeed
</p>
<br />

<p>
<img src="https://i.imgur.com/BmNJMji.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Install Active Directory Domain Services

On the Domain Controller(DC-1)
  
Setup a new forest as mydomain.com

created a name domain name "mydomain.com"

  
</p>
<br />

<p>
<img src="hhttps://i.imgur.com/BmNJMji.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
