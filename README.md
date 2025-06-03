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
- HeidiSQL
<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Create a virtual machine running Windows 10

- Enable Internet Information Services

- Install PHP on the virtual machine 

- Install the Rewrite Module 

- Install Microsoft Visual C++ redistributable

- Install MySQL

<h2>Installation Steps</h2>
<br />
<img src="https://github.com/user-attachments/assets/4f8d22dc-2697-4ad3-87fc-c0eaf8357561" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
Set up a virtual machine with Windows 10. Make sure it has at least 2 CPUs and 16 GB of RAM.


</p>
<p>
<br />
<img src="https://github.com/user-attachments/assets/a2a1f876-5143-4dba-906e-3957a229ff87" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
Go to Control Panel and turn on Internet Information Services. After that, expand the World Wide Web Services section, then go to Application Development Features and make sure the CGI option is checked. Once that’s done, hit OK.


</p>
</p>
<br />
<br />
<img src="https://github.com/user-attachments/assets/c1900d07-a59c-4aa0-b983-44c36b78b76c" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
Install PHP Manager for IIS.


</p>
<p>
<br />
<br />
<img src="https://github.com/user-attachments/assets/dd68f339-21bc-48ce-8595-0ee9805475dc" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
Install the Rewrite Module. 


</p>
<p>
<br />
<br />
<img src="https://github.com/user-attachments/assets/2cb935af-be02-4323-8557-94934d715aa1" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
Create the directory C:\PHP.


</p>
<p>
<br />
<br />
<img src="https://github.com/user-attachments/assets/9c8a4c7c-f549-4465-bb8d-e0a802ab2392" height="80%" width="80%" alt="Disk Sanitization Steps">
<br />
Install Microsoft Visual C++ Redistributable. 


</p>
<p>
<br />
<br />
<img src="https://github.com/user-attachments/assets/a2c0b57a-2e37-40a5-a2f5-b2e834a9b5ea" height="80%" width="80%" alt="Disk Sanitization Steps">
<br />
Install MySQL. Use the typical install option, and make sure you launch the MySQL Instance Configuration Wizard when it finishes.


</p>
<br />
<br />
<img src="https://github.com/user-attachments/assets/a6759635-1453-4834-a0d3-5e728d23bc0d" height="80%" width="80%" alt="Disk Sanitization Steps">
<br />
Set up your server using the standard configuration. 

  
</p>
<br />
<br />
<img src="https://github.com/user-attachments/assets/c1d7e90f-1ff0-4d9d-be3e-ccc15126ef86" height="80%" width="80%" alt="Disk Sanitization Steps">
<br />
Run IIS as an administrator.

  
</p>
<br />
<br />
<img src="https://github.com/user-attachments/assets/ed37a292-fa41-4277-bff5-7bc9ad594103" height="80%" width="80%" alt="Disk Sanitization Steps">
<br />
Next, we’ll register PHP in IIS Manager. Just click "Register" and browse to wherever you saved PHP on your hard drive. Don’t forget to reload IIS when you’re done.


</p>
<br />
<br />
<img src="https://github.com/user-attachments/assets/021711e7-4a30-4393-ae59-d82213d1b2ce" height="80%" width="80%" alt="Disk Sanitization Steps">
<br />
Go ahead and extract the osTicket installation folder, then copy the upload folder into C:\inet\wwwroot.


</p>
<br />
<br />
<img src="https://github.com/user-attachments/assets/599e179c-96f3-479b-ae55-d23703cf5a5d" height="80%" width="80%" alt="Disk Sanitization Steps">
<br />
Rename the upload folder to osTicket, then restart the ISS server. 


</p>
<br />
<br />
<img src="https://github.com/user-attachments/assets/46dd667f-35b8-4172-ac5c-d42f8238862a" height="80%" width="80%" alt="Disk Sanitization Steps">
<br />
Head over to the osTicket folder in IIS. Once you're there, click Browse *.80 (http) on the right-hand side.


</p>
<br />
<br />
<img src="https://github.com/user-attachments/assets/c803bd8a-c5d5-4b1f-94c0-6c2140475911" height="80%" width="80%" alt="Disk Sanitization Steps">
<p>
This will open the osTicket installation page in your default browser. Before we jump into the install, we need to take care of a few things first.


