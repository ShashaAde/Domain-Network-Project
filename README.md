# Domain Network Project

## Objective

The objective of this project is to integrate and expand the networks of three merging companies by planning, building, and configuring IT systems, services, and network infrastructure, including setting up core services, security enhancements, web servers, and more, to successfully manage and operate a IT network.

### Skills Learned

- System Administration and Virtualization       
- Active Directory (AD) and Domain Configuration 
- Networking and Connectivity
- User Creation                 
- Local Users and Groups Management             
- Group Policy Management                      
- Linux System Administration                  
- Web Development and Hosting                  

### Services/Tools Used
- Cisco Packet Tracer to map out the logical layout of my network.
- WordPress to setup an online market place through a LAMP server.
- VMware to set up the servers and workstations.
- Created domain and DNS zones for the VMs.
- Used tools (ipconfig/ifconfig, ping) to assign IPs and test connectivity.
- Enabled RDP for remote access to Windows Pro.
- Set up SSH for remote access to Ubuntu systems.
- Created users and organized them into groups based on departments.
- Applied policies to manage security settings and restrictions.
- Installed WordPress on Ubuntu with Apache and MySQL.
- Wrote a script to search logs for specific domain and login activities.

## Steps

|  Tasks                                                                                                                                                                                                                     |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [Virtual Machine Installation and Operating Systems Setup](Virtual-Machine-Installation-and-Operating-Systems-Setup)|
| [Configured Windows Server 2019 to a Domain](Configured-Windows-Server-2019-to-a-Domain)|
| [Used Network Topology, Commands, and Concepts to Connect Each VM to the Domain](Used-Network-Topology,-Commands,-and-Concepts-to-Connect-Each-VM-to-the-Domain)|
| [Used Remote Desktop Connection to RDP from the Domain Windows Server 2019 to the Workstation Windows 10 Pro](Used-Remote-Desktop-Connection-to-RDP-from-the-Domain-Windows-Server-2019-to-the-Workstation-Windows-10-Pro)|
| [Created Users from CMD/CLI and Gave Them, sudo/admin rights for Ubuntu and Windows](Created-Users-from-CMD/CLI-and-Gave-Them,-sudo/admin-rights-for-Ubuntu-and-Windows)|
| [Set Up Multiple Accounts for the Window Pro 10 Workstation Through the Window Domain](Set-Up-Multiple-Accounts-for-the-Window-Pro-10-Workstation-Through-the-Window-Domain)|
| [Used Active Directory and Group Policies to Manage Domain Accounts](Used-Active-Directory-and-Group-Policies-to-Manage-Domain-Accounts)|
| [Created a Webpage by Setting Up WordPress With Linux Ubuntu Desktop](Created-a-Webpage-by-Setting-Up-WordPress-With-Linux-Ubuntu-Desktop)|
| [Created an Ubuntu Server for System Logging of the Domain Server with Syslog](Created-an-Ubuntu-Server-for-System-Logging-of-the-Domain-Server-with-Syslog)|
| [Made a Bash Script that Asks for a Keyword to Search for, then Queries the Logs for the Keyword](Made-a-Bash-Script-that-Asks-for-a-Keyword-to-Search-for,-then-Queries-the-Logs-for-the-Keyword)|

## Virtual Machine Installation and Operating Systems Setup
-Downloaded VMware Workstation 17 Player to create and run multiple virtual machines on.

-Downloaded the needed ISO files to run on VMware, which included: Windows Server 2019, Windows, Ubuntu Live Server, and Ubuntu. 

