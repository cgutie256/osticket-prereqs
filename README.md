# osticket-prereqs
<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />




<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

1.Enable interenet information services

2.Install web platform installer

3.Install my sequel and setup username and password 

4.Install c++ redistrabutable 

5.Configure permissions and install OS ticket

<h2>Installation Steps</h2>

<p>
<img src="https://github.com/user-attachments/assets/a2a1f876-5143-4dba-906e-3957a229ff87" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Install / Enable IIS in Windows WITH CGI
World Wide Web Services -> Application Development Features -> [X] CGI

</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/64eb1cbf-d841-4482-9c03-56e162b7004f" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
install PHP Manager for IIS (PHPManagerForIIS_V1.5.0.msi)

</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/9dfa9316-f483-42d4-8ab2-53986090c069" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
From the “osTicket-Installation-Files” folder, install MySQL 5.5.62 (mysql-5.5.62-win32.msi)
Typical Setup ->
Launch Configuration Wizard (after install) ->
Standard Configuration ->
Username: root
Password: root

</p>
<br />
<img src="https://github.com/user-attachments/assets/2ddf06d7-53f6-49a1-8416-0d41e842b75f" height="80%" width="80%" alt="Disk Sanitization Steps">/
<img src="https://github.com/user-attachments/assets/a15a708e-b7d2-4ee1-8abf-91f05895f47d" height="80%" width="80%" alt="Disk Sanitization Steps"/>

</p>
<p>
Assign Permissions: ost-config.php
Disable inheritance ->
Remove All
New Permissions -> Everyone -> All
