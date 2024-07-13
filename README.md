<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This lab demonstration outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />



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
1. Begin by visiting https://portal.azure.com/ to establish a resource group and set up a virtual machine.
Ensure the virtual machine meets the specifications of Windows 10 Pro,version 22H2, with a minimum configuration of 2vCPUs and 16 GB of memory. Once the virtual machine is created, connect to it using the assigned IP address through the Remote Desktop application.  
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

  2.After entering the IP address in Remote Desktop, log in with the username and password you set up when creating your VM. </p>
<br />

<p>

  
  <img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/dd081a73-13a6-4de0-b590-ad259e89403d" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
3. Once you're logged into VM, go to Start menu, click on "Run" and enter "control panel".  
</p>
<br />

<p>
<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/2085ba05-1b14-40eb-bd22-a4fa9bea5e55" height=" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
4. From the Control Panel, navigate to "Program."
</p>
<br />


<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/bd5bac3a-28da-454e-aca1-4045a2b98637" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
5. In the Programs section,click on Turn Windows features on or off."
</p>
<br />


<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/4def1848-cc74-4879-824e-7ea73503052f" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
6.To install or enable CGI and Common HTTP Features in Windows:
 
  Navigate to World Wide Web Services->Application Development Features->
     
      
  Check the box for CGI and Common HTTP Features in Windows:
 - [X]CGI
  
 - [X]Common HTTP Features (ensure all features are selected).
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
7. To verify that ISS is installed,open a web browser and enter 127.0.0.1 the page should appear like this. 
</p>
<br />

</p>
<br />


<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/5d16c692-1953-4a8f-9171-7d03a7f83e49" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
8. Download PHP Mananger for IIS from the Installation Files (PHPManagerForIIS_V1/5.0.msi). Follow the wizard to install and complete the installation. 
 
9. Download the Rewrite Module from the installation Files (rewrite_en-US.msi). Right-click to install.

10.Create a folder named PHP on the C Drive. 

11.Download PHP 7.3.8 (php-7.3.8-nts-Win32-VC15-X86.zip) from the installation Files and extract its contents into C:\PHP

NOTE : If prompted, select "Keep" to proceed with the file download.


<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/ff46864c-9eeb-4247-a41c-9033115f3ef1" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
12.After downloading, right click the file and select "Extract All" into the PHP folder on the C drive.
</p>
<br />

</p>
<br />

<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/426a411e-4ea8-469b-aff4-688a02e4fee6" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
13.Download VC_redist.x86.exe from the installation files and install it by right-click and follow the wizard.
</p>
<br />

14.Download MySQL 5.5.62 (mysql-5.5.62-win32.msi) from the installation files and intall it. 
  
   Run the setup wizard: Typical Setup, then Launch Configuration Wizard after installtion, and select Standard Configuration.
   
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

Create a new root password: Password 1
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
15. Once all files are installed, open the search bar and type "IIS." Right-click on IIS and select "Run as administrator." 
  The program page should appear like this. 
</p>
<br />


<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/152a884c-eca5-4cac-be13-cc642d91d05f" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
16. To register PHP, double click on PHP Manager.
</p>
<br />


<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/6b45fa51-dec9-4875-b98f-99c232e74eb7" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
17.Click on 'Register new PHP version." 
</p>
<br />


<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/93d541f5-ea4a-45f9-b108-846c446987dc" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
18. Navigate to C Drive-> PHP, and click on PHP-cgi file. 
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
19.) Restart the IIS server.
</p>
<br />
  
  
<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/b90b01db-1fc5-4203-b47c-f85b47030f48" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
20.Download and install osTicket v1.15.8- from installation files.
  
  -Exract the contents of the"upload" folder and copy them into the C:\inetpub\wwwroot.
 
  -Withen C:\inetpub\root, rename the "upload" folder to "osTicket".

  Reload IIS once more.
</p>
<br />  
  
21.Navigate to IIS, then go to Sites -> Default -> osTicket. On the right-hand side, click on "Browser *:80".
</p>
<br />      
    
<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/364ea0a2-3392-4f72-97b5-7ba23f85a66c" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
22. You should see a page like this, indicating that osTicket is operational. 

  Note some extensions may not be enabled.
</p>
<br />      
    
  
<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/2b2b3ef5-07e6-4ba3-a8e0-a665c92edb52" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
23. To enable extenstions,- return to IIS, navigate to Sites->Default->osTicket. Double-click PHP manager, then click on "Enable or disable an extension."

   
</p>
<br />      
        
