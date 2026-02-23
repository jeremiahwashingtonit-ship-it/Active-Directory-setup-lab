<h1>Installing Active Directory on Windows Server on Virtual Machine</h1>



<h2>Description</h2>
In this lab, we are going to deploy a Windows Server 2025 Virtual Machine on a Proxmox VE hypervisor to establish a functional Active Directory environment. After promoting the server to a Domain Controller, we will architect a hierarchical Organizational Unit (OU) structure for departments like IT, HR, and Sales to mimic a corporate network. To complete the project, we will provision user accounts and security groups within these OUs, implementing Role-Based Access Control and verifying domain connectivity through DNS..
<br />


<h2>Languages and Utilities Used</h2>

- <b>Virtualization: Proxmox VE </b> 
- <b>Windows Server 2025</b>
- <b>VirtIO Drivers</b>
- <b>PowerShell</b> 

<h2>Environments Used </h2>

- <b>Windows 11 Enterprise </b> (21H2)
- <b>Server 2025 </b>

<h2>Program walk-through:</h2>

<p align="center">
Launch the utility: <br/>
<img src="https://i.imgur.com/62TgaWL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Select the disk:  <br/>
<img src="https://i.imgur.com/tcTyMUE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Enter the number of passes: <br/>
<img src="https://i.imgur.com/nCIbXbg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Confirm your selection:  <br/>
<img src="https://i.imgur.com/cdFHBiU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Wait for process to complete (may take some time):  <br/>
<img src="https://i.imgur.com/JL945Ga.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Sanitization complete:  <br/>
<img src="https://i.imgur.com/K71yaM2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Observe the wiped disk:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
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
