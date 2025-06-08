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
### 3. Download Windows 11 ISO 
-	Visit Microsoft Evaluation Center https://www.microsoft.com/en-us/evalcenter 
-	Select windows 11 Enterprise and click on evaluate now

![Windows 11](https://github.com/Judeorabueze/Windows-11-Virtual-Homelab-Setup/blob/main/Windows%2011.png)

-	Click on Download the ISO - Window 11 enterprise
  (NOTE: This is an evaluation version and may be free to use for a period of 90days and may have some limitations)
- Complete the Free Trial form and click download.
- Select the appropriate Windows 11 Enterprise and Language
  (In my case, English (United States) ; 64-bit version was selected)
- Click on download.

![Windows 11](https://github.com/Judeorabueze/Windows-11-Virtual-Homelab-Setup/blob/main/Windows%2011B.PNG)

Allow some minutes or hours to complete the download.
##
### 4. Install and configure Windows 11 ISO in Oracle VirtualBox
-	Open the VirtualBox already installed in the host machine
-	On the tools section, click on new and give a name to the Virtual Machine to be installed. (In my case, Windows 11. You can give yours a different name)
-	Specify the folder (path) for the VirtualBox ( ...user\VirtualBox VMs)
-	On ISO Image, click other and select the windows 11 file that was downloaded

![VM](https://github.com/Judeorabueze/Windows-11-Virtual-Homelab-Setup/blob/main/VM%201.PNG)

-	Click on Skip unattended installation and click next
-	Allocate resources for the VM and click on next. (For better experience it is recommended to increase the default depending on the available resources In the computer.

![VM](https://github.com/Judeorabueze/Windows-11-Virtual-Homelab-Setup/blob/main/VM2.png)

-	Check the Enable EFI box ( This is important because VirtualBox does not have Secure Boot enabled by default which is required by Windows 11)
Failure to check this may cause the windows11 not to install
-	Leave the Hard Disc setting on default and click on finish.

![VM3](https://github.com/Judeorabueze/Windows-11-Virtual-Homelab-Setup/blob/main/vm%203.png)

Windows 11 ISO has been added to VirtualBox and is visible on the left "New group" panel of the Oracle VirtualBox.
-	Click on the VM (Windows 11) and then click start, to start installation.
-	Press any key to boot the Windows 11 Virtual machine.
-	Select Language and continue.


- Created a new VM and adjusted settings (EFI, resources)
- Enabled drag & drop and clipboard sharing
- Installed VirtualBox Guest Additions for improved VM integration
- Took and restored VM snapshots as a backup solution


## Lessons Learned
- Gained hands-on experience with BIOS configuration and virtualization setup  
- Understood the installation and configuration process for VirtualBox and Windows 11  
- Learned how to manage VM snapshots for quick recovery  
- Improved virtual lab management skills for future cybersecurity or IT training  

