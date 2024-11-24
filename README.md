# Domain Network Project

## Objective

The objective of this project is to integrate and expand the networks of three merging companies by planning, building, and configuring IT systems, services, and network infrastructure, including setting up core services, security enhancements, web servers, and more, to successfully manage and operate a IT network.

### Skills Learned

- System Administration and Virtualization       
- Active Directory (AD) and Domain Configuration 
- Networking and Connectivity                   
- Local Users and Groups Management             
- Group Policy Management                      
- Linux System Administration                  
- Web Development and Hosting                  

### Services/Tools Used
- Cisco Packet Tracer to map out the logical layout of my network
- Wordpress to setup a online market place thorugh a LAMP server
- VMware to set up the servers and workstations
- Created domain and DNS zones for the VMs.
- Used tools (ipconfig/ifconfig, ping) to assign IPs and test connectivity.
- Enabled RDP for remote access to Windows Pro.
- Set up SSH for remote access to Ubuntu systems.
- Created users and organized them into groups based on departments.
- Applied policies to manage security settings and restrictions.
- Installed WordPress on Ubuntu with Apache and MySQL.
- Wrote a script to search logs for specific domain and login activities.
  
## Steps

## Virtual Machine Installation and Operating Systems Setup
-Downloaded VMware Workstation 17 Player to create and run multiple virtual machines om.

-Downloaded the needed ISO files to run on VMware, which included: Windows Server 2019, Windows, Ubuntu Live Server, and Ubuntu. 

