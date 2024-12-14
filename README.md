<p align="center">
<img src="https://i.imgur.com/t8XMFgR.png" alt="osTicket logo"/>
</p>

<h1>Microsoft Azure - Network Protocol Group (NSG)</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines Windows & Linux)
- Remote Desktop
- Resource Group
- WiresShark
- Network Security Group

<h2>Operating Systems Used </h2>

- Windows 10</b>

<h2>List of Prerequisites</h2>

![image](https://github.com/user-attachments/assets/d5626510-e8d8-40e2-a7cb-5be00d00727e)
![image](https://github.com/user-attachments/assets/b11f16c7-e556-4c1b-bb59-79f63ff33592)
![image](https://github.com/user-attachments/assets/e501c462-b21e-42f3-a81d-354b568b1a68)
![image](https://github.com/user-attachments/assets/f1310512-8f48-4bab-8e8f-e710ea6dbfec)

<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/WdZREHh.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Using wireshark to capture network packets. Pinging from one computer to another which in this case; Windows PC to Linux PC. 
</p>
<br />

<p>
<img src="https://i.imgur.com/BlJhUPY.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Using PowerShell to ping other computer, to create traffic. This alows wireshark to capture network traffic between the two computers.
</p>
<br />

<p>
<img src="https://i.imgur.com/5Tk3aVo.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Creating a rule in NSG to deny ping from any source. Adding it to the top will make it the first priority to read. If it is second to read and SSH is first to read. Ping ight go through since it could be a default rule. This would let ping go through. Which we want to block ping and deny access.
</p>
<br />
