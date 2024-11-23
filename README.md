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

•	Set up multiple servers through VMs, including Windows Server 2019, Windows Pro, Ubuntu, and Ubuntu Server.
-	Downloaded a ISO file for each OS to be assigned to a VM
-	Specified a set amount of memory and cores to be assigned to each VM
-	Went through and fully installed each OS while completing the accounts setup required

•	Set up the domain by configuring the Windows Server 2019.
- Added a static IP address to the host while making the primary DNS IP address the same address, to be able to promote the server to Domain
-	Installed Active Directory Domain Service with its roles and features through the server role setup
-	Installed DNS server through the server role setup
-	Created a root domain name to promote the server to a Windows Domain controller

•	Used network topology, commands, and concepts to connect each VM to the domain.
-	Used ipconfig/ifconfig to get the Ips of each system
-	Created forward and reverse lookup zones for the Windows Pro, and Ubuntu VMs to add to my domain
-	Used ping to test if the domain was able to reach the systems and vice versa
-	Joined Windows Pro system to the domain through it systems properties
 
-	Changed the Ubuntu system’s hostname to the domain name and installed realmd package on the system to join it to my domain

•	Set up remote desktop to gain remote access to my Windows Pro system from the Windows Domain.

•	Setup SSH to gain remote access from my Window domain into the Ubuntu client and server and vice versa.

•	Set up multiple accounts on a Windows Pro system through the Window Domain.
-	Created and organized unit with sub-organized units of containing different departments of a company
-	Created users in each of the sub-organized units and grouped them based on their department using security groups

•	Used active directory and group policies to manage the Window Domain.
-	Created a group policy through account policies in the security settings to limit the character length of a password to 12 minimum for users on the Windows Pro system
-	Created a group policy through software restriction policies in the security settings to restrict all users in the company form opening internet explorer

•	Used group policies for network file share to make a secure drive-map for the domain controller and departments within the organization to share files.
-	Created a drive map trough group policy to allow two distinct departments to share files with each other

•	Created a webpage by setting up WordPress with Linux.
-	Downloaded databases, Apache and WordPress packages onto the Ubuntu system
-	Created a database for WordPress setup configuration
-	Installed WordPress and accessed the account through my Ubuntu’s public Ip address

•	Created an Ubuntu server for system logging of the domain server with syslog.
-	Configured syslog in the Ubuntu server to run under the UDP syslog port
-	Configured syslog in the Ubuntu server to save the domain controller logs in a specified path while displaying it by hostname and program
-	Configured syslog in the Ubuntu client to find the location of the server, to send its log messages from the domain controller to the Ubuntu server

•	Made a bash script to search through logs to find logs for the domain controller and sudo logins on the Linux devices.

