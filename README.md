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
Prerequisites:

- Server Setup-Ensure a web server.
- Database Preparation-Verify PHP and Composer are installed.

<h2>Installation Steps</h2>

<p>

</p>
Step 1: Azure VM Setup
Create a Resource Group.
Establish a Windows 10 VM in the Resource Group with 2-4 vCPUs.
Allow the creation of a new Virtual Network (Vnet).

![image](https://github.com/Chas101/osticket-ex-prereqs/assets/153942150/db8319a2-618e-40b6-8aea-7135fe6efe52)


![image](https://github.com/Chas101/osticket-ex-prereqs/assets/153942150/d16191cf-a5af-41af-88de-771d63f4f0b7)


<p>

<br />

<p>

</p>
<p>
Step 2:
  Enable CGI and Common HTTP Features in IIS on the Windows VM.
Install IIS Management Console.
Download and install PHP Manager for IIS.
Download and install the Rewrite Module.
Set up C:\PHP and install PHP 7.3.8.
Install VC_redist.x86.exe.
Install MySQL 5.5.62 with a typical setup, choosing "Password1" as the password.

![image](https://github.com/Chas101/osticket-ex-prereqs/assets/153942150/0231b7ae-0ffe-4488-8d2f-370089dd368e)

![image](https://github.com/Chas101/osticket-ex-prereqs/assets/153942150/3804223e-9d1e-40bd-8947-857feaf928e0)

![image](https://github.com/Chas101/osticket-ex-prereqs/assets/153942150/65f81339-4e09-4cf7-9c1f-198928e1a4f2)

![image](https://github.com/Chas101/osticket-ex-prereqs/assets/153942150/493fa1c6-9aeb-4b56-bab1-5af2b1085913)

![image](https://github.com/Chas101/osticket-ex-prereqs/assets/153942150/24262764-b636-47d9-87fc-e7c0a05ea4a8)

![image](https://github.com/Chas101/osticket-ex-prereqs/assets/153942150/66e25645-f1ab-43d0-9ede-d38b495e6964)

![image](https://github.com/Chas101/osticket-ex-prereqs/assets/153942150/3817314f-f41d-451a-a435-ed7a9e4e4ea7)

![image](https://github.com/Chas101/osticket-ex-prereqs/assets/153942150/f70a7681-29c0-43b5-b622-ad22af78600d)

</p>
<br />

<p>


</p>
<p>
Step 3:
Open IIS as an Admin and register PHP.
Reload IIS (Stop and Start the server to check).
</p>
<br />

![image](https://github.com/Chas101/osticket-ex-prereqs/assets/153942150/ef90ff5a-6d2a-4a49-b1b0-eec782049e6e)

![image](https://github.com/Chas101/osticket-ex-prereqs/assets/153942150/9633a6be-234f-47e2-a522-a50cce7b6f3a)

![image](https://github.com/Chas101/osticket-ex-prereqs/assets/153942150/96bad6dd-0c0e-447f-b192-63ae0b8319b7)


<p>
Step 4:
Download osTicket and place the "upload" folder in c:\inetpub\wwwroot, renaming it to "osTicket."
Reload IIS.
Enable necessary PHP extensions in PHP Manager.
Rename ost-sampleconfig.php to ost-config.php.
Set permissions on ost-config.php.
Continue osTicket setup in the browser, specifying Helpdesk as the name and the default email for customer communication.
Download and install HeidiSQL.
In HeidiSQL, create a new session (root/Password1), connect to it, and create a database named "osTicket."
Complete osTicket setup in the browser, specifying MySQL Database as "osTicket," MySQL Username as "root," and MySQL Password as "Password1." Click "Install Now"

![image](https://github.com/Chas101/osticket-ex-prereqs/assets/153942150/e292c56b-2213-4ea5-b53e-d69319122f3d)

![image](https://github.com/Chas101/osticket-ex-prereqs/assets/153942150/9f1a06f9-b12d-4d31-ac5a-0fafc6eda846)

![image](https://github.com/Chas101/osticket-ex-prereqs/assets/153942150/fff90571-7ec8-4764-80e9-c6c1f47cfb20)

![image](https://github.com/Chas101/osticket-ex-prereqs/assets/153942150/e8bd226a-25a9-4435-a526-04174ea3509d)

![image](https://github.com/Chas101/osticket-ex-prereqs/assets/153942150/3e30bbdb-f5e2-4587-a129-6693b9ea5975)

![image](https://github.com/Chas101/osticket-ex-prereqs/assets/153942150/feade532-4594-4be9-833b-5e0716ea8513)

![image](https://github.com/Chas101/osticket-ex-prereqs/assets/153942150/13739bbd-7b61-4f3f-8bc1-621007eb92f4)

![image](https://github.com/Chas101/osticket-ex-prereqs/assets/153942150/5cfdbf4c-e271-45b4-9318-168468caffc1)

![image](https://github.com/Chas101/osticket-ex-prereqs/assets/153942150/f80ae4c9-e4fc-430b-bec0-db5319fcc3d9)

![image](https://github.com/Chas101/osticket-ex-prereqs/assets/153942150/65df8fad-0f0b-4c5e-8283-a2956c68ed70)

![image](https://github.com/Chas101/osticket-ex-prereqs/assets/153942150/7a449f5f-987b-4285-a815-839365628f81)
 
![image](https://github.com/Chas101/osticket-ex-prereqs/assets/153942150/a6929403-3d4b-4567-9fdc-afcd88494ee1)

