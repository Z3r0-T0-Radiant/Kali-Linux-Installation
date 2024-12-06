# Setting Up Kali Linux
This guide provides instructions for installing and configuring Kali Linux using VirtualBox. The process includes system preparation, creating a virtual machine, and completing the installation.

## 1. Introduction to Kali Linux
Kali Linux is a Debian-based Linux distribution designed for security auditing, penetration testing, and ethical hacking. Developed by Offensive Security, it includes over 600 preloaded security tools. It is widely used for tasks such as testing network vulnerabilities, conducting digital forensics, and learning cybersecurity concepts. Some commonly used tools included Nmap (Network scanning), Metasploit (Exploit development) and Wireshark (Traffic analysis).

## 2. Preparing for Installation
### Requirements
1.	A compatible system with at least 4GB of RAM and 40GB of disk space.
2.	A virtual machine manager such as	VirtualBox, VMware, Hyper-V (for Windows), or Parallel Desktop (for macOS). This guide uses VirtualBox.
3.	The Kali Linux ISO image, available on the official website. Download the Kali Linux 2024.3 Installer ISO from the "Installer Images" section.

### Preparation Steps
#### Install VirtualBox:

1. Search for "VirtualBox" in a browser.
![image](https://github.com/user-attachments/assets/d4ca8276-fb25-4ff8-80af-8d72facf174e)


2. Download and install VirtualBox by following the provided instructions.	
![image](https://github.com/user-attachments/assets/9699a145-8cb3-4076-86b5-1dbffd23aad7)


#### Download Kali Linux ISO: 
1. Navigate to the Kali Linux official website.
![image](https://github.com/user-attachments/assets/2bab9978-a13b-4194-b36e-fe1a48e45746)

2. Download the Kali Linux 2024.3 Installer ISO.
![image](https://github.com/user-attachments/assets/57028f5b-1152-4848-9f9b-9b4384c97dd0)

## 3. Installing Kali Linux
### Step 1: Create a Virtual Machine
1. Open VirtualBox and select Machine > New.
![image](https://github.com/user-attachments/assets/f0edb50e-51bf-4b11-bc89-2a5bd135dd57)

2. Specify the name of the virtual machine and input the Kali Linux installer ISO file.
![Screenshot 2024-12-04 185247](https://github.com/user-attachments/assets/de9fc41e-3e8b-4955-a287-6d9e695731fd)

### Step 2: Configure the Virtual Machine

1. **RAM:**  Allocate 5112MB (adjust based on system capacity).
2. **CPUs:**  Assign 4.
![image](https://github.com/user-attachments/assets/3469fd74-7fae-43cf-9e7b-2c7d82d9b05f)
	 
3. **Storage:** Allocate at least 20GB (50GB is recommended).
![image](https://github.com/user-attachments/assets/9189beea-1829-4efd-a766-79d37e32dde8)

4. Set both **Shared Clipboard and Drag’n’Drop** to bidirectional.
![Screenshot 2024-12-06 155935](https://github.com/user-attachments/assets/1039df7d-2721-4df3-929b-0416e9a9b9c8)

5. **Maximize** video memory.
![image](https://github.com/user-attachments/assets/a189c08b-611e-488c-9d66-b41b6a1c4217)

6. Check the **ISO file** under the storage settings.
![Screenshot 2024-12-06 160023](https://github.com/user-attachments/assets/1ebe9431-145b-4923-be9f-4ce03fcb4898)

7. Configure the network adapter to **NAT or Bridged Adapter** for host-system interaction.  
![image](https://github.com/user-attachments/assets/f69b54ea-d9e3-4e42-a99e-d046a1c17618)

### Step 3: Complete the Installation
1.	Start the virtual machine and select Graphical Install.  
![image](https://github.com/user-attachments/assets/2e951508-b04e-4ca8-8fdc-4d29c6a2a030)
![image](https://github.com/user-attachments/assets/40adfa38-93fe-4613-85f7-1c0d4f4a558a)

2. Choose the language, location, and keyboard layout.
3. Specify the hostname (e.g., kaliMachine) and leave the domain name empty.
![image](https://github.com/user-attachments/assets/dc192191-a333-4622-a043-442c83ad0311)

4. Set up username, and password.
![image](https://github.com/user-attachments/assets/15ab5e5d-d40d-4475-b020-30d0e5d993d5)
![image](https://github.com/user-attachments/assets/527d0513-cc3a-4cfc-b886-1af773c96452)


5. Use guided disk partitioning for beginners.
![image](https://github.com/user-attachments/assets/e63a6dd6-5ef3-4e4a-b687-c6810fedc1a1)
![image](https://github.com/user-attachments/assets/5d4d871e-faed-4998-a90e-88e018c03062)
![image](https://github.com/user-attachments/assets/cae2becf-7de0-419c-95c7-df1bf1bf67bf)

6. Confirm partitioning by selecting Finish partitioning and write changes to disk.  
![image](https://github.com/user-attachments/assets/9b553d03-f796-45ba-b523-b894d2a199ff)
![image](https://github.com/user-attachments/assets/00b4a607-2f55-4ef8-a749-1c387fe760ec)

7. Select the checkbox option as below.
![image](https://github.com/user-attachments/assets/5d6bc450-bff8-4feb-84fe-6676b6c094c0)

8. Install GRUB bootloader on /dev/sda.
![image](https://github.com/user-attachments/assets/184dff3b-3de6-449b-a065-ab0df78e2ae8)
![image](https://github.com/user-attachments/assets/0258e5a3-050e-4896-8cf4-6daeeb8b5ea8)

9. Reboot the virtual machine after installation.

## Post-Installation Setup
1.	Adjust the screen resolution in the display settings.
![Screenshot 2024-12-06 162503](https://github.com/user-attachments/assets/004fe410-cdea-4279-853d-b036bab5c81f)
2.	Open a terminal and run the following commands to update and upgrade the system: 

```
sudo apt update  
sudo apt upgrade
```

![Screenshot 2024-12-06 162759](https://github.com/user-attachments/assets/57da5a28-967b-447d-8d40-770f077a62b3)


Kali Linux is now ready for use in cybersecurity learning and penetration testing.

