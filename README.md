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

- Item 1 Azure Virtual Machine (VM): A Windows 10 VM with 4 vCPUs named osticket-vm, configured with a username (labuser) and password (osTicketPassword1!) keep the password simple in order to remember it you will need it again. 
- Item 2 IIS Installation and Configuration: Install and enable IIS on Windows with the CGI feature, along with the necessary components like the PHP Manager for IIS and the Rewrite Module.
- Item 3 PHP Installation: Install PHP 7.3.8 (non-thread-safe version) into the C:\PHP directory and configure PHP with IIS using PHP Manager.
- Item 4 MySQL Installation: Install MySQL 5.5.62, configure it with the root username and password (root/root), and set up a new MySQL database called osTicket.
- Item 5 osTicket Installation Files: Unzip and set up the osTicket installation files in C:\inetpub\wwwroot, enable necessary PHP extensions (php_imap.dll, php_intl.dll, php_opcache.dll), and configure file permissions on ost-config.php before completing the osTicket setup in the browser.

<h2>Installation Steps</h2>

<p>
<img src=https://i.imgur.com/WnPl0Y9.png height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In this step, I created a Windows 10 Virtual Machine in Azure with 4 vCPUs, named osticket-vm, and configured it with the username labuser and password osTicketPassword1!. To connect to the VM, I retrieved its public IP address from the Azure portal and used it to establish a Remote Desktop connection. This VM will serve as the host environment for the osTicket installation.
</p>
<br />

<p>
<img src=https://i.imgur.com/6aIWWc5.png height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Within the osticket-vm, I downloaded the osTicket-Installation-Files.zip and unzipped it to the desktop, creating the "osTicket-Installation-Files" folder. These files will be used to install osTicket and its dependencies. I then installed and enabled IIS with the CGI feature by navigating to World Wide Web Services > Application Development Features and checking the CGI box. Next, I installed the PHP Manager for IIS and the Rewrite Module from the folder. Lastly, I created the C:\PHP directory to prepare for PHP installation.
</p>
<br />

<p>
<img src=https://i.imgur.com/jYTdn3x.png height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lastly I configured PHP 7.3.8 (non-thread-safe version) with IIS using the PHP Manager for IIS. Next, I installed MySQL 5.5.62, set it up with the root username and password (root/root), and created a new MySQL database called osTicket. I then unzipped the osTicket installation files into C:\inetpub\wwwroot, enabled the necessary PHP extensions (php_imap.dll, php_intl.dll, php_opcache.dll), and configured the file permissions on ost-config.php before completing the osTicket setup through the browser.
</p>
<br />
