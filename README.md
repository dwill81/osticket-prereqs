<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1> Prerequisites and Installation of osTicket deployed through Azure</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Microsoft Web Platform Installer
- OsTicket V1.15.8
- HeidiSQL

<h2>Installation Steps</h2>

<p>
<img width="384" alt="image" src="https://user-images.githubusercontent.com/122701786/212573630-af7892a3-78cc-42aa-af2a-a4abbab4b4db.png">
<img width="311" alt="image" src="https://user-images.githubusercontent.com/122701786/212573696-96a8e587-f9f8-4179-9a5b-da04790c9fe3.png">
</p>
<p>
1. Create a "Virtual Machine" with Azure and "Remote Desktop" into the created VM. 
</p>
<br />

<p>
<img src="https://imgur.com/n9ibcLa.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
2. Install/Enable Internet "Internet Information Services" (IIS) in windows: control panel --> programs --> Turn Windows features on or off --> check box titled "Internet Information Services".  IIS is a windows server in which OsTicket requires to be enabled in order to run properly, even though OsTicket runs through the web browser.


</p>
<p>
<img src="https://i.imgur.com/8ob8uQq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
3. Install osTicket v1.15.8.
</p>

<br />

<p>
<img src="https://i.imgur.com/SbhSS6V.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
4. Go Back To IIS, Sites->Default->osTicket, Double click PHP Manager, Enable PHP_imap.dll, Enable PHP_intl.dll, Enable PHP_opcache.dll
</p>
<br />

<p>
<img src="https://i.imgur.com/wVSvcC6.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
5. Rename File To OST-Config.PHP And Assign Permissions To File.
</p>
<br />

<p>
<img src="https://i.imgur.com/U0zZqC1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
6. Continue Setting Up OsTicket In Browser.
  -Name Help Desk
  -Add Default Email
</p>
<br />

<p>
<img src="https://i.imgur.com/IdTzZWd.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
7. Download And Install HeidiSQL.
</p>
<br />

<p>
<img src="https://i.imgur.com/0LOpcLJ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
8. You should see a congratulations screen in the browser window if everything was done correctly. Help desk tickets are now able to be created and assigned.
</p>
<br />

<img width="707" alt="Screenshot 2023-01-15 200435" src="https://user-images.githubusercontent.com/122701786/212579185-8929e2d9-1170-4387-a3b2-226635346f1c.png">

<img width="748" alt="image" src="https://user-images.githubusercontent.com/122701786/212580509-b093a742-8185-4b58-b70f-89d383182846.png">

