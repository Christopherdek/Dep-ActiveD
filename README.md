<h1>Deploying Active Directory and Creating Users</h1>

![image](https://github.com/Christopherdek/Dep-ActiveD/assets/148359456/d1e221ad-0e55-4691-81ef-20286bcebe5a)



This is a brief tutorial that outlines the beginning stages of Active directory by confirming the connectivity between the client and Domain Controller and the installation of Active Directory. Towards the end, we will take a look at how to create a organizational unit and a username and log in with the new account.<br />



<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Stages</h2>

- Confirm the connection between the Domain Controller and the client
- Install Active Directory
- Create an organizational unit
- Create a new employee
- Add the new employee to the “Domain Admins” Security Group
- Log in with the new employee account


<h2>Stages</h2>

<p>
<p>
Go into the command prompt to confirm connectivity between the Domain Controller and client by using the ping -t command and the private ip address of the Domain Controller
</p>
<img src="https://i.imgur.com/vkTuj9O.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />

<p>
<p>
Install Active Directory. When you get to the "Select server roles", make sure to click the "Active Directory Domain Services" option.
</p>
<img src="https://i.imgur.com/ONdLQ46.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/0LO1L1m.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/Ly5zwkQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<br />

<p>
<p>
Create an Organizational Unit by right clicking "mydomain.com", then select "new". Finally, click the "Organizational Unit" option.
</p>
<img src="https://i.imgur.com/8FHGlI1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />

<p>
<p>
Create a new user by right clicking "mydomain.com", then select "new". Click the "User" option.
</p>
<img src="https://i.imgur.com/rOYg2ZU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />


<p>
<p>
When you select a new group for the new user, in the "Enter the object name to select", type in "Domain". Then click "check names". Click the "Domain Admins" option. Make sure to save everything by clicking "ok" and "apply" when finished.
</p>
<img src="https://i.imgur.com/9t7t2iG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />


<p>
<p>
Log out of the Remote Desktop that is connected to the Domain Controller and log back in as “mydomain.com\john_admin”. Confirm that you are logged in as the new user by using the command prompt.
</p>
<img src="https://i.imgur.com/Mxlj5SK.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />

