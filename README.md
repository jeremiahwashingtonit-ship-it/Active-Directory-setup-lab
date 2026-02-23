<h1>Installing Active Directory on Windows Server on Virtual Machine</h1>



<h2>Description</h2>
In this lab, we are going to deploy a Windows Server 2025 Virtual Machine on a Proxmox VE hypervisor to establish a functional Active Directory environment. After promoting the server to a Domain Controller, we will architect a hierarchical Organizational Unit (OU) structure for departments like IT, HR, and Sales to mimic a corporate network. To complete the project, we will provision user accounts and security groups within these OUs, implementing Role-Based Access Control and verifying domain connectivity through DNS..
<br />


<h2>Languages and Utilities Used</h2>

- <b>Virtualization: Proxmox VE </b> 
- <b>Operating System: Windows Server 2025</b>
- <b>Identity Management: Active Directory Domain Services (AD DS)</b>
- <b>Drivers: VirtIO Guest Tools for optimized VM performance</b>
   

<h2>Environments Used </h2>

- <b>Windows 11 Enterprise (21H2): Client workstation for domain joining and GPO testing </b> (21H2)
- <b>Windows Server 2025: Primary Domain Controller (DC) </b>

<h2>Program walk-through:</h2>

<p align="center">
Creating the virtual machine and setting the Windows Server 2025 and VirtIO drivers iso image: <br/>
<img src="https://i.imgur.com/OHQIN5s.png" height="80%" width="80%" alt="creating VM "/>
<br />
<br />
Installing the Windows Serevr 2025 OS :  <br/>
<img src="https://i.imgur.com/b8nUFSG.png" height="80%" width="80%" alt="installing OS"/>
<br />
<br />
Installing Active Directoy, Group Policy Managment and other need roles : <br/>
<img src="https://i.imgur.com/qwk9eSM.png" height="80%" width="80%" alt="instaling AD"/>
<br />
<br />
Promted the  server to a Domain Controler (DC) and created an AD domain(WashingtonLab.local) :  <br/>
<img src="https://i.imgur.com/jYproc2.png" height="80%" width="80%" alt="DC creation"/>
 <img src="https://i.imgur.com/dJ9gAac.png height="80%" width="80%" alt="DC creation "/>
<br />
<br />
  Creating Organizational Unit (OU) structure for departments like IT, HR, and Sales to mimic a corporate network  <br/>
<img src="https://i.imgur.com/Y0BeLpt.png" height="80%" width="80%" alt="OU creation"/>
<br />
<br />
Manually added Users to the IT Group:  <br/>
<img src="https://i.imgur.com/yZ177on.png" height="80%" width="80%" alt="Addinig user to IT"/>
<br />
<br />
Change IP from a dymanic to a static IP, that won't be released to the dhcp pool:  <br/>
<img src="https://i.imgur.com/icgnMSG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
