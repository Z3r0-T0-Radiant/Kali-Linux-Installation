# Setting Up Kali Linux
This guide provides instructions for installing and configuring Kali Linux using VirtualBox. The process includes system preparation, creating a virtual machine, and completing the installation.

## 1. Introduction to Kali Linux
Kali Linux is a Debian-based Linux distribution designed for security auditing, penetration testing, and ethical hacking. Developed by Offensive Security, it includes over 600 preloaded security tools. It is widely used for tasks such as testing network vulnerabilities, conducting digital forensics, and learning cybersecurity concepts.
Some commonly used tools are:
•	Nmap: Network scanning
•	Metasploit: Exploit development
•	Wireshark: Traffic analysis

## 2. Preparing for Installation
Requirements
1.	A compatible system with at least 4GB of RAM and 40GB of disk space.
2.	A virtual machine manager such as VirtualBox, VMware, Hyper-V (for Windows), or Parallel Desktop (for macOS). This guide uses VirtualBox.
3.	The Kali Linux ISO image, available on the official website. Download the Kali Linux 2024.3 Installer ISO from the "Installer Images" section.
4.	
Preparation Steps
1.	Install VirtualBox: 
o	Search for "VirtualBox" in a browser.
![image](https://github.com/user-attachments/assets/38d709f2-9bac-450d-82dd-4df3c7d242a8)

o	Download and install VirtualBox by following the provided instructions.	![image](https://github.com/user-attachments/assets/4127fb4a-4f04-4ec7-81a3-4526bcf9c160)

2.	Download Kali Linux ISO: 
o	Navigate to the Kali Linux official website.
![image](https://github.com/user-attachments/assets/d31eccde-3fa5-4c54-a65c-8aaa7d4468e5)
o	Download the Kali Linux 2024.3 Installer ISO.
![image](https://github.com/user-attachments/assets/5516a267-4fde-497c-812b-005c6c97bea1)

## 3. Installing Kali Linux
### Step 1: Create a Virtual Machine
Open VirtualBox and select Machine > New.

Specify the name of the virtual machine.
Input the Kali Linux installer ISO file.


### Step 2: Configure the Virtual Machine
1.	Set up virtual hardware: 
o	RAM: Allocate 5112MB (adjust based on system capacity).
o	CPUs: Assign 4.
o	 
o	Storage: Allocate at least 20GB (50GB is recommended).
o	 
2.	Adjust additional settings: 
o	Set both Shared Clipboard and Drag’n’Drop  to bidirectional.
o	 
o	Maximize video memory.
o	 
o	Check the ISO file under the storage settings.
o	 
o	Configure the network adapter to NAT or Bridged Adapter for host-system interaction.  
### Step 3: Complete the Installation
1.	Start the virtual machine and select Graphical Install.  
2.	 
3.	Follow the installation steps: 
o	Choose the language, location, and keyboard layout.
o	Specify the hostname (e.g., kaliMachine) and leave the domain name empty.
o	 
o	 
o	Set up the full name, username, and password.
o	  
o	Use guided disk partitioning for beginners.
o	   
o	Confirm partitioning by selecting Finish partitioning and write changes to disk.  
o	 
o	Install the base system and software packages.
o	 
o	Install GRUB bootloader on /dev/sda.
o	  
o	 
##4.	Reboot the virtual machine after installation.
Post-Installation Setup
1.	Adjust the screen resolution in the display settings.
2.	Open a terminal and run the following commands to update and upgrade the system: 
3.	sudo apt update  
4.	sudo apt upgrade  
5.	to upgrade software application in Kali Linux
________________________________________
Kali Linux is now ready for use in cybersecurity learning and penetration testing.

