<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png"/>
</p>

<h1> How to Install osTicket </h1>
This is an easy guide to installing a help desk ticketing system called osTicket.<br/>


<h2> Files You Need to Download</h2>

- ### [Download Now](https://drive.google.com/drive/u/2/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6) 📁

<h2> Software & Technologies Used</h2>

- Windows 10 (Build 19044)
- Microsoft Azure (Virtual Machines)
- Remote Desktop (RDP)
- Internet Information Services (IIS)

  <h2> Prerequisites </h2>

- Create a Virtual Machine in Azure
- Install osTicket v1.15.8
- Install HeidiSQL
- Install MySQL
- Install PHP
- install Microsoft Visual C++ Redistributable
  <h2>Steps</h2>
<h3 align="center">Create Virtual Machine in Azure</h3>
<br />
<p>
<h3 align="center">First, start by creating a Resource Group inside Azure.</h3>
<br />
</p>
<p>
	<img src="https://i.imgur.com/eBi5k2l.png" height="75%" width="100%" />
</p>
<p>
<h3 align="center">Now, create a Windows 10 Virtual Machine (VM), typically with 2-4 Virtual CPUs. For username and password, it can be anything as we'll be using this info to remote in with our main computer. When creating the Virtual Machine (VM), allow Azure to create a new Virtual Network (Vnet):</h3>
<br />
</p>
<p>
	<img src="https://i.imgur.com/dEF1c7h.png" height="75%" width="100%" />
</p>
<br />
<br />
<h3 align="center">Open your Remote Desktop Connection app on your computer and connect to your Virtual Machine that was created in Azure. </h3>
<br />
<p>
	<img src="https://github.com/Joeljjoseph1998/osticket-prereqs/assets/50834280/2e71fd86-4198-47aa-aa1a-d0aed1b8e0eb"/>
	

</p>
<br />
<br />
<h3 align="center">Now we need to install / Enable IIS in Windows. Go to your Search Bar > Type "Control Panel" > Click "Programs" > "Turn Windows features on or off" > Scroll down to "Internet Information Services (IIS).</h3>
<br />
<p>
	<img src="https://i.imgur.com/iB0DDRd.png" height="75%" width="100%" />
</p>
<br />
<br />
<h3 align="center">Once clicked, find the "Internet Information Services" expand it and then expand the "World Wide Web" tab. Afterward, expand the application Developer tab. Finally check the "CGI" button & press Ok. You will need CGI to download the PHP Manager. The PHP manager is a back-end web programming language that allows osTicket to run off a web browser.</h3>
<br />
<p>
  <img src="https://github.com/Joeljjoseph1998/osticket-prereqs/assets/50834280/a6af9c35-e10c-4d7e-b2c8-30ffbe128f08" height="75%" width="100%"/>
</p>
<br />
<h3 align="center">Install PHP Manager</h3>
<br />
<p>
<h3 align="center">Download the PHP manager file, and agree with all the terms. We've now downloaded the PHP manager into our operating system.</h3>
<p>
  <img src="https://github.com/user-attachments/assets/35c7fd05-68ee-46bf-b41e-a714e4e13d35"height="75%" width="100%"/>
</p>
<br />
<h3 align="center">Install Rewrite Module</h3>
<br />
<p>
<h3 align="center">Download the Rewrite Module file, agree with all the terms and it should now be installed onto the Computer.</h3>
<p>
  <img src="https://github.com/user-attachments/assets/9da5e091-6d3c-4f53-83f6-24f2a0a39573"height="75%" width="100%"/>
</p>
<br />
<h3 align="center">CREATE DIRECTORY C:\PHP</h3>
<br />
<p>
<h3 align="center"> Open File Explorer, type, "C:\" in the search bar, Right-click and create a new folder called, "PHP". Download php-7.3.8-nts-Win32-VC15-x86.zip from<a href="https://drive.google.com/drive/u/2/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6"> Files You Need to Download</a>, Extract it by going to where you download the file, Right-click the PHP 7.3.8 file and press extract to the PHP Folder you just created.
</h3>
<p>
  <img src="https://github.com/user-attachments/assets/ef71b49e-5bb9-456b-9edf-b586ae0b321d"height="75%" width="100%"/>
  <img src="https://github.com/user-attachments/assets/ef71b49e-5bb9-456b-9edf-b586ae0b321d"height="75%" width="100%"/>
