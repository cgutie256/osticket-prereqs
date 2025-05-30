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

- Create a virtual machine running windows 10

- Enable Internet Information Services

- Install PHP on virtual machine 

- Install the Rewrite Module 

- Install Microsoft Visual c++ redistrabutable

- Install MySQL

<h2>Installation Steps</h2>
<br />
<img src="https://github.com/user-attachments/assets/4f8d22dc-2697-4ad3-87fc-c0eaf8357561" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p>
Set up a virtual machine with Windows 10. Make sure it has at least 2 CPUs and 16 GB of RAM.


</p>
<p>
<br />
<img src="https://github.com/user-attachments/assets/a2a1f876-5143-4dba-906e-3957a229ff87" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p>
Go to Control Panel and turn on Internet Information Services. After that, expand the World Wide Web Services section, then go to Application Development Features and make sure the CGI option is checked. Once that’s done, hit OK


</p>
</p>
<br />
<br />
<img src="https://github.com/user-attachments/assets/c1900d07-a59c-4aa0-b983-44c36b78b76c" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p>
Install PHP Manager for IIS 


</p>
<p>
<br />
<br />
<img src="https://github.com/user-attachments/assets/dd68f339-21bc-48ce-8595-0ee9805475dc" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p>
Install Rewrite Module 


</p>
<p>
<br />
<br />
<img src="https://github.com/user-attachments/assets/2cb935af-be02-4323-8557-94934d715aa1" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<p>
Create the directory C:\PHP


</p>
<p>
<br />
<br />
<img src="https://github.com/user-attachments/assets/9c8a4c7c-f549-4465-bb8d-e0a802ab2392" height="80%" width="80%" alt="Disk Sanitization Steps">
<p>
Install Microsoft Visual C++ Redistrabutable 


</p>
<p>
<br />
<br />
<img src="https://github.com/user-attachments/assets/a2c0b57a-2e37-40a5-a2f5-b2e834a9b5ea" height="80%" width="80%" alt="Disk Sanitization Steps">
<p>
Install MySQL. Use the typical install option, and make sure you launch the MySQL Instance Configuration Wizard when it finishes.


</p>
<br />
<br />
<img src="https://github.com/user-attachments/assets/a6759635-1453-4834-a0d3-5e728d23bc0d" height="80%" width="80%" alt="Disk Sanitization Steps">
<p>
Setup your server using standard configuration 

  
</p>
<br />
<br />
<img src="https://github.com/user-attachments/assets/c1d7e90f-1ff0-4d9d-be3e-ccc15126ef86" height="80%" width="80%" alt="Disk Sanitization Steps">
<p>
Run IIS as an administrator

  
</p>
<br />
<br />
<img src="https://github.com/user-attachments/assets/ed37a292-fa41-4277-bff5-7bc9ad594103" height="80%" width="80%" alt="Disk Sanitization Steps">
<p>
Next, we’ll register PHP in IIS Manager. Just click "Register" and browse to wherever you saved PHP on your hard drive. Don’t forget to reload IIS when you’re done.


</p>
<br />
<br />
<img src="https://github.com/user-attachments/assets/021711e7-4a30-4393-ae59-d82213d1b2ce" height="80%" width="80%" alt="Disk Sanitization Steps">
<p>
Go ahead and extract the osTicket installation folder, then copy the upload folder into C:\inet\wwwroot.


</p>
<br />
<br />
<img src="https://github.com/user-attachments/assets/599e179c-96f3-479b-ae55-d23703cf5a5d" height="80%" width="80%" alt="Disk Sanitization Steps">
<p>
Rename the upload folder to osTicket then restart the ISS server 


</p>
<br />
<br />
<img src="https://github.com/user-attachments/assets/46dd667f-35b8-4172-ac5c-d42f8238862a" height="80%" width="80%" alt="Disk Sanitization Steps">
<p>
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
<p>
Jump back into IIS and double-click the PHP Manager icon in the osTicket folder. Then click Enable or disable an extension.


</p>
<br />
<br />
<img src="https://github.com/user-attachments/assets/7e8224fa-fadf-4f86-a0db-05b5a29539cc" height="80%" width="80%" alt="Disk
Sanitization Steps">
</p>
Enable the following extensions: php_imap.dll, php_intl.dll, and php_opcache.dll. Once that’s done, go ahead and restart your server.


</p>
<br />
<br />
<img src="https://github.com/user-attachments/assets/166e552d-9067-4117-9556-1537fe65e5aa" height="80%" width="80%" alt="Disk
Sanitization Steps">
Go back and refresh the browser with the osTicket installation page. You should see all green check marks—don’t worry about the last two if they’re not green, they’re not needed for this setup.


</p>
<br />
<br />