### Windows Server 2019 Setup
  ![Screenshot 2024-11-23 182357](https://github.com/user-attachments/assets/14286d57-5b24-410f-9320-c23a6e9f58b8)
  
 Opted to install the Windows Server 2019 ISO file, until later on in the installation process to avoid a VMware disk error which happens when installing the ISO file right away.
  
  ![Screenshot 2024-11-23 172302](https://github.com/user-attachments/assets/84713e12-d589-4b8a-a10b-448862247b45)

Selected the Windows Server 2019 operating system as a host on this particular virtual machine.

  ![Screenshot 2024-11-23 172719](https://github.com/user-attachments/assets/8fb8627d-4b5f-48c2-83c7-6719c5f6984e)

Allocated memory, and assigned processor cores to the virtual machine. 
    
  ![Screenshot 2024-11-23 172701](https://github.com/user-attachments/assets/404af2d2-2076-40aa-829d-41928e2fb2a7)

  Installed the virtual machine with customized settings to my liking.

  ![Screenshot 2024-11-23 174231](https://github.com/user-attachments/assets/8b8d4a25-fb4f-4312-a338-a265639bc5d9)

  To avoid the VMware disk error, after creating the virtual machine I then addded in the ISO file for Windows Server 2019.
  
  ![Screenshot 2024-11-23 174355](https://github.com/user-attachments/assets/93984941-1fe0-4cef-b919-b0d1ba7e0fff)
  
  Started up the Operating System installation process for Windows Server 2019.
  
  ![Screenshot 2024-11-23 174444](https://github.com/user-attachments/assets/8bedcf7b-77f5-4ec8-acc6-66ff5923778e)

  Chose the Standard Windows Server 2019 Operating System as the operating system to be installed on this particular machine.
  
  ![Screenshot 2024-11-23 174539](https://github.com/user-attachments/assets/49fc3eb7-abdf-4e0f-8c9e-6a4b842238c1)

  Partitioned the hard drive to provide overall performance and scallability options.
    - The installation proccess completed and I was sent to the start up log-in interface.

### Windows 10 Pro (Workstation) Setup
  ![Screenshot 2024-11-23 180354](https://github.com/user-attachments/assets/1471993e-ef37-4b0c-a988-4471e3aba989)

  Selected the Windows ISO file for installation into the Virtual Machine set aside for my worksations.  
  
  ![Screenshot 2024-11-23 180457](https://github.com/user-attachments/assets/7b4b4dfa-cc1e-4e85-9631-878f8fd4fd7a)

  Allocated memory, and assigned processor cores to the virtual machine. 
  
  ![Screenshot 2024-11-23 180513](https://github.com/user-attachments/assets/b6778fa8-16fa-4b9b-87ed-65092ed1b33a)

  Installed the virtual machine with customized settings to my liking.

  ![Screenshot 2024-11-23 181254](https://github.com/user-attachments/assets/d35d2ef7-2d17-4674-90c7-d9b8c10823d5)

  Started up the Operating System installation process for Windows 10 Pro (workstations).

  ![Screenshot 2024-11-23 181438](https://github.com/user-attachments/assets/03084196-5a90-4bd1-b047-37d3d82ae8c4)

  Chose Windows 10 Pro as the operating system to be installed on this particular virtual machine.

  ![Screenshot 2024-11-23 181531](https://github.com/user-attachments/assets/d0d4afcd-c138-425d-9f60-71db056c0681)

  Partitioned the hard drive to provide overall performance and scallability options. 
  
  ![Screenshot 2024-11-23 181554](https://github.com/user-attachments/assets/fb14bbf5-78d3-4cd3-9209-dfcf6e462b18)

  The installation of the Windows 10 Pro operating system began.
  
  ![Screenshot 2024-11-23 182845](https://github.com/user-attachments/assets/27f4adfa-a8ef-4b38-85d5-bf80ea3463e5)

  Once the operating system compelted installing, I began to personalize the virtual machine's microsoft account. 
  
  ![Screenshot 2024-11-23 183107](https://github.com/user-attachments/assets/fc7f3e1c-3eca-4ecb-aa20-686ec5d4ccff)

  Set up a account that will be a administrator for this virtual machine. 
  - The installation proccess completed and I was sent to the start up log-in interface.


### Ubuntu Server Setup
  ![Screenshot 2024-11-23 174653](https://github.com/user-attachments/assets/f904ec06-e32a-4dea-9708-4ae51806eeab)

  Selected the Ubuntu Server ISO file for installation into the Virtual Machine set aside for my worksations.  
  
  ![Screenshot 2024-11-23 174741](https://github.com/user-attachments/assets/b64023a9-cec9-4e84-a98f-c288bb6392e9)

  Set up a Linux user that would be used to install the operating system.
  
  ![Screenshot 2024-11-23 175433](https://github.com/user-attachments/assets/324fee11-7af6-4857-a1ba-e0f78bd85cfb)

  Installed the virtual machine with customized settings to my liking.
  
  ![Screenshot 2024-11-23 180805](https://github.com/user-attachments/assets/280e6faa-146a-4d93-8443-7d0dd60bc79f)

  Started the installation proccess of the Ubuntu Server operating system.
  
  ![Screenshot 2024-11-23 180952](https://github.com/user-attachments/assets/3c16a7a7-a94d-471d-978a-f7458c96f317)

  Made a user account that would be used for logging into the server.
  
  ![Screenshot 2024-11-23 181033](https://github.com/user-attachments/assets/7f5efe43-17ac-49c4-a2d0-030d8675ffc8)

  Installed OpenSSH server package into the server to allow SSH to remote machines.
  
  ![Screenshot 2024-11-23 181121](https://github.com/user-attachments/assets/db5d4064-0a40-4c88-bc6b-3af1c19bede4)

  Installed the operating system with the setting preferences that I chose.
    - The installation proccess completed and I was sent to the start up log-in interface.


### Ubuntu Setup
  ![Screenshot 2024-11-23 200344](https://github.com/user-attachments/assets/9f319339-32f7-4cd1-abca-5cfe5fc0745c)

  Selected the Ubuntu ISO file for installation into the Virtual Machine set aside for my worksations.  

  ![Screenshot 2024-11-23 175054](https://github.com/user-attachments/assets/d9bd9c96-d768-40e8-8b29-909d4521990f)

  Set up a user that would be used to install the operating system.
  
  ![Screenshot 2024-11-23 175154](https://github.com/user-attachments/assets/6f6d0c20-f566-4661-87c2-84b5a0ddeb32)

  Installed the virtual machine with customized settings to my liking.
  
  ![Screenshot 2024-11-23 175613](https://github.com/user-attachments/assets/3c3fc66f-d621-4055-845a-ad0dd6111ab6)

  Chose the deafult installation of the Ubuntu operating system. 
  
  ![Screenshot 2024-11-23 180151](https://github.com/user-attachments/assets/1330af93-9df2-47b3-9291-d22f8fe02645)

  Set up a user account for Ubuntu.
    - The installation proccess completed and I was sent to the start up log-in interface.

## Configuring Windows Server 2019 to a domain 
  ### Careating an Active Directory domain
  ![Screenshot 2024-11-23 203245](https://github.com/user-attachments/assets/45fe1317-d947-4a8d-b4df-b8a1901ebf08)

  Used the command line to find my network settings and configuration

  ![Screenshot 2024-11-23 204956](https://github.com/user-attachments/assets/2a54c1ec-087e-428a-8061-018e0a31dedb)

  Added a static IP addres with the alternate DNS server addres being the same, to allow this host to be promoted to Domain. 

  ![Screenshot 2024-11-23 205447](https://github.com/user-attachments/assets/d73e319c-b2fa-4bc4-b2b3-c902f5ff1670)

  Manage my server to install roles and features as role based.

  ![Screenshot 2024-11-23 205534](https://github.com/user-attachments/assets/6c7a9042-042c-466e-a9bf-b4413bd2efe7)

  Added AD Domain Services and DNS Server roles to the server.

  ![Screenshot 2024-11-23 205558](https://github.com/user-attachments/assets/6c10bc20-d2af-47ec-98ff-65c8ce243982)

  Doubble checked to make sure Group Policy Managment features were still selected.

  ![Screenshot 2024-11-23 205701](https://github.com/user-attachments/assets/824396b3-5686-4291-8abf-e768a9ef000b)

  Installed the roles and features that I selected. 
  
  ![Screenshot 2024-11-23 210525](https://github.com/user-attachments/assets/3a00963c-691c-45b5-b533-7bf153dba514)

  After deploying the AD Domain Services I am now able to promote the server to a domain controller.
  
  ![Screenshot 2024-11-23 210938](https://github.com/user-attachments/assets/23541d1a-511f-428b-9ea7-02e0247684fc)

  Giving the domain (under a new forest) a root name with the .local naming convention.

  ![Screenshot 2024-11-23 211319](https://github.com/user-attachments/assets/f3cf5889-943a-413b-8917-949734ba5c68)

  Left the rest of the settings as default when proceding with the domain promoiton.
    
  - Allowed the promotion operation to complete.
    
  ![Screenshot 2024-11-23 212225](https://github.com/user-attachments/assets/d1d3c307-542e-4eb6-840e-c4e3add71ca1)
  The server has now been promoted. 
  
## Used network topology, commands, and concepts to connect each VM to the domain.
  Used ipconfig/ifconfig to get the Ips of each virtual machine.
  - Used sudo to install net-tools for Ubuntu desktop & server.
    ```
    sudo apt install net-tools

### Joining my Ubuntu desktop to the Domain 

![Screenshot 2024-11-23 234707](https://github.com/user-attachments/assets/efc38c49-f81e-42a8-95b0-d2d438cc068b)

Added my domain IP as the DNS Server address for my Ubuntu desktop.

sudo service NetworkManager restart

sudo apt install -y realmd libnss-sss libpam-sss sssd sssd-tools adcli samba-common-bin oddjob oddjob-mkhomedir packagekit

-Installed realmd packages that allow my Ubuntu desktop to connect to my domain controller.

hostnamectl set-hostname ubuntu.portfolio.local

-Changed the host name on my Ubuntu desktop.

systemctl disable systemd-resolved.service
systemctl stop systemd-resolved.service

-Disableing the systemd resolve service, so our domain server can resolve the DNS. 

![Screenshot 2024-11-24 001231](https://github.com/user-attachments/assets/3673c437-5b39-4199-9fbf-d96979a9e6df)

-Configured the resolv.conf file to point to the domnain controller with nano. 

 ### Created foward lookup zones for the Windows Pro, and Ubuntu VMs to add to my domain 
 ![Screenshot 2024-11-23 215517](https://github.com/user-attachments/assets/1faa15e7-c699-47cd-94aa-888987457e36)

 Accessed the DNS Manager thorugh the tools section of the Server Manager.
 
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

  Accessed the DNS Manager thorugh the tools section of the Server Manager.
 
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

A problem I am running into right now is that my workstation can reach my domain, but my domain can't find the workstaion.
- I then tried my Ubuntu desktop virtual machine and my domain was able to find it. 
- I trouble shooted this problem by turning off the workstations firewall, and that let me know were to find a solution.
  
![Screenshot 2024-11-23 231808](https://github.com/user-attachments/assets/34ba4c14-35f5-4b6c-9915-e3b5ff3d9219)

To solve this problem, I made a Inbound Protocol ICMPv4 rule , to allow incomming ping requests from all IPs.
- I was then able to ping the workstation.



   



  



