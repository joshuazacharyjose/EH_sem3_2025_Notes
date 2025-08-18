# Installation and Setting up of Kali Linux on Windows 11, using VirtualBox

The following **_instructions_** are to **install** and **set up** the _files_ required to run a ***virtual desktop*** of **_Kali Linux_** needed for your _cybersecurity practices_. Follow each step ***carefully*** to perfectly set up Kali in _VirtualBox_.

> [!NOTE]
> There are certain prerequisites and system requirements to keep in mind 
when wanting to establish a virtual connection of Kali in your system, 
as mentioned below:
> 
> ## Kali Linux VirtualBox System Requirements
> 
> Run Kali Linux smoothly on your Windows machine using VirtualBox by ensuring the following system requirements.
> 
> <hr>
> 
> ### ֎ Minimum System Requirements
> 
> | Component          | Requirement                                           |
> |-------------------|-------------------------------------------------------|
> | **Host OS**       | Windows 7 or later (64-bit recommended)               |
> | **RAM**           | 2 GB for Kali VM (at least 4 GB total on host)        |
> | **CPU**           | Dual-core processor (VT-x or AMD-V enabled)           |
> | **Storage**       | 20 GB free disk space                                 |
> | **VirtualBox**    | Version 6.x or later                                  |
> 
> <hr>
> 
> ### ֎ Recommended System Requirements
> 
> | Component          | Requirement                                           |
> |-------------------|-------------------------------------------------------|
> | **Host OS**       | Windows 10/11 (64-bit)                                |
> | **RAM**           | 4 GB for Kali VM (8 GB or more on host)               |
> | **CPU**           | Quad-core processor with virtualization support       |
> | **Storage**       | 40–60 GB free disk space (SSD strongly recommended)   |
> | **VirtualBox**    | Latest version (7.x or higher)                        |
> | **Graphics**      | GPU with 3D acceleration support (optional)           |
> 
> <hr>
>
> ## Prerequisites to Configure
>
>- **<ins>Virtualization Support</ins>**: Enable **VT-x** (Intel) or **AMD-V** (AMD) in BIOS/UEFI
>- **<ins>Admin Access</ins>**: Required to install and configure VirtualBox and BIOS settings
>- **<ins>Stable Internet Connection</ins>**: For downloading Kali and VirtualBox images
>- **<ins>Allocation of System Resources</ins>**: Allocate at least **2 CPUs** and **4 GB RAM** to the Kali virtual machine
>- **<ins>Regular Updation</ins>**: Keep **VirtualBox and Kali updated** regularly for security and performance

<hr>

- ## Step 1: Download and Install VirtualBox
  - Visit the official [VirtualBox](https://virtualbox.org) website.
  - Download the preffered installer (for my system, it was Windows).
  - Run the setup and install the software, as per the instructions.

    <img width="1860" height="1034" alt="Screenshot 2025-07-22 052559" src="https://github.com/user-attachments/assets/119e3efe-13e6-40a9-ba0c-0b8cdfb79794" />

    <hr>

- ## Step 2: Download the required Kali Linux files
  - Visit the official [Kali Linux](https://www.kali.org/) and click on Download.
  - In the '_Choose You Platform_' page, select ***Virtual Machines***.
  - Here, click on the download icon under '_VirtualBox_' (the file size is apporximately 3.3 GB).
 
    <img width="1853" height="1037" alt="Screenshot 2025-07-22 053554" src="https://github.com/user-attachments/assets/8eb1b050-7a3f-448e-b2f5-9ab52e87e6b8" />

- ## Step 3: Extract the Kali Linux files
  - After downloading has finished, extract the **`.7z`** file using [7-Zip](https://www.7-zip.org) or [WinRAR](https://www.win-rar.com).
  - Now, there are two files to keep note of:
    1. **`.vdi` <ins>(Virtual Disk Image)</ins>:** Contains the virtual hard drive of Kali Linux.
    2. **`.vbox` <ins>(VirtualBox Machine Definition)</ins>:** Stores the required virtual machine configuration.

   <br> 
  <img width="583" height="317" alt="Screenshot 2025-07-22 055203" src="https://github.com/user-attachments/assets/70ff6abc-751b-4d82-8f99-f89ff24aaa73" />

> [!TIP]
> Since you have VirtualBox installed, just double-click the **`.vbox`** file to automatically get started with the Kali VM in VirtualBox.

  <hr>
  
- ## Step 4: Enable required Windows features _(required for Windows users)_
  Before going ahead with the initialization of the VM, certain features in Windows are to be enabled:

  - Open **Control Panel → Programs → Turn Windows features on or off**.
  - Enable the following features:
    - **Virtual Machine Platform**
    - **Windows Hypervisor Platform**
  - Click **OK** and then restart the machine.
 
    <img width="546" height="489" alt="Screenshot 2025-07-22 055803" src="https://github.com/user-attachments/assets/d4e99ab9-208e-4a96-a7d8-120201e9a6af" />

  <hr>

- ## Step 5: Launch and configure the Kali Linux VM
  - In the folder where Kali files are extracted, open the **`.vbox`** file by double-clicking it.
 
    <img width="1909" height="1079" alt="Screenshot 2025-07-22 060534" src="https://github.com/user-attachments/assets/bb7c5567-b736-42d9-948b-701c99cfc3ce" />

  - Here, in the VirtualBox software, click on **Settings**.
  - Under the **System** subsection, allocate the required RAM and CPU cores for Kali to run smoothly
    <br>
    <img width="680" height="137" alt="Screenshot 2025-07-22 070229" src="https://github.com/user-attachments/assets/5f4f7214-0c98-4c60-8126-b9a5020a82bf" />
    <img width="664" height="130" alt="Screenshot 2025-07-22 070240" src="https://github.com/user-attachments/assets/30dfe1ea-7b5e-4056-916a-e5cff5176da3" />
    
> [!WARNING]
> Make sure at least the minimum system requirements are met, and that enough resources are allocated for the smooth performance of your main machine as well.

  - Click on 'Start' to initialize the VM and wait patiently.

    <img width="1919" height="1079" alt="Screenshot 2025-07-22 071055" src="https://github.com/user-attachments/assets/feab18e1-b422-4c46-8e0f-b5140263732b" />
  - At the login screen, enter the 'Username' and 'Password' as _`kali`_,  and click on 'Log In'.

    <img width="1919" height="1079" alt="Screenshot 2025-07-22 071317" src="https://github.com/user-attachments/assets/ecfc5cad-c108-4a7b-8c8a-3738bc6c9aa4" />

  