</p>
<br />
<h3 align="center">VC_REDIST DOWNLOAD</h3>
<br />
<h3 align="center"> Download and install VC_Redist, Agree with any terms and agreements and finish installing.</h3>
</h3>
<p>
  <img src="https://github.com/user-attachments/assets/b9cf40e7-45fa-4e6d-802a-d7a805071de3"height="75%" width="100%"/>
</p>
<br />
<h3 align="center">DOWNLOAD MySQL </h3>
<h3 align="center"> Download and install MySQL, Agree with any terms and agreements up until you get to the password portion. Here you can create a username and password for the database that you'll be using to store the Ticket Information used in osTicket. 
<br />
<p>
  <img src="https://github.com/user-attachments/assets/6028ca14-61bf-41d0-8e3b-75bda25438c9"height="75%" width="100%"/>
  <img src="https://github.com/user-attachments/assets/4f6db40f-1ec5-4723-8513-43b9da29507d"height="75%" width="100%"/>
  <img src="https://github.com/user-attachments/assets/005ac52b-48ab-414f-8c6d-eb7da50ab043"height="75%" width="100%"/>
  <img src="https://github.com/user-attachments/assets/3a88b52d-594d-4d11-a601-d0d3929f9f4b"height="75%" width="100%"/>
<br />
  <img src="https://github.com/user-attachments/assets/0a5df7f6-72da-4c6a-ad5c-a9f4d820b106" height="75%" width="100%"/>
</p>
<br />
<h3 align="center">Open IIS as Admin</h3>
<br />
<p>
 <img src="https://github.com/user-attachments/assets/67d6ce5e-ab33-44f9-98f4-c4e7f8f80d7f"height="75%" width="100%"/>
</p> 
<br />
<h3 align="center">Register PHP from within IIS (PHP Manager -> C:\PHP\php-cgi.exe)
<br/>
<p>
 <img src="https://github.com/user-attachments/assets/70b2dbf8-9469-458d-a093-bebfab5fdb14"height="75%" width="100%"/>
 <img src="https://github.com/user-attachments/assets/f532b964-089a-4215-82cb-af3a3821eb3f"height="75%" width="100%"/> 
 <img src="https://github.com/user-attachments/assets/41455960-0fb2-4e5c-9279-4857d3fd6394"height="75%" width="100%"/>
 <img src="https://github.com/user-attachments/assets/0a8d2fa6-0e14-4346-a419-461179240359"height="75%" width="100%"/>
</p>
<br />
<h3 align="center"> Reload IIS (Open IIS, Stop and Start the server)
<br /> 
<p>
 <img src="https://github.com/user-attachments/assets/63e8c462-ec46-4ae8-a662-c51e64775ee8"height="75%" width="100%"/>
 <img src="https://github.com/user-attachments/assets/a6b7f87e-746b-4d21-8b15-25e21674601e"height="75%" width="100%"/>
</p>
<br />
<h3 align="center">Install osTicket v1.15.8</h3>
<br />
<p>
  Download osTicket (download from within lab files: link).
</p>
<p>
	Extract and copy the “upload” folder INTO c:\inetpub\wwwroot:
</p>
	<img src="https://i.imgur.com/0MUJLMU.png" height="75%" width="100%" />
	<img src="https://i.imgur.com/1h9goM8.png" height="75%" width="100%" />
<p>
	Within c:\inetpub\wwwroot, Rename “upload” to “osTicket”:
</p>
<p>
	<img src="https://i.imgur.com/pDikkgq.png" height="75%" width="100%" />
</p>
<br />
<br />
<p>
	Reload IIS(Open IIS, Stop and Start the server)as shown before. </h3>
</p>
<p>
	When done go on the right and click “Browse *:80”:
</p>
<p>
	<img src="https://github.com/user-attachments/assets/c1298e3e-467f-4270-a691-6a14681f19c1" height="75%" width="100%"/>
</p>
<br />
<br />
<h3 align="center">Enable Extensions in IIS: Note that some extensions are not enabled</h3>
<br />
<p>
	Go back to IIS, sites -> Default -> osTicket.
</p>
<p>
	Double-click PHP Manager:
</p>
<p>
	<img src="https://github.com/user-attachments/assets/18bc79c1-ed51-43f1-a32f-c27c4cd3f6f7" height="75%" width="100%" />
