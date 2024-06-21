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


<h2>Installation Steps</h2>

<p>
<img src="https://github.com/NicholasNunezGit/Prerequisites-for-osticket/assets/172544736/d5150d03-385b-4a27-8307-b9ea7b0f286a" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
To being the installation process you need to turn on Windows features illustrated above. You turn will need to turn on the IIS Management Console, CGI, and Common HTTP Features.
</p>
<br />

<p>
<img src="https://github.com/NicholasNunezGit/Prerequisites-for-osticket/assets/172544736/f332508d-f20c-4853-8749-92a7c73f4ab0" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
For the next step I have linked a google drive containing the neccessary files to install osTicket. <a href="https://drive.google.com/drive/u/1/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6"/>
  
  Download and install PHP Manager for IIS (PHPManagerForIIS_V1.5.0.msi).
  
  Download and install Rewrite Module (rewrite_amd64_en-US.msi).
  
  <img src="https://github.com/NicholasNunezGit/Prerequisites-for-osticket/assets/172544736/7c30baa2-82c5-46d6-9d3d-2acf41852437"/>

  Before the next installion first create a folder named PHP in your C: drive.
  
  Download and unzip  PHP 7.3.8 into the PHP folder you just created.

  Download and install VC_redist.x86.exe

  Download and install MySQL 5.5.62 (mysql-5.5.62-win32.msi)
    During the installion you will choose the typical install process and continue to the next installer. 
    
  <img src="https://github.com/NicholasNunezGit/Prerequisites-for-osticket/assets/172544736/d393ca28-119f-40b9-9956-35794f63d625"/>
 
  When prompted choose standard configuration 

  <img src="https://github.com/NicholasNunezGit/Prerequisites-for-osticket/assets/172544736/dcf73415-2faf-484e-9667-fda25a706219"/>

  For this lab we will be using "Password1".
    
  <img src="https://github.com/NicholasNunezGit/Prerequisites-for-osticket/assets/172544736/06a2f406-f203-42a2-ba12-033e77d9aa36"/>

   You will now run ISS manager as administrator.

  <img src="https://github.com/NicholasNunezGit/Prerequisites-for-osticket/assets/172544736/58c5f052-f6fc-4252-8eb3-13430fd2d3bb"/>

  Next we will regiser our PHP version.
    To register you will find the php-cgi in the directory C:\PHP.

  <img src="https://github.com/NicholasNunezGit/Prerequisites-for-osticket/assets/172544736/1bf52ef2-db33-4d41-bc00-7f8d589653b5"/>

  Next we will stop and start our server.

  Download an extract osTicket v1.15.8 to the directory C:\inetpub\wwwroot.

  <img src="https://github.com/NicholasNunezGit/Prerequisites-for-osticket/assets/172544736/67e17ba1-ca3e-414f-9a88-a4d5be044f87"/>

  Once extracted you will rename “upload” to “osTicket”.

  Next you will stop and start your ISS server.

  <img src="https://github.com/NicholasNunezGit/Prerequisites-for-osticket/assets/172544736/b2565ab5-d155-4a55-ab43-26b229eca5c9"/>

  Next in the ISS manager click on sites>Default Web Site>osticket
    Then click on browse *80

  <img src="https://github.com/NicholasNunezGit/Prerequisites-for-osticket/assets/172544736/6c33487a-0b97-403a-9c5a-824a2a71fc0e"/>

  We will now install the missing extensions

  <img src="(https://github.com/NicholasNunezGit/Prerequisites-for-osticket/assets/172544736/24c0b143-b4db-464b-8115-491280141d95"/>

  You will open the PHP Manager and click Enable or Disable an extension
    Enable extensions "php_opcache.dll", "php_intl.dll", and "php_imap.dll"

  <img src="https://github.com/NicholasNunezGit/Prerequisites-for-osticket/assets/172544736/804d813d-086c-4de7-9f97-c74a4f83bf0c"/>
  
  Your osTicket setup screen should now look like this.

  <img src="https://github.com/NicholasNunezGit/Prerequisites-for-osticket/assets/172544736/4f4e799c-f774-4072-ba71-f2894ddd17ce"/>

  Next in the directory C:\inetpub\wwwroot\osticket\include we will rename "ost-sampleconfig.php" to "ost-config.php"

  <img src="https://github.com/NicholasNunezGit/Prerequisites-for-osticket/assets/172544736/ea647d7b-a356-4b38-9978-eef4c7a101a6"/>

  We will now change the permission settings of the "ost-config.php" 
    Right click on the "ost-config.php" file and got to properties.
    Go to the security tab and click on advanced.
    Click on change permissions and then Disable inheritance.

  <img src="https://github.com/NicholasNunezGit/Prerequisites-for-osticket/assets/172544736/5be77fec-c19d-410b-8e64-609ef10c66cd"/>

  Now we will add permisions.
  Click add and under basic permissions check mark Full control, Modify, Read & excecute, Read, and Write.
  Click select a principal and in the text box type "Everyone".

  Return to the osTicket setup page and click continue.

  <img src="https://github.com/NicholasNunezGit/Prerequisites-for-osticket/assets/172544736/3e84ab33-9556-4890-b53d-b2bfd459ad93"/>

  Now fill out System Settings and Admin Users section. Make sure to take note of the information you use we will be using it again.

  Next you will install "HeidiSQL_12.3.0.6589_Setup.exe".

  <img src="https://github.com/NicholasNunezGit/Prerequisites-for-osticket/assets/172544736/e7212135-f6b2-47b5-83c8-75f6c00a930b"/>

  After insallation launch and start a new session.
    For this I will be using Username:Root Password:Password1.
  
  <img src="https://github.com/NicholasNunezGit/Prerequisites-for-osticket/assets/172544736/2ed66e7e-a25f-4cdf-99d8-1731b0135091"/>

  Next click open and then right click on unnamed and go to create new> Database. We will name this osTicket.
  
  <img src="https://github.com/NicholasNunezGit/Prerequisites-for-osticket/assets/172544736/e6335b15-5620-4eb4-9bd9-a4122fb64c32"/>
 
  Next return to the osTicketSetup and use the username, password, and database information we just created in the Database Settings.

  Now click install now.

  <img src="https://github.com/NicholasNunezGit/Prerequisites-for-osticket/assets/172544736/d5e27bdc-fd90-44ef-8349-56d4071274e1"/>

  You should now see this screen and have successfully installed osTicket.

  Now you should change permissions of the "ost-config.php" to read only.

  Finally you should clean up left over the file located at C:\inetpub\wwwroot\osTicket\setup

  Congratulations you have completed installation of osTicket.

