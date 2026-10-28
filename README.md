# Setting-up-My-Kali-Linux-virtual-machine-

Kali Linux Virtual Machine Setup Guide
A step-by-step guide to installing, configuring, and preparing Kali Linux on Windows using Oracle VirtualBox.

     Project Overview
This project documents the process of setting up a Kali Linux virtual machine for learning Linux commands, networking, cybersecurity, and ethical hacking in a controlled laboratory environment.

     Objectives
Install Oracle VirtualBox on Windows.
Download and import the official Kali Linux virtual machine.
Configure RAM, CPU, display, and network settings.
Update and upgrade Kali Linux.
Configure internet connectivity.
Improve display resizing and mouse integration.
Create snapshots for recovery.
Install and explore cybersecurity tools.
  
     Requirements
     
Windows 10 or Windows 11 (64-bit)
Intel VT-x or AMD-V virtualization support
Oracle VirtualBox
7-Zip for extracting the downloaded archive
Official Kali Linux VirtualBox image
Internet connection
At least 40–60 GB of available disk space recommended
Recommended Virtual Machine Configuration
Component	Recommended setting
RAM	2–4 GB
CPU	2 cores
Video memory	128 MB
Virtual disk	40–80 GB
Network adapter	NAT
Adjust these settings according to your computer's available resources.

     Installation Steps
     
1. Download VirtualBox
Download and install Oracle VirtualBox from:

https://www.virtualbox.org/wiki/Downloads

2. Download Kali Linux
Download the prebuilt VirtualBox image from the official Kali Linux website:

https://www.kali.org/get-kali/#kali-virtual-machines

3. Extract the Virtual Machine
Install 7-Zip from:

https://www.7-zip.org/

Extract the downloaded Kali Linux .7z archive.

4. Import Kali Linux
Open VirtualBox.
Select Add from the available machine management options.
Browse to the extracted folder.
Select the .vbox configuration file.
Configure the virtual machine resources.
Select the VM and click Start.
5. Log In
For the official prebuilt image, the default credentials are generally:

Username: kali
Password: kali
Change the default password after your first login.

     Initial Configuration
Change Password
passwd
Update Package Lists
sudo apt update
Upgrade Installed Packages
sudo apt full-upgrade -y
Restart the System
sudo reboot

    Network Configuration
Configure the VirtualBox network adapter to use NAT for basic internet access.

Check network interfaces:

ip addr
Check routing:

ip route
Test internet connectivity:

ping -c 4 1.1.1.1
Test DNS resolution:

ping -c 4 google.com

     Useful Linux Commands
Command	Description
pwd	Display the current directory
ls -la	List files and directories
cd Documents	Navigate to a directory
ip addr	Display network interfaces
df -h	Check available disk space
free -h	Display memory usage
nmap --version	Check the installed Nmap version
Install Nmap if needed:

sudo apt install nmap
    
     Create a Virtual Machine Snapshot
After completing the installation and updates:

Open VirtualBox Manager.
Select your Kali Linux virtual machine.
Open the Snapshots view.
Select Take Snapshot.
Name it Clean Kali Installation.
Snapshots allow you to restore a previous VM state after configuration changes or failed experiments. Keep separate backups of important files.

     Security and Ethical Use
Use Kali Linux tools only on systems you own or have explicit authorization to test.

For practice, use isolated virtual networks and intentionally vulnerable training machines. Avoid testing public systems without permission.

     Official Resources
Kali Linux Downloads
Kali Linux Documentation
Kali VirtualBox Installation Guide
Oracle VirtualBox Downloads
7-Zip Downloads
    
     Project Status
[x] Installation procedure documented
[x] Recommended VM configuration documented
[x] Network configuration documented
[x] Essential commands documented
[x] Security guidelines included
[ ] Installation tested and screenshots added
[ ] Cybersecurity lab exercises documented

     Author

JOSEPH MATABARO INNOCENT
Created as a personal learning project to develop practical skills in Linux administration, networking, and cybersecurity.

<img width="1919" height="1079" alt="88275" src="https://github.com/user-attachments/assets/dd4f15f1-f649-4b2f-b11e-2b7e7c9a8c78" />
<img width="1550" height="803" alt="88276" src="https://github.com/user-attachments/assets/6f5051f4-f4cf-4a69-b1f4-00a7d000e27d" />
<img width="1919" height="1076" alt="Screenshot_2026-10-28_04-45-56" src="https://github.com/user-attachments/assets/c4ad5062-993b-4b34-9992-12fea3df58ff" />