### Windows Server 2019 Setup
  ![Screenshot 2024-11-23 182357](https://github.com/user-attachments/assets/14286d57-5b24-410f-9320-c23a6e9f58b8)
  
 Opted to install the Windows Server 2019 ISO file, until later on in the installation process to avoid a VMware disk error which happens when installing the ISO file right away.
  
  ![Screenshot 2024-11-23 172302](https://github.com/user-attachments/assets/84713e12-d589-4b8a-a10b-448862247b45)

Selected the Windows Server 2019 operating system as a host on this virtual machine.

  ![Screenshot 2024-11-23 172719](https://github.com/user-attachments/assets/8fb8627d-4b5f-48c2-83c7-6719c5f6984e)

Allocated memory, and assigned processor cores to the virtual machine. 
    
  ![Screenshot 2024-11-23 172701](https://github.com/user-attachments/assets/404af2d2-2076-40aa-829d-41928e2fb2a7)

  Installed the virtual machine with customized settings to my liking.

  ![Screenshot 2024-11-23 174231](https://github.com/user-attachments/assets/8b8d4a25-fb4f-4312-a338-a265639bc5d9)

  To avoid the VMware disk error, after creating the virtual machine I then added in the ISO file for Windows Server 2019.
  
  ![Screenshot 2024-11-23 174355](https://github.com/user-attachments/assets/93984941-1fe0-4cef-b919-b0d1ba7e0fff)
  
  Started up the Operating System installation process for Windows Server 2019.
  
  ![Screenshot 2024-11-23 174444](https://github.com/user-attachments/assets/8bedcf7b-77f5-4ec8-acc6-66ff5923778e)

  Chose the Standard Windows Server 2019 Operating System as the operating system to be installed on this virtual machine.
  
  ![Screenshot 2024-11-23 174539](https://github.com/user-attachments/assets/49fc3eb7-abdf-4e0f-8c9e-6a4b842238c1)

  Partitioned the hard drive to provide overall performance and scalability options.
    - The installation process completed, and I was sent to the startup log-in interface.

### Windows 10 Pro (Workstation) Setup
  ![Screenshot 2024-11-23 180354](https://github.com/user-attachments/assets/1471993e-ef37-4b0c-a988-4471e3aba989)

  Selected the Windows ISO file for installation into the Virtual Machine set aside for my workstations.  
  
  ![Screenshot 2024-11-23 180457](https://github.com/user-attachments/assets/7b4b4dfa-cc1e-4e85-9631-878f8fd4fd7a)

  Allocated memory, and assigned processor cores to the virtual machine. 
  
  ![Screenshot 2024-11-23 180513](https://github.com/user-attachments/assets/b6778fa8-16fa-4b9b-87ed-65092ed1b33a)

  Installed the virtual machine with customized settings to my liking.

  ![Screenshot 2024-11-23 181254](https://github.com/user-attachments/assets/d35d2ef7-2d17-4674-90c7-d9b8c10823d5)

  Started up the Operating System installation process for Windows 10 Pro (workstations).

  ![Screenshot 2024-11-23 181438](https://github.com/user-attachments/assets/03084196-5a90-4bd1-b047-37d3d82ae8c4)

  Choose Windows 10 Pro as the operating system to be installed on this virtual machine.

  ![Screenshot 2024-11-23 181531](https://github.com/user-attachments/assets/d0d4afcd-c138-425d-9f60-71db056c0681)

  Partitioned the hard drive to provide overall performance and scalability options. 
  
  ![Screenshot 2024-11-23 181554](https://github.com/user-attachments/assets/fb14bbf5-78d3-4cd3-9209-dfcf6e462b18)

  The installation of the Windows 10 Pro operating system began.
  
  ![Screenshot 2024-11-23 182845](https://github.com/user-attachments/assets/27f4adfa-a8ef-4b38-85d5-bf80ea3463e5)

  Once the operating system completed installing, I began to personalize the virtual machine's Microsoft account. 
  
  ![Screenshot 2024-11-23 183107](https://github.com/user-attachments/assets/fc7f3e1c-3eca-4ecb-aa20-686ec5d4ccff)

  Set up a account that will be a administrator for this virtual machine. 
  - The installation process  completed, and I was sent to the startup log-in interface.


### Ubuntu Server Setup
  ![Screenshot 2024-11-23 174653](https://github.com/user-attachments/assets/f904ec06-e32a-4dea-9708-4ae51806eeab)

  Selected the Ubuntu Server ISO file for installation into the Virtual Machine set aside for my workstations.  
  
  ![Screenshot 2024-11-23 174741](https://github.com/user-attachments/assets/b64023a9-cec9-4e84-a98f-c288bb6392e9)

  Set up a Linux user that would be used to install the operating system.
  
  ![Screenshot 2024-11-23 175433](https://github.com/user-attachments/assets/324fee11-7af6-4857-a1ba-e0f78bd85cfb)

  Installed the virtual machine with customized settings to my liking.
  
  ![Screenshot 2024-11-23 180805](https://github.com/user-attachments/assets/280e6faa-146a-4d93-8443-7d0dd60bc79f)

  Started the installation process of the Ubuntu Server operating system.
  
  ![Screenshot 2024-11-23 180952](https://github.com/user-attachments/assets/3c16a7a7-a94d-471d-978a-f7458c96f317)

  Made a user account that would be used for logging into the server.
  
  ![Screenshot 2024-11-23 181033](https://github.com/user-attachments/assets/7f5efe43-17ac-49c4-a2d0-030d8675ffc8)

  Installed OpenSSH server package into the server to allow SSH to remote machines.
  
  ![Screenshot 2024-11-23 181121](https://github.com/user-attachments/assets/db5d4064-0a40-4c88-bc6b-3af1c19bede4)

  Installed the operating system with the setting preferences that I chose.
    - The installation process completed, and I was sent to the startup log-in interface.


### Ubuntu Setup
  ![Screenshot 2024-11-23 200344](https://github.com/user-attachments/assets/9f319339-32f7-4cd1-abca-5cfe5fc0745c)

  Selected the Ubuntu ISO file for installation into the Virtual Machine set aside for my workstations.  

  ![Screenshot 2024-11-23 175054](https://github.com/user-attachments/assets/d9bd9c96-d768-40e8-8b29-909d4521990f)

  Set up a user that would be used to install the operating system.
  
  ![Screenshot 2024-11-23 175154](https://github.com/user-attachments/assets/6f6d0c20-f566-4661-87c2-84b5a0ddeb32)

  Installed the virtual machine with customized settings to my liking.
  
  ![Screenshot 2024-11-23 175613](https://github.com/user-attachments/assets/3c3fc66f-d621-4055-845a-ad0dd6111ab6)

  Choose the default installation of the Ubuntu operating system. 
  
  ![Screenshot 2024-11-23 180151](https://github.com/user-attachments/assets/1330af93-9df2-47b3-9291-d22f8fe02645)

  Set up a user account for Ubuntu.
    - The installation process completed, and I was sent to the startup log-in interface.

## Configured Windows Server 2019 to a Domain 
  ### Created an Active Directory domain
  ![Screenshot 2024-11-23 203245](https://github.com/user-attachments/assets/45fe1317-d947-4a8d-b4df-b8a1901ebf08)

  Used the command line to find my network settings and configuration

  ![Screenshot 2024-11-23 204956](https://github.com/user-attachments/assets/2a54c1ec-087e-428a-8061-018e0a31dedb)

  Added a static IP address with the alternate DNS server address being the same, to allow this host to be promoted to Domain. 

  ![Screenshot 2024-11-23 205447](https://github.com/user-attachments/assets/d73e319c-b2fa-4bc4-b2b3-c902f5ff1670)

  Manage my server to install roles and features as role based.

  ![Screenshot 2024-11-23 205534](https://github.com/user-attachments/assets/6c7a9042-042c-466e-a9bf-b4413bd2efe7)

  Added AD Domain Services and DNS Server roles to the server.

  ![Screenshot 2024-11-23 205558](https://github.com/user-attachments/assets/6c10bc20-d2af-47ec-98ff-65c8ce243982)

  Double checked to make sure Group Policy Management features were still selected.

  ![Screenshot 2024-11-23 205701](https://github.com/user-attachments/assets/824396b3-5686-4291-8abf-e768a9ef000b)

  Installed the roles and features that I selected. 
  
  ![Screenshot 2024-11-23 210525](https://github.com/user-attachments/assets/3a00963c-691c-45b5-b533-7bf153dba514)

  After deploying the AD Domain Services I am now able to promote the server to a domain controller.
  
  ![Screenshot 2024-11-23 210938](https://github.com/user-attachments/assets/23541d1a-511f-428b-9ea7-02e0247684fc)

  Giving the domain (under a new forest) a root name with the .local naming convention.

  ![Screenshot 2024-11-23 211319](https://github.com/user-attachments/assets/f3cf5889-943a-413b-8917-949734ba5c68)

  Left the rest of the settings as default when proceeding with the domain promotion.
    
  - Allowed the promotion operation to complete.
    
  ![Screenshot 2024-11-23 212225](https://github.com/user-attachments/assets/d1d3c307-542e-4eb6-840e-c4e3add71ca1)
  The server has now been promoted. 
  
## Used Network Topology, Commands, and Concepts to Connect Each VM to the Domain
  Used ipconfig/ifconfig to get the Ips of each virtual machine.
  - Used sudo to install net-tools for Ubuntu desktop & server.
    
        sudo apt install net-tools

### Joined my Ubuntu desktop to the Domain 

  ![Screenshot 2024-11-23 234707](https://github.com/user-attachments/assets/efc38c49-f81e-42a8-95b0-d2d438cc068b)

  Added my domain IP as the DNS Server address for my Ubuntu desktop.
    
    
    sudo service NetworkManager restart

    sudo apt install -y realmd libnss-sss libpam-sss sssd sssd-tools adcli samba-common-bin oddjob oddjob-mkhomedir packagekit

  Installed realmd packages that allow my Ubuntu desktop to connect to my domain controller.

    hostnamectl set-hostname ubuntu.portfolio.local

  Changed the host name on my Ubuntu desktop.

    systemctl disable systemd-resolved.service
    systemctl stop systemd-resolved.service

  Disabling the systemd resolve service, so our domain server can resolve the DNS. 

     sudo nano /etc/resolv.conf

  ![Screenshot 2024-11-24 001829](https://github.com/user-attachments/assets/34e2b288-6a14-4f28-b7f4-88de32d1af3f)

  Configured the resolv.conf file to point to the domain controller with nano. 

    realm discover portfolio.local

  ![Screenshot 2024-11-24 002936](https://github.com/user-attachments/assets/e4e687b3-251f-4e0d-8015-95b1450ee771)

  Checking if the Ubuntu desktop can discover the domain controller.

    realm join -U Administrator portfolio.local

  Ran into a problem, where it said I didn't have the prober permissions to join.
    - After doing research I found that editing/creating a /etc/krb5.conf and adding the following worked:
    
    [libdefaults]
    default_realm = portfolio.local
    rdns = false
  
  ![Screenshot 2024-11-24 010956](https://github.com/user-attachments/assets/a8ddad54-15c0-4086-bf97-fc74d58d8e9c)

 Joined the Ubuntu desktop to the domain with realm. 

### Joined my Ubuntu server to the Domain 

    sudp apt update -y

  - Making sure I have all the current packages updated.

        sudo apt install -y realmd libnss-sss libpam-sss sssd sssd-tools adcli samba-common-bin oddjob oddjob-mkhomedir     packagekit

  - Installed realmd packages that allow my Ubuntu desktop to connect to my domain controller.

        sudo hostnamectl set-hostname ubntu-s.portfolio.local

  - Changed the host name of the Ubuntu server.

  hostname

  - Checked to see if hostname changed.

        systemctl disable systemd-resolved.service
        systemctl stop systemd-resolved.service

  - Disableing the systemd resolve service, so our domain server can resolve the DNS. 

        systemctl status systemd-resolved.service

  - Checked to make sure the service is no longer running. 

        sudo vim /etc/resolv.conf
 
  ![Screenshot 2024-11-24 013616](https://github.com/user-attachments/assets/bd2edc72-64db-46d4-bcd4-310c2827fd51)

  Configured the resolv.conf file to point to the domain controller with vim. 

    realm discover portfolio.local

  ![Screenshot 2024-11-24 013843](https://github.com/user-attachments/assets/b411c205-6f3b-4545-8735-1e1f8d3cf892)

  Checking if the Ubuntu desktop can discover the domain controller.

  realm join -U Administrator portfolio.local

   - Ran into the same problem that happened with the Ubuntu desktop, where it said I didn't have the proper permissions to join.
   - After repeating the troubleshooting process by editing/creating a /etc/krb5.conf and adding the request to join worked:

    [libdefaults]
    default_realm = portfolio.local
    rdns = false
  
  ![Screenshot 2024-11-24 015433](https://github.com/user-attachments/assets/4f09b362-c636-4eeb-b173-853e2df42caf)

  Joined the Ubuntu desktop to the domain with realm.

### Joined my Windows 10 Pro (workstation) to the Domain 

  ![Screenshot 2024-11-24 021453](https://github.com/user-attachments/assets/4a87f882-9092-40ec-9f25-dfef359bd8d2)

  Set the workstation's IP address to static (while on a administrator account), and made the DNS server's IP address the same as my domain controllers IP.
  
  ![Screenshot 2024-11-24 021838](https://github.com/user-attachments/assets/e1fe1b1d-ae1c-48a4-90c9-7dd6f6f1cec9)

  Performed a nslookup to make sure the DNS server is resolved. 

  ![Screenshot 2024-11-24 022432](https://github.com/user-attachments/assets/3bdf33ee-b355-4051-ad2d-c97f1d2b6fc7)

  Changed the workstation's name and domain through System Properties in Windows Settings.

  ![Screenshot 2024-11-24 022959](https://github.com/user-attachments/assets/92ee8194-6104-463f-ab5b-ab6c7980daba)

  Joined the workstation to the domain. 

### Created forward lookup zones for the Windows Pro, and Ubuntu VMs to add to my domain 

 ![389244565-1faa15e7-c699-47cd-94aa-888987457e36](https://github.com/user-attachments/assets/66dfa8e5-6176-4698-8e37-dfce82b8e26f)

 Accessed the DNS Manager through the tools section of the Server Manager.
 
 ![Screenshot 2024-11-23 215951](https://github.com/user-attachments/assets/4d2b3342-33c9-40b6-ab22-319be5640f39)

 Created a new Zone.
   - Made sure the new Zone was a Primary zone.
   - Assigned a name (portfolio.com) to the zone.
   
![Screenshot 2024-11-23 220609](https://github.com/user-attachments/assets/dd45a557-9812-4366-9f25-cab111b796f8)

 This the result of the new Zone (forward). 

![Screenshot 2024-11-23 222039](https://github.com/user-attachments/assets/56d16158-b825-4b1b-9b09-5a6e2ce5a441)

Added a new host (PW) to resolve a name to its IP.
  - I did the same for the Domain, Ubuntu desktop and Ubuntu server.

 ### Created reverse lookup zones for the Windows Pro, and Ubuntu VMs to add to my domain 

  Accessed the DNS Manager through the tools section of the Server Manager.
 
![Screenshot 2024-11-23 222719](https://github.com/user-attachments/assets/d9cf1e96-a94e-422b-8b4c-1e6dc622445a)

 Created a new Zone.
   - Made sure the new Zone was a Primary zone.
   - Chose IPv4Reverse Lookup Zone.

![Screenshot 2024-11-23 223425](https://github.com/user-attachments/assets/f96456cc-cd26-4027-8015-570f1daf5363)

Provided my Network ID.

![Screenshot 2024-11-23 223651](https://github.com/user-attachments/assets/bee9a233-91e0-4a54-9971-94b5e20382a2)

This is the result of the new Zone (reverse).

![Screenshot 2024-11-23 224147](https://github.com/user-attachments/assets/a4436a9e-6dd0-44fa-8cb5-3dfb440bd25c)

Added a new Pointer for PW to resolve a IP to its name.
  - I did the same for the Domain, Ubuntu desktop and Ubuntu server.

### Results and Testing 
![Screenshot 2024-11-23 224658](https://github.com/user-attachments/assets/1e5d1a06-737d-495e-b83d-d491577712b8)

![Screenshot 2024-11-23 232820](https://github.com/user-attachments/assets/bc875524-1700-484b-8054-58574edd2c6e)

This is the result of the forward lookup zone.

![Screenshot 2024-11-23 224716](https://github.com/user-attachments/assets/96995709-9dd1-465a-9cd0-022e8519a8b4)

![Screenshot 2024-11-23 233116](https://github.com/user-attachments/assets/71e59ea1-f813-4369-9aa7-be4c574360d1)

This is the result of the reverse lookup zone.

A problem I am running into right now is that my workstation can reach my domain, but my domain can't find the workstation.
  - I then tried my Ubuntu desktop virtual machine and my domain was able to find it. 
  - I troubleshot this problem by turning off the workstations firewall, and that let me know were to find a solution.
  
![Screenshot 2024-11-23 231808](https://github.com/user-attachments/assets/34ba4c14-35f5-4b6c-9915-e3b5ff3d9219)

To solve this problem, I made a Inbound Protocol ICMPv4 rule , to allow incoming ping requests from all IPs.
  - I was then able to ping the workstation.

## Used Remote Desktop Connection to RDP from the Domain Windows Server 2019 to the Workstation Windows 10 Pro
  ### Turning on Remote desktop access for the workstation
  
  ![Screenshot 2024-11-24 154426](https://github.com/user-attachments/assets/5ff10613-4189-4d08-b6c0-2106cbe699b1)

  Searched for the desktop settings in the Windows search bar.
    - Enabled Remote Desktop in the Windows System settings. 

  ![Screenshot 2024-11-24 154023](https://github.com/user-attachments/assets/de24266a-c48d-47e8-9aec-1d53a30f3c47)
  
  Searched for the Remote Desktop Connection App in the Windows Search bar.
    - Connected to the workstation by entering in its name on the network.
    - If I had more than one account on the computer then it would of prompted me to enter in which account I would like to RDP into. 

  ![Screenshot 2024-11-24 154650](https://github.com/user-attachments/assets/2563144f-2d8a-4fdd-8bac-5147705520b1)

  Once the workstation was found, I was prompted to log into the user account on the workstation (Administrator).

  ### Results
  
  ![Screenshot 2024-11-24 155224](https://github.com/user-attachments/assets/00d69c0b-cbd6-4b67-901b-70b271986d49)

  The domain controller was able to successfully RDP into the workstation. 

  ## Used SSH to Gain Remote Access to Linux Clients from a Windows client, as well as from One Linux Client to Another 

  ### Used PowerShell on a Windows client to SSH into Linux clients.

  Searched for Windows PowerShell in the Windows search bar.
    - Ran Windows PowerShell as administrator. 

    Get-WindowsCapability -Online | ? Name -like 'OpenSSH.Client*'
  
  ![Screenshot 2024-11-24 161146](https://github.com/user-attachments/assets/16503570-7f19-4fd2-bd55-fd9952617a19)

  Checked to see if ssh was installed.

    ssh shashaade@ubntu-s.portfolio.local 
  
  ![Screenshot 2024-11-24 162416](https://github.com/user-attachments/assets/46d4365f-6e21-40d6-9cca-1b768a95cece)

  After entering my Ubuntu server's login credentials, I was able to successfully SSH into it.
   
  ![Screenshot 2024-11-24 225216](https://github.com/user-attachments/assets/96ada3a8-a0d8-43c0-a17a-5cab9a6916f2)

  This is the same process for using SSH to get into the Ubuntu desktop.

  ### Used SSH to gain remote access between two Linux clients.

    ssh shashaade@ubntu-s.portfolio.local 
  
  ![Screenshot 2024-11-24 223950](https://github.com/user-attachments/assets/277ec7d5-e339-48d3-8c11-f6b8b9f6e3af)

  After entering my Ubuntu server's login credentials, I was able to successfully SSH into it.
  
  ![Screenshot 2024-11-24 224756](https://github.com/user-attachments/assets/4e908bcb-6cfd-4ed0-b65a-51b9596b9d04)

  This is the same process for using SSH to get into the Ubuntu desktop.

  
## Created Users from CMD/CLI and Gave Them, sudo/admin rights for Ubuntu and Windows
  ### Windows 

  net user username (testAdmin) password (justforfun12) /add 
  
  Added a new user on the client.

    net localgroup administrators user (testAdmin) /add

  Added the user to the local client's andministration group.

  ### Ubuntu 

    sudo adduser username (sha) 

  Added a new user on the client.

    sudo usermod -aG sudo username (sha)

  Added the user to the local client's andministration group.
  
    net user
  ![Screenshot 2024-11-24 212306](https://github.com/user-attachments/assets/50966798-e4dc-44ef-ab91-252ed1870ac2)

  Confirmed the user account was created on the client.

## Set Up Multiple Accounts for the Window Pro 10 Workstation Through the Window Domain
  
  ![Screenshot 2024-11-24 180441](https://github.com/user-attachments/assets/03a7b669-5963-40e3-bb7d-beb4f683116a)

  Created and organized unit with sub-organized units of containing different departments of a company within the Active Directory Users and Computers tool settings.

  ![Screenshot 2024-11-24 181150](https://github.com/user-attachments/assets/78de467f-96ea-48d3-9e00-c744c3153b52)

  Created users in each of the sub-organized units.
  
  ![Screenshot 2024-11-24 181312](https://github.com/user-attachments/assets/6aff5f79-100e-466c-8e3d-f62111a94690)

  Made security groups for each department.
  
  ![Screenshot 2024-11-24 181537](https://github.com/user-attachments/assets/e91bd76e-a588-4dcd-8407-02019c3a4138)

  Added each user to their respective groups. 
  
  ![Screenshot 2024-11-24 182209](https://github.com/user-attachments/assets/4e392cb5-ede6-48d5-b833-a882dbb5c474)

  Accessed the accounts (on the workstation) that were made by the domain controller.

## Used Active Directory and Group Policies to Manage Domain Accounts

  ### Created a group policy through account policies in the security settings to limit the character length of a password to 12 minimum for users on the Windows Pro system
  
  ![Screenshot 2024-11-24 184621](https://github.com/user-attachments/assets/d3eded6b-0649-4f70-b52f-f9d1fae514a7)

  Created a new policy for my domain controller from the Group Policy Management in the Tools tab.
  - This policy is will be applied to those in Portfolio.INC.
    
  ![Screenshot 2024-11-24 183726](https://github.com/user-attachments/assets/5f339739-7042-4dfd-97ac-abf621d0a2c2)

  Edited the Company Policy in Portfolio.INC to change the Password Policy (under the Computer Configuration's tab) to allow the minimum characters of a password to be 12. 
  
  ![Screenshot 2024-11-24 184844](https://github.com/user-attachments/assets/e6286fe6-8f3e-464b-bd97-924b89b24951)

  When trying to change the password with anything lower than 12 characters, this is the message that was shown. 

  ### Created a group policy through software restriction policies in the security settings to restrict all users in the domain form opening Internet Explorer.
  
  ![Screenshot 2024-11-24 190142](https://github.com/user-attachments/assets/47b45f40-6537-467b-a821-318c7efcb3e4)

  Created a new policy for my domain controller from the Group Policy Management in the Tools tab.
  - This policy is will be applied to all users in the domain.
  
  ![Screenshot 2024-11-24 190614](https://github.com/user-attachments/assets/22f2a892-2aaf-4bc4-83e3-e797b7f64983)

  Enabled a policy to disable Microsoft Store under the Group Policy Manager Editor with the path of: Computer configuration > policies > administrative templates > windows components  > Internet Explorer.
  
  ![Screenshot 2024-11-24 193814](https://github.com/user-attachments/assets/7f24f933-bb2d-4072-a12c-906522e82cc5)

  Now you can not opened Internet Explorer/ Microsoft Edge


  ### Used group policies for network file share to make a secure drive-map for the domain controller and departments within the organization to share files.

  ![Screenshot 2024-11-24 203856](https://github.com/user-attachments/assets/f6263b97-e3e2-42c8-8f6b-db316478ed9d)

  Allowed sharing permissions to everyone om a file "Share" through Advanced Sharing Permissions of folder properties.
  -within that "Share" file I added department folders for: IT, CEO, Accounts and Sales.
  
  ![Screenshot 2024-11-24 204238](https://github.com/user-attachments/assets/6ef3660a-c251-49e3-8289-90b854a77d3c)

  Made a Organizational Unit for shared folders, where I assigned all users to a select group based off their department.
  
  ![Screenshot 2024-11-24 204619](https://github.com/user-attachments/assets/1c470dab-8447-4b0c-b821-a73c6c6ce9e4)
  
  Gave sf-admins ownership of the "Share" file with full control, while domain users are given read & execute access. 
  
  ![Screenshot 2024-11-24 205519](https://github.com/user-attachments/assets/aa5597ff-da2f-4ac1-8e08-890d4bc81935)

  Changed ownership to "sf-administrators", and disable inheritance for each subfolder in the shares folder, while giving each subcategory all permissions except file deleting, changing permissions and the ability to take ownership.
  - Also removed Domain Users from having any permissions. 

  ![Screenshot 2024-11-24 210135](https://github.com/user-attachments/assets/d86173f3-c085-423e-b620-398996f3e15f)

  Created a map drive with Group Policy Management in the domain controller's tools tab
  
  ![Screenshot 2024-11-24 210503](https://github.com/user-attachments/assets/29a9b83b-9aec-4572-9c0c-cd4805d2d949)

  Edited the mapped-drive group policy to create a map drive by navigating to: User Configuration > Preferences > Windows Settings > Drive Maps
  
  ![Screenshot 2024-11-24 210540](https://github.com/user-attachments/assets/7b1c0adb-7742-49ea-ad59-770a109ece91)

  Created a Drive Map and using the path location of the "Shares" file
  - Linked the GPO to the domain.

  ### Results 
  ![Screenshot 2024-11-24 211003](https://github.com/user-attachments/assets/1d6e8328-7ffa-4148-bc48-620661dfcab8)

  On my workstation I can see the shared network file.
  
  ![Screenshot 2024-11-24 211119](https://github.com/user-attachments/assets/5d467d8a-acfa-402b-a1aa-f3112abcd250)

  On my CEO account, I can only access the CEO folder
  - This is what happens when trying to access another folder. 
   
  ![Screenshot 2024-11-24 211138](https://github.com/user-attachments/assets/fa5189df-6af4-464e-b606-a38bddd4228e)

  Here I am able to access the CEO folder, where I can do everything, but delete and take over files. 

## Created a Webpage by Setting Up WordPress With Linux Ubuntu Desktop
  Used Ubuntu's guide on how to Install and configure WordPress https://ubuntu.com/tutorials/install-and-configure-wordpress#1-overview
  ### Installed Dependencies 
  
    sudo apt update
  
  Made sure my ubuntu was updated before installing packages in the CLI

    sudo apt install apache2 \
                 ghostscript \
                 libapache2-mod-php \
                 mysql-server \
                 php \
                 php-bcmath \
                 php-curl \
                 php-imagick \
                 php-intl \
                 php-json \
                 php-mbstring \
                 php-mysql \
                 php-xml \
                 php-zip
                 
   Installed multiple packages 
   
   ### Installed WordPress
    
     sudo mkdir -p /srv/www
     sudo chown www-data: /srv/www
     sudo apt install curl
     curl https://wordpress.org/latest.tar.gz | sudo -u www-data tar zx -C /srv/www

   Made a new directory for WordPress, and then changed the owner to Apache. 
   
   sudo nano /etc/apache2/sites-available/wordpress.conf
   
   Created a file to host the Apache site for WordPress. 
  
  ### Configured Apache for WordPress
  
    <VirtualHost *:80>
      DocumentRoot /srv/www/wordpress
      <Directory /srv/www/wordpress>
          Options FollowSymLinks
          AllowOverride Limit Options FileInfo
          DirectoryIndex index.php
          Require all granted
      </Directory>
      <Directory /srv/www/wordpress/wp-content>
          Options FollowSymLinks
          Require all granted
      </Directory>
    </VirtualHost>
    
   Added configurations within the file above.
   
     sudo a2ensite wordpress
     systemctl reload apache2

   Enabled the Wordpress site.
   
     sudo a2enmod rewrite
     systemctl restart apache2

   Enabled a Apache module.

     sudo a2dissite 000-default
     systemctl reload apache2

   Disabled the default website.

     sudo service apache2 reload

   Reloaded apache.

   ### Configured database
   
     sudo mysql -u root
  
   ![Screenshot 2024-11-24 232806](https://github.com/user-attachments/assets/7c1a15c2-15ee-4298-8365-34617435f596)

   Opened MySQL database.
   
    CREATE DATABASE wordpress;
   
   Created a new database named "wordpress".
   
     CREATE USER wordpress@localhost IDENTIFIED BY '<your-password(testing)>';  
  
   Created a new user named "wordpress", and configured its password.
    
     GRANT SELECT,INSERT,UPDATE,DELETE,CREATE,DROP,ALTER ON wordpress.* TO wordpress@localhost;

   Gave permissions on the WordPress database.
   
     FLUSH PRIVILEGES;
  
   Updated MySQL permissions.

     quit 
   
   Exited out of the database.

   ### Configured WordPress

     cd /srv/www/wordpress/
   ![Screenshot 2024-11-24 233923](https://github.com/user-attachments/assets/302e3a2a-b86d-49a4-b8e1-6c0971f79bad)
 
   Moved into the WordPress directory.
   - ls displays a list of files in the current directory.

    sudo -u www-data cp wp-config-sample.php wp-config.php
  
   Copied a the sample file into "wp-config.php".

     sudo -u www-data nano wp-config.php
  
   ![Screenshot 2024-11-24 234909](https://github.com/user-attachments/assets/442c4053-4442-42c7-af34-89101ae0d7d6)

   Editing the "wp-config.php" file 
   - Entered my database name (WordPress), database user (WordPress) and password (testing) into the file.

   ### Configure WordPress
   
   ![Screenshot 2024-11-24 235503](https://github.com/user-attachments/assets/d267231b-8ada-42e2-9a83-242376ee87cb)

   Went to my browser to configure WordPress by searching "http://localhost/".
   
   ![Screenshot 2024-11-24 235707](https://github.com/user-attachments/assets/f49ab4d0-c7ff-4da4-b8c6-bd047a262f47)

   Successfully installed WordPress through apache for my Linux client.

## Created an Ubuntu Server for System Logging of the Domain Server with Syslog
   ### Configured rsyslog

     nano /etc/rsyslog.conf
   
   Edited the rsyslog file. 

   ![Screenshot 2024-11-25 002320](https://github.com/user-attachments/assets/b325f76f-831a-4e22-92d3-a63e0b6dfc62)

   Added configurations to the rsyslof file.
    - These configuration tells the server that we are running syslog with its port UDP 514.
   
   ![Screenshot 2024-11-25 002657](https://github.com/user-attachments/assets/532b2496-f6bc-4fe9-91ec-0533e3f334b0)

   Added configurations that will send the logs to a designated area to be displayed by Hostname/Program

     rsyslogd -f /etc/rsyslog.conf -N1
   ![Screenshot 2024-11-25 003402](https://github.com/user-attachments/assets/478aa63f-8274-4d3e-b486-9f42aa3a7de7)

   Checked for any configuration errors. 

   ### Configured client 

     sudo nano /etc/rsyslog.conf

   Edited the rsyslog file on my Ubuntu desktop to connect to my domain controller. 
  
   ![Screenshot 2024-11-25 013531](https://github.com/user-attachments/assets/e6d3c88a-8717-436c-885a-fe9c9f51f594)

   
   Told the rsyslog server where it can find the client at, and added other configurations at the bottom. 
   - These configurations where from a YouTube video found here: https://www.youtube.com/watch?v=mBJ8JfJnlXQ&t=199s

         rsyslogd -f /etc/rsyslog.conf -N1
  
   ![Screenshot 2024-11-25 010147](https://github.com/user-attachments/assets/11fdac9a-f44a-40e5-bc3d-578190756660)

   Checked for any configuration errors.

   netstat -anup
   ![Screenshot 2024-11-25 014037](https://github.com/user-attachments/assets/f98be6ee-ee83-43b3-8550-9a5dbc63a0a7)

   Checked to see if rsyslog's port (514 UDP) was up.

     cd /var/log

   Moved to the log directory.

     ls
   
   ![Screenshot 2024-11-25 014226](https://github.com/user-attachments/assets/3bed20a2-2287-4a56-bbad-ebcbde79d1d3)

   Listed all the files in the log directory.

     cd/ubuntu-s 
     ls

   Moved into my log files I configured and listed all the files that my client is logging.

   ### Results 
   
   ![Screenshot 2024-11-25 014435](https://github.com/user-attachments/assets/8ea8f7c8-9edd-4d0e-b496-e3c50634b447)

  ## Made a Bash Script that Asks for a Keyword to Search for, then Queries the Logs for the Keyword
  
    cd/var/log 

  Moved to the log directory.
  
    touch query_logs.sh

  Created the script file. 

    nano query_logs.sh 

  Edited the script file.

    #!/bin/bash
  
   read -p "Enter a keyword to search for in logs: " keyword
   
     grep -ri "$keyword" /var/log 2>/dev/null || echo "No results found for '$keyword'."

   Created a script to search the logs for a keyword that I typed in and then displays where the keyword was found. 

     chmod +x search_logs.sh

   Gave the script execute rights.

     ./query_logs.sh

   Ran the bash script. 

   ### Results
  
   ![Screenshot 2024-11-25 024048](https://github.com/user-attachments/assets/0e7a56e2-3b66-4e4e-bc04-420b37b734b0)
  
   ![Screenshot 2024-11-25 024403](https://github.com/user-attachments/assets/6b3141c2-468f-488c-9b88-154b63fef0ff)

   The bash script prompts the user to enter in a word they would like to see associated with any logs that are being captured in the domain controller. 
   
   - It then finds logs with the keyword and displays them. 
   - If no logs are found, it displays "No results found for (the keyword).


  
  


   


  

    
   
   
   



  



