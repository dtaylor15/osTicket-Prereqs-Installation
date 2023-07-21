# osTicket-Prereqs-Installation
<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

# osTicket - Prerequisites and Installation
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket. 

Come across errors you can't figure out? Message me on Discord @deedeet15 👾<br />

## Environments and Technologies Used

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop 
- Internet Information Services (IIS)
- [osTicket Installation Documentation](https://docs.osticket.com/en/latest/Getting%20Started/Installation.html) 

## Operating Systems Used

- Windows 10</b> (21H2)

## List of Prerequisites

1. [Create a virtual machine in Azure and access it using Remote Desktop](https://github.com/dtaylor15/osTicket-Prereqs-Installation#create-a-virtual-machine-in-azure-and-access-it-using-remote-desktop)

    - Microsoft Remote Desktop for [MacOS](https://apps.apple.com/us/app/microsoft-remote-desktop/id1295203466?mt=12)
2. [Access the required installation files](https://github.com/dtaylor15/osTicket-Prereqs-Installation#access-the-required-installation-files) 
3. [Enable IIS and subsequent features in Windows VM](https://github.com/dtaylor15/osTicket-Prereqs-Installation#in-windows-enable-iis-and-subsequent-features) 
4. [Download and install the required installation files](https://github.com/dtaylor15/osTicket-Prereqs-Installation#download-and-the-install-the-required-installation-files)
5. [Setup osTicket](https://github.com/dtaylor15/osTicket-Prereqs-Installation#setup-osticket)
6. [Clean up your setup/permissions](https://github.com/dtaylor15/osTicket-Prereqs-Installation#clean-up-your-setuppermissions)
7. [Access your osTicket helpdesk login](https://github.com/dtaylor15/osTicket-Prereqs-Installation#access-your-osticket-helpdesk-login)
8. [Browse your osTicket end-user page](https://github.com/dtaylor15/osTicket-Prereqs-Installation#browse-your-osticket-end-user-page)

## Installation Steps
### Create a virtual machine in Azure and access it using Remote Desktop
<p>


https://github.com/dtaylor15/osTicket-Prereqs-Installation/assets/101889571/82c34051-02dc-44cd-b6da-41fce79d06cb

</p>
<p>
Name your VM "VM-osTicket" for best organizational practices. The region you choose is where your VM's physical reasources are located. Create a VM with a Windows 10 image and 4vCPUs for optimal proccessing speed. Set a usermae and password you will remember, this is how you will log onto the desktop. Creating a new VM in azure will automatically create a vnet (your VM's network) and a resource group (where your VM will be stored in Azure). Ensure RDP port 3389 is enabled, this is how you will access your VM's desktop. Make no changes on the Disk tab. On the Network tab observe your vnet and IP address. Ensure that the IP and NIC will delete when your VM is deleted. This prevents unwanted storage charges in Azure. Make no changes on the Management, Monitoring, and Advanced tabs. Review and create your VM. Wait for Deployment to finish. 
</p>

> **Note**
> Using a virtual machine to host osTicket preserves resources on your personal machine.

<br />

<p>
<img width="782" alt="remote in" src="https://github.com/dtaylor15/osTicket-Prereqs-Installation/assets/101889571/a1736836-486b-4b11-8654-60345ca9dac9">
    
</p>
<p>
Copy VM-osTicket's public IP address and paste it in Remote Desktop Connection (Windows) or Microsoft Remote Desktop (MacOS). Give it a "friendly name" and log in with the username and password you configured. If using a Windows PC, your log in screen may look different. The functions are still the same. The VM's desktop will populate after a successful login. 
</p>
<br />

### Access the required installation files
<p>
<img width="505" alt="Screenshot 2023-07-20 at 16 28 36" src="https://github.com/dtaylor15/osTicket-Prereqs-Installation/assets/101889571/7c5a3d5c-a66d-4bf8-949f-5f6aa19a187e">
<br />
</p>

Copy and paste [this link](https://drive.google.com/drive/folders/1Jc9E6JWnnyLiUse49tfqYC4zGCkVRwSW?usp=drive_link)  within your Windows VM for easy access to the required instalation files
<br />


### Enable IIS and subsequent features in Windows VM
<p><img width="683" alt="Screenshot 2023-07-21 at 11 36 10" src="https://github.com/dtaylor15/osTicket-Prereqs-Installation/assets/101889571/80491660-de23-4166-b131-893a1dcbd7cd">
</p>
<p>
Find IIS: Control Panel -> Programs and Features -> Turn Windows features on and off
</p>
<br />

<br />
<p> <img width="983" alt="Screenshot 2023-07-21 at 11 51 43" src="https://github.com/dtaylor15/osTicket-Prereqs-Installation/assets/101889571/a7dfc3a3-0346-4b06-9211-91969bfbb111">
</p>

<p>In the Windows Features settings enable: [▪️]Internet Information Services -> [▪️]Web Management Tools -> [▪️]IIS Management Console -> [✔] IIS Management Console
   
Enable CGI and Common HTTPS features: [▪️]World Wide Web Services -> [▪️]Application Development Features -> [✔] CGI -> [▪️]Common HTTP Features
 </p>
 
<br />

https://github.com/dtaylor15/osTicket-Prereqs-Installation/assets/101889571/5b498b8b-833a-4cdf-9b53-fe6f16a606da

<p>Verify IIS functionality with loopback address: Type 127.0.0.1 in Edge browser, the IIS welcome page will populate. </p>
<br />

    
### Download and the install the required installation files
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

### Setup osTicket
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

### Clean up your setup/permissions
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

### Access your osTicket helpdesk login
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

### Browse your osTicket end-user page
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

## osTicket - Prerequisites and Installation Complete!👏🏾
<p>Come across errors you can't figure out? Message me on Discord @deedeet15 👾</p>
