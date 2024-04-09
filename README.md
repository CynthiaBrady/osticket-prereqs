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

- Azure Virtual Machine
- Internet Information Services (IIS)
- PHP Manager
- Rewrite Module
- VC Redist
- MySQL
- Heidi SQL
- osTicket v1.15.8
- Link to downloads:

<h2>Installation Steps</h2>
1.) First go to https://portal.azure.com/ to create a resource group and virtual machine.
For the vurtual machine you will need to use Windows 10 Pro, version 22H2 and for the size you will need at least 2vcpus and 16 gbs of memory.
After creating the virtual machine you will connect to the VM by using the same IP address as the vm was setup to connect with remote desktop app.
</p>
<br />

<p>
  
<p>

  
  <img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/52c26df6-a890-4068-9177-3cf6b5946b7a" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
 <img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/4798867e-b47e-42ae-b5e0-17eaa74b626e" height="80%" width="80%" alt="Disk Sanitization Steps"/> 

</p>




<p>


 


  <img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/7f11d9d3-9fa6-44e6-92a0-563dc37aa441" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

  2.)After pasting the IP address in remote desktop log in with the user name and password that you used when you created your VM.  </p>
<br />

<p>

  
  <img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/dd081a73-13a6-4de0-b590-ad259e89403d" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
3.) Once logged in the VM go to start menu, click run and type in control panel.  
</p>
<br />

<p>
<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/2085ba05-1b14-40eb-bd22-a4fa9bea5e55" height=" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
4.) From control panel click on programs. 
</p>
<br />


<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/bd5bac3a-28da-454e-aca1-4045a2b98637" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
5.) In programs you will click on Window features on or off.
</p>
<br />


<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/4def1848-cc74-4879-824e-7ea73503052f" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
6.)You will Install/Enable in Windows with CGI and Common HTTP Features.
 
-World Wide Web Services->Application Development Features->
  
 - [X]CGI
  
 - [X]Common HTTP Features (make sure all features are selected.)
</p>
<br />


<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/d266cc7b-d624-441c-ad61-509cc5e88fc2" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

</p>
<br />

<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/774b678b-8668-4b4a-a232-3ca8b8aa05fc" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
7.)To make sure ISS is installed you can open a web brower and type in 127.0.0.1 and the page should look like this. 
</p>
<br />

</p>
<br />


<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/5d16c692-1953-4a8f-9171-7d03a7f83e49" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
8.)From the Installation Files,download and install PHP Mananger for IIS (PHPManagerForIIS_V1/5.0.msi) To install go through the wizard install and complete the install. 
 
9.)From the Intallation Files, download Rewrite Module(rewrite_en-US.msi) right click and install.

10.)Create a folder in the C Drive named PHP

11.)From the Installation Files,download and PHP 7.3.8 (php-7.3.8-nts-Win32-VC15-X86.zip) and unzip the contents into C:\PHP

!! ATTENTION!! if this appears,close to "keep" the file:


<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/ff46864c-9eeb-4247-a41c-9033115f3ef1" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
12.)Once downloaded then you right click on the file and click extract all into folder PHP folder on the C drive.
</p>
<br />

</p>
<br />

<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/426a411e-4ea8-469b-aff4-688a02e4fee6" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
13.From the installation files download and intall VC_redist.x86.exe. Right click and go through the wizard.
</p>
<br />

14.From the intallation files download and install MySQL 5.5.62 (mysql-5.5.62-win32.msi)
  
   Run the setup wizard: Typical Setup->Launch Configuration Wizard ( after install) ->Standard Configuration->
   
<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/63b46af3-160a-460e-bb5d-cd8dd06bc9b8" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

  
</p>
<br />


<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/c2517379-def7-4f4c-8d90-a4316d513aa6" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

</p>
<br />


</p>
<br />

Make a new root password: Password1
</p>
<p>
<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/613026cf-b242-465d-ad85-9ba9850a343b" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Execute the process to the next page.
</p>
<br />


<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/36968d80-da5f-4be5-9134-21a415ffce7e" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
15. After all files are installed go to search bar and type IIS and right click IIS to run as administrator. The progarm page should look this. 
</p>
<br />


<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/152a884c-eca5-4cac-be13-cc642d91d05f" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
16. To register PHP double click on PHP Manager.
</p>
<br />


<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/6b45fa51-dec9-4875-b98f-99c232e74eb7" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
17.Click on Register new PHP version. 
</p>
<br />


<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/93d541f5-ea4a-45f9-b108-846c446987dc" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
18. Go to C Drive -> PHP -> click on PHP-cgi file. 
</p>
<br />


<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/51acac5d-3ecf-4efb-9028-f02b6f4fb943" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

</p>
<br />


<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/78bda78f-2c6c-418d-a2d4-055557cccdb8k" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
19.) Restart ISS server
</p>
<br />
  
  
<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/b90b01db-1fc5-4203-b47c-f85b47030f48" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
20.Download and Install osTicket v1.15.8- from installation Files.
  
  -Exract and copy the "upload" folder into the c:\inetpub\wwwroot
 
  -withen c:\inetpub\root, Rename "upload"to "osTicket"

  Reload IIS again.
</p>
<br />  
  
21.On IIS go to sites -> Default -> osTicket -On the right,click "Browser *:80"
</p>
<br />      
    