<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/b6b902b8-a1a0-4b24-a446-458386543729" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

<br />      
          
  
<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/b044645a-681d-40f8-85d5-ffe1c73f932c" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
24. Enable the following three extensions:
 
  -Enable: php-imap.dll
  
  -Enable: php_intl.dll
 
  -Enable: php_opcache.dll

  After enabling these extensions, refresh the osTicket site in your browse and observe the changes.
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
25. After enabling extensions in ISS, proceed to rename a file in osTicket folder. 
  
  Navigate to C:\inetpub\wwwroot\osTicket\osticket\include\ and rename the ost-sampleconfig.php to ost-config.php
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
26. Now. let's assign permissions by right clicking the file and selecting Properties.
  
  Next, click on Security, then select Advanced. 
  
</p>
<br />              
  
<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/46f65f8b-b73a-48ac-823b-b9f33df03b1a)"/>
</p>
<p>
27. Click on "Disable inheritance." 
</p>
<br />                
  
<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/006d4462-4dcf-43b5-bd42-73128f10607e"/>
</p>
<p>
28.Remove all permissions inherited from this object.
</p>
<br />                


<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/11df3a86-2688-4698-907f-f1747aeb2389"/>
</p>
<p>
29. Click on "Add" to include permissions. 
</p>
<br />                


<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/d914a294-d4ad-41a7-8d9c-9b4b3d7ccca3"/>
</p>
<p>
30. Select a principal and enter "Everyone" in the box. 
</p>
<br />                

<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/3ee9cea6-78bf-4d41-bb1f-5e4f6144dd63"/>
</p>
<p>
31.Click on "Full Control" to insure all the boxes are checked.
</p>
<br />                


<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/b3875262-2657-46b2-98d4-307cc46f9a06"/>
</p>
<p>
32.Click "Apply" to apply the changes.
</p>
<br />                


<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/a47720d3-7ea5-4a35-a92c-71a817e3aeef"/>
</p>
<p>
33.Now, navigate to the osTicket setup page and click on "Continue". Fill out the Systems settings and Admin User details. Don't forget your chosen password.

  - Name HelpDesk

- Default email (receives email from customers):[Your email address]

34. To configure the database setting at the bottom of the page, download and install HeidiSQL from the installation files. 



</p>
<br />                


<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/ee2cae1b-a7df-4961-af88-7006111fc587"/>
</p>
<p>
35.Once the program is launched, we'll establish a new connection to the database. 
</p>
<br />                


<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/2bb124bf-ce31-4a30-820d-9101ffa59845"/>
</p>
<p>
36. For the username, use "root" and for the password use "Password1".
</p>
<br />                


<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/56fb426f-ec1f-41a0-ba61-cdf941571816"/>
</p>
<p>
37.We are now connected to the session, so we can proceed to complete the Database settings. In the Database Settings, enter "root" for the username and "Password1" for the password.
  
  Next, let's create a new database in HiediSQL.

  Right-click on "Unnamed", select "Create New",and then select "Database'. 

  
</p>
<br />                


<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/f0b1c240-39b6-47e1-a4a7-acab53d4f6c1"/>
</p>
<p>

</p>
<br />                

 Name the new database 'osTicket". 


<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/a3231ec9-dd90-45b4-a030-2c50c5fddada" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

 Return to the osTicket browser and enter "osTicket" in the MySQL Database box. 
 
  <img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/a30cae90-8b72-49e4-bba7-56a396237f5b" height="80%" width="80%" alt="Disk Sanitization Steps"/>

  
</p>
<br />              

38. You should now be able to click "Intall Now" to proceed with intalling osTicket. 
</p>
<br />              


<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/0cf0ff62-a789-44e7-82ab-fec99824889b" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
42. The final step is to perform cleanup. Delete only the setup folder located at 
  C:\inetpub\wwwroot\osTicket\setup.
 
  Next, navigate to the include folder and set the permissions for ost-config.php back to "Read-only." 
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
43. Once the permissions are set, you can test osTicket by logging in.
</p>
<br />              
</p>

<img src="https://github.com/CynthiaBrady/osticket-prereqs/assets/160746865/db7a096a-f0fa-4e66-8cef-0eeb9cbbeb5f" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

44. Congratulations! You have successfully installed and setup osTicket!
</p>
<br />              







