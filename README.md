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
- Check if the host system is visualization enabled:
   -	Right click on the task bar of the the host machine.
   -	Navigate to the task manager.
   -	Click on performance and then CPU.

![Image](https://github.com/user-attachments/assets/9fc86f4c-73de-4934-a3a5-249766e840af)

- Installed Oracle VirtualBox on a Windows host
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

