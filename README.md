<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Install osTicket with Prerequisites](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Enabling IIS in Windows Features
- Installing the prerequisite files
- Item 3
- Item 4
- Item 5

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
For the next step I have linked a google drive with neccessary files included.
  
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

  

 

</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
