# Deploying Active Directory and Creating Users

<p align="center">
  <img alt="Active Directory" src="https://github.com/Christopherdek/Dep-ActiveD/assets/148359456/d1e221ad-0e55-4691-81ef-20286bcebe5a">
</p>

This tutorial provides a concise walkthrough of the initial stages of Active Directory. It covers the confirmation of connectivity between the client and Domain Controller and the installation of Active Directory. Toward the end, we'll explore creating an organizational unit and a user account, followed by logging in with the new account.

## Environments and Technologies Used

- **Microsoft Azure (Virtual Machines/Compute)**
- **Remote Desktop**
- **Internet Information Services (IIS)**

## Operating System Used

- **Windows 10 (21H2)**

## Stages

1. Confirm the connection between the Domain Controller and the client.
2. Install Active Directory.
3. Create an organizational unit.
4. Create a new employee.
5. Add the new employee to the “Domain Admins” Security Group.
6. Log in with the new employee account.

## Stage 1: Confirming Connectivity

Open the command prompt to confirm connectivity between the Domain Controller and the client using the `ping -t` command and the private IP address of the Domain Controller.

<p align="center">
  <img alt="Confirm Connectivity" src="https://i.imgur.com/vkTuj9O.png">
</p>

## Stage 2: Installing Active Directory

Install Active Directory. During the "Select server roles" step, ensure to select the "Active Directory Domain Services" option.

<p align="center">
  <img alt="Install Active Directory" src="https://i.imgur.com/ONdLQ46.png">
  <img alt="ADDS Role Selection" src="https://i.imgur.com/0LO1L1m.png">
  <img alt="ADDS Installation" src="https://i.imgur.com/Ly5zwkQ.png">
</p>

## Stage 3: Creating an Organizational Unit

Create an Organizational Unit by right-clicking "mydomain.com", then select "new", and finally, click the "Organizational Unit" option.

<p align="center">
  <img alt="Create Organizational Unit" src="https://i.imgur.com/8FHGlI1.png">
</p>

## Stage 4: Creating a New User

Create a new user by right-clicking "mydomain.com", then select "new", and click the "User" option.

<p align="center">
  <img alt="Create New User" src="https://i.imgur.com/rOYg2ZU.png">
</p>

## Stage 5: Adding User to Domain Admins Group

When selecting a new group for the new user, in the "Enter the object name to select," type "Domain," then click "check names." Click the "Domain Admins" option. Save everything by clicking "OK" and "Apply" when finished.

<p align="center">
  <img alt="Add User to Domain Admins" src="https://i.imgur.com/9t7t2iG.png">
</p>

## Stage 6: Logging In

Log out of the Remote Desktop connected to the Domain Controller and log back in as “mydomain.com\john_admin.” Confirm that you are logged in as the new user using the command prompt.

<p align="center">
  <img alt="Log In" src="https://i.imgur.com/Mxlj5SK.png">
</p>
