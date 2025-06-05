# Windows 11 Virtual Home Lab Setup

## Description
This project demonstrates how to set up a Virtual Home Lab using Oracle VirtualBox and Windows 11, with step-by-step guidance on enabling system virtualization, installing VirtualBox, setting up a Windows 11 VM, and managing snapshots.

## Tools Used
- Oracle VirtualBox
- Windows 11 ISO (Evaluation Edition)
- Host Machine (Windows OS with virtualization support)

## What I Did
### 1. Enable System Visualization ( Host – Windows system )
  To run VirtualBox (type 2 hypervisor) effectively, virtualization technology (VT-x or AMD-V) must be enabled in the host machine BIOS/UEFI settings.
- Ensure the host system is visualization enabled:
   -	Right click on the task bar of the the host machine.
   -	Navigate to the task manager.
   -	Click on performance and then CPU.

![Virtualization Enabled](https://github.com/Judeorabueze/Windows-11-Virtual-Homelab-Setup/blob/main/Visualization%20enabled.jpg)

From the screenshot above, the host system is visualization enabled.
##
### 2. Download and Install a VirtualBox
-	Visit https://www.virtualbox.org/wiki/Downloads
-	Select the appropriate VirtualBox platform package (In this case, Windows) 
-	Click the host (Windows) and allow to download.

![VirtualBox](https://github.com/Judeorabueze/Windows-11-Virtual-Homelab-Setup/blob/main/Virtualbox%201.png)

-	Double-click on the downloaded VirtualBox win.exe 
-	Allow the app to make changes on the host computer – click on yes
-	Oracle VirtualBox setup windows installer pop-up – click on next

![VirtualBox](https://github.com/Judeorabueze/Windows-11-Virtual-Homelab-Setup/blob/main/Virtualbox%202.png)

-	Accept the user agreement
-	On the custom setup box, select VirtualBox Application and click on Next

![VirtualBox](https://github.com/Judeorabueze/Windows-11-Virtual-Homelab-Setup/blob/main/Virtualbox%203.png)

-	On the network interfaces warning , click on yes
-	Missing dependencies box, click on yes
-	Follow the installation prompts, click yes on ready for installation and allow for the installation to be completed.

![VirtualBox](https://github.com/Judeorabueze/Windows-11-Virtual-Homelab-Setup/blob/main/Virtualbox%204a.png)

-	Click on Finish to complete the installation.
-	Open the installed Oracle virtualBox.

![VirtualBox](https://github.com/Judeorabueze/Windows-11-Virtual-Homelab-Setup/blob/main/Virtualbox%205.png)

Installation is completed and the screenshot above shows that the hypervisor (Oracle VirtualBox) is running smoothly on the host Windows OS. 
##
### 3. Installation of a Windows Virtual Machine (Windows 11)

- Downloaded and installed Windows 11 ISO (Enterprise Evaluation)
- Created a new VM and adjusted settings (EFI, resources)
- Installed and configured Windows 11 in the VM
- Enabled drag & drop and clipboard sharing
- Installed VirtualBox Guest Additions for improved VM integration
- Took and restored VM snapshots as a backup solution

## Screenshots
![Virtualization Enabled](screenshot1.png)  
![VirtualBox Installed](screenshot2.png)  
![Windows 11 Running on VM](screenshot3.png)  
![Snapshot Taken](screenshot4.png)

## Lessons Learned
- Gained hands-on experience with BIOS configuration and virtualization setup  
- Understood the installation and configuration process for VirtualBox and Windows 11  
- Learned how to manage VM snapshots for quick recovery  
- Improved virtual lab management skills for future cybersecurity or IT training  