<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/364ea0a2-3392-4f72-97b5-7ba23f85a66c" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
22. You should see a page like this and that means osTicket is working. 

  Some extensions are not enabled,
</p>
<br />      
    
  
<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/2b2b3ef5-07e6-4ba3-a8e0-a665c92edb52" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
23. To enable the extenstions- Go back to IIS,sites->Default->osTicket-Double click PHP manager- Click "Enable or disable an extension"

   
</p>
<br />      
        
<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/b6b902b8-a1a0-4b24-a446-458386543729" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

<br />      
          
  
<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/b044645a-681d-40f8-85d5-ffe1c73f932c" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
24. Enable all three extensions:
 
  -Enable: php-imap.dll
  
  -Enable: php_intl.dll
 
  -Enable: php_opcache.dll

  Refresh the osTicket site in your browse,observe the changes
</p>
<br />        
  
  
<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/402cf2ee-8afd-4836-be36-635e71670b86" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

</p>
<br />          
  
<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/b660b284-3928-42ca-bcee-96bdb94c5ea0" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
25. After extensions are enabled in ISS we will go to rename one of the files in osTicket folder. 
  
  Open up C;\inetpub\wwwroot\osTicket\osticket\include\ost-config.php and rename the ost-sampleconfig.php to ost-config.php
</p>
<br />          
  
  
<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/430bb161-b1af-43c9-9ee9-46fc05c6509f" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p
</p>
<br />            
  
  <img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/1e5b08cc-6674-46ff-9409-717e9058803f" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
26. Now we are going to assign permissions right click, the file and go to properties.
  
  Then click on security,click on advance. 
  
</p>
<br />              
  
<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/46f65f8b-b73a-48ac-823b-b9f33df03b1a)"/>
</p>
<p>
27. Click on disable inheritance. 
</p>
<br />                
  
<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/006d4462-4dcf-43b5-bd42-73128f10607e"/>
</p>
<p>
28.Remove all inherited permissions from this object.
</p>
<br />                


<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/11df3a86-2688-4698-907f-f1747aeb2389"/>
</p>
<p>
29. Click add to add permissions. 
</p>
<br />                


<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/d914a294-d4ad-41a7-8d9c-9b4b3d7ccca3"/>
</p>
<p>
30. Select a principal and type in "Everyone" in the box. 
</p>
<br />                

<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/3ee9cea6-78bf-4d41-bb1f-5e4f6144dd63"/>
</p>
<p>
31.Click on Full Control so all the boxes are checked.
</p>
<br />                


<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/b3875262-2657-46b2-98d4-307cc46f9a06"/>
</p>
<p>
32.Click and apply.
</p>
<br />                


<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/a47720d3-7ea5-4a35-a92c-71a817e3aeef"/>
</p>
<p>
33.Now go over to the osTicket setup page and (click continue). Fill out the Systems settings and Admin User. Don't forget your chosen password.

  - Name HelpDesk

- Default email (receives email from customers)

34. To set up the database setting at the bottom of the page we need to download and install HeidiSQL from the installation files. 



</p>
<br />                


<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/ee2cae1b-a7df-4961-af88-7006111fc587"/>
</p>
<p>
35.Once the program is open we will create a new connection to the database. 
</p>
<br />                


<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/2bb124bf-ce31-4a30-820d-9101ffa59845"/>
</p>
<p>
36. For the username use root and for the password use Password1.
</p>
<br />                


<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/56fb426f-ec1f-41a0-ba61-cdf941571816"/>
</p>
<p>
37.Connected to the session and now we can go back to the finish setting up Database setting. In the Database Settings type in root for the username and Password1 for the password.
  
  Now we are going to create a new database in HiediSQL.

  Right click on "Unnamed" select "create new" then select "database'. 

  
</p>
<br />                


<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/f0b1c240-39b6-47e1-a4a7-acab53d4f6c1"/>
</p>
<p>

</p>
<br />                

 Name the new database osTicket 


<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/a3231ec9-dd90-45b4-a030-2c50c5fddada" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

 Go back to osTicket browser and type in osTicket in the MySQL Database box. 
 
  <img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/a30cae90-8b72-49e4-bba7-56a396237f5b" height="80%" width="80%" alt="Disk Sanitization Steps"/>

  
</p>
<br />              

38. You should be able to click intall now and should intall osTicket. 
</p>
<br />              


<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/0cf0ff62-a789-44e7-82ab-fec99824889b" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
42. The last step is to clean up. We are going to delete the setup folder only. 
  Go to C:\inetpub\wwwroot\osTicket\setup and only delete setup folder. 
 
  From there go to the include folder to ost-config.php to set the permissions back to "Read" only. 
</p>
<br />              


<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/d2c25227-e7a6-4f7e-8ae6-3afd26c16c2b" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

</p>
<br />              

<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/b51bb9a8-6e39-4a93-9667-89be0d816267" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/ee577375-b067-4063-9f00-0aa53caaf52c" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
43. After the permissons are set then we can test the osTicket by logining in.
</p>
<br />              


<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/46b3a8b4-d8dc-4af0-91e7-66894f9e31aa" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
44. You have now installed and setup osTicket!
</p>
<br />              


<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/64a3a309-0584-401c-ac75-db64e9149c41" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>



<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/46b3a8b4-d8dc-4af0-91e7-66894f9e31aa" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>