</p>
<br />
<br />
<img src="https://github.com/user-attachments/assets/c9308543-0dd1-4a79-9819-4aa421498fc8" height="80%" width="80%" alt="Disk
Sanitization Steps">
<br />
Return to IIS and double-click the PHP Manager icon in the osTicket folder. Then click Enable or disable an extension.


</p>
<br />
<br />
<img src="https://github.com/user-attachments/assets/7e8224fa-fadf-4f86-a0db-05b5a29539cc" height="80%" width="80%" alt="Disk
Sanitization Steps">
<br />
Enable the following extensions: php_imap.dll, php_intl.dll, and php_opcache.dll. Once that’s done, go ahead and restart your server.


</p>
<br />
<br />
<img src="https://github.com/user-attachments/assets/166e552d-9067-4117-9556-1537fe65e5aa" height="80%" width="80%" alt="Disk
Sanitization Steps">
</p>
Go back and refresh the browser with the osTicket installation page. You should see all green check marks—don’t worry about the last two if they’re not green, they’re not needed for this setup.


</p>
<br />
<br />
<img src="https://github.com/user-attachments/assets/773c2574-7548-4e3a-90cd-a219084ce683" height="80%" width="80%" alt="Disk
Sanitization Steps">
<br />
Open up the osTicket folder on your computer and go into the include folder. Find the file called ost-sampleconfig.php and rename it to ost-config.php.


</p>
<br />
<br />
<img src="https://github.com/user-attachments/assets/d84b7d15-cd10-477a-89ed-70f47cc2c09b" height="80%" width="80%" alt="Disk
Sanitization Steps">
<br />
Right-click the file and go to Properties. Under the Security tab, click the Advanced button. First, disable inheritance, then remove all the existing permissions.


</p>
<br />
<br />
<img src="https://github.com/user-attachments/assets/942bc020-4290-49c4-977b-1b4458a1cac2" height="80%" width="80%" alt="Disk
Sanitization Steps">
<br />
Add permissions to Everyone as the principal.


</p>
<br />
<br />
<img src="https://github.com/user-attachments/assets/809e9ede-1c67-4242-a863-efada9f34bfa" height="80%" width="80%" alt="Disk
Sanitization Steps">
<br />
Give full control to everyone. Click ok. Click apply, then click ok.


</p>
<br />
<br />
<img src="https://github.com/user-attachments/assets/9e23a8aa-891e-4a76-b49f-3bdc478cca5b" height="80%" width="80%" alt="Disk
Sanitization Steps">
<br />
Head back to the installation screen in your browser and fill out the first half of the setup page. Just make sure the admin email and the default email are two different addresses.


</p>
<br />
<br />
<img src="https://github.com/user-attachments/assets/d49e4310-798a-46e7-94f9-6fccbb47d264" height="80%" width="80%" alt="Disk
Sanitization Steps">
<br />
Next up, we’re gonna install HeidiSQL. Just go with all the default settings during the install, and make sure to launch it once it’s done.


</p>
<br />
<br />
<img src="https://github.com/user-attachments/assets/fe8e7dde-2839-4bd1-8875-3259382d5f47" height="80%" width="80%" alt="Disk
Sanitization Steps">
<br />
Connect to the SQL server created previously.


</p>
<br />
<br />
<img src="https://github.com/user-attachments/assets/38a69eb2-cb69-4928-ab85-c7b443d135b8" height="80%" width="80%" alt="Disk
Sanitization Steps">
<br />
Right-click the Unnamed section on the left column and create a new database called osTicket.


</p>
<br />
<br />
<img src="https://github.com/user-attachments/assets/bfffa257-8512-4a9e-90da-06dcb15788a9" height="80%" width="80%" alt="Disk
Sanitization Steps">
<br />
Enter the info from the osTicket database you just set up on the install page, then hit Install Now.


</p>
<br />
<br />
<img src="https://github.com/user-attachments/assets/997d4249-d640-4072-a42a-f1f8d0a5f758" height="80%" width="80%" alt="Disk
Sanitization Steps">
<br />
Installation is complete and succesful. 


</p>
<br />
<br />
<p>Admin/Analyst Login Page:</p>
<p><a href="http://localhost/osTicket/scp/login.php">http://localhost/osTicket/scp/login.php</a> </p>
<br />
<p>End Users osTicket URL:</p>
<p><a href="http://localhost/osTicket">http://localhost/osTicket</a> </p>