</p>
<p>
	Click “Enable or disable an extension”.
</p>
<p>
	Enable: php_imap.dll.
</p>
<p>
	Enable: php_intl.dll.
</p>
<p>
	Enable: php_opcache.dll:
</p>
<p>
	<img src="https://github.com/user-attachments/assets/68a9927e-4229-4031-b902-d2c543992e0b" height="75%" width="100%"/>
</p>
<br />
<br />
<h3 align="center">Refresh the osTicket site in your browser, observe the changes</h3>
<br />
<p>
	<img src="https://i.imgur.com/6iSNd4H.png" height="75%" width="100%" />
</p>
<br />
<br />
<h3 align="center">Rename</h3>
<br />
<p>
	From: C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php.
</p>
<p>
	To: C:\inetpub\wwwroot\osTicket\include\ost-config.php:
</p>
<p>
	<img src="https://github.com/user-attachments/assets/2816468f-f13d-484b-8734-2cb180897bbd" height="75%" width="100%" />
</p>
<br />
<br />
<h3 align="center">Assign Permissions: ost-config.php</h3>
<br />
<p>
	Disable inheritance -> Remove All:
</p>
<p>
	<img src="https://github.com/user-attachments/assets/2748780f-13bd-4fc2-85bd-3eba4a782c52" height="75%" width="100%" />
</p>
<p>
	New Permissions -> Everyone -> All:
</p>
<p>
	<img src="https://github.com/user-attachments/assets/50536df0-30b1-4110-85f2-d1e7d9580b05" height="75%" width="100%" />
</p>
<p>
	<img src="https://github.com/user-attachments/assets/80422b00-109b-4923-b66c-6e239c4b8379"height="75%" width="100%" />
</p>
<br />
<h3 align="center">Continue Setting up osTicket in the browser (click Continue)</h3>
<br />
<p>
	Name Helpdesk.
</p>
<p>
	Default email (receives email from customers):
</p>
<p>
	<img src="https://github.com/user-attachments/assets/f259e08d-2498-4469-acb6-7f9c21999042" height="75%" width="100%" />
	<img src="https://github.com/user-attachments/assets/1ab1a36c-90af-4b8d-b3e9-a8b6bf4d20d2" height="75%" width="100%" />
</p>
<br />
<br />
<h3 align="center">Download and Install HeidiSQL</h3>
<br />
<p>
	<img src="https://github.com/user-attachments/assets/7f980259-ac59-4f8e-97bb-3d543b986425" height="75%" width="100%" />
</p>
<p>
	Create a new session, root/Password1.
</p>
<p>
	Connect to the session:
</p>
<p>
	<img src="https://github.com/user-attachments/assets/74071101-f451-4251-9743-640af120ee86" height="75%" width="100%" "/>
</p>
<p>
	Create a database called “osTicket”:
</p>
<p>
	<img src="https://github.com/user-attachments/assets/5094205c-bc84-4416-8f62-1ebc39f08b25" height="75%" width="100%" />
	<img src="https://github.com/user-attachments/assets/5e653744-7042-4ef0-8aa5-63efcf50a736" height="75%" width="100%" />
</p>
<br />
<br />
<h3 align="center">Continue Setting up osTicket in the browser</h3>
<br />
<p>MySQL Database: osTicket</p>
<p>
	MySQL Username: root
</p>
<p>
	MySQL Password: Password1:
</p>
<p>
	<img src="https://github.com/user-attachments/assets/6ce4aa56-2a88-4851-9841-edd95c795e8c" height="75%" width="100%" />
</p>
<p>Click “Install Now!”</p>
<p>Congratulations, hopefully it is installed with no errors!</hp>
<p>
	<img src="https://github.com/user-attachments/assets/48f500ce-1609-44c6-b9fa-f3463c396472" height="75%" width="100%" />
</p>
<br />
<br />
<h3 align="center">Login to the osTicket Admin Panel (http://localhost/osTicket/scp/login.php)</h3>
<br />
<p>
	<img src="https://github.com/user-attachments/assets/a1867dd7-3626-46b2-b9de-33967d6109dc" height="75%" width="100%" />
</p>
<br />
<br />
<h3 align="center"> Congrats, You've Finished Installing osTicket.</h3>
