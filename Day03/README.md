# Linux Commands and Installation of Visual Studio Code in Kali Linux
- ## Familiarisation of Some Linux Commands
  There are some **important** _Linux commands_ that we have used in the _terminal_ in ***Kali Linux***, in which we could handle _files_ and _their permissions_, _move through directories_, et cetera. 

   Below is a **table** of all the _commands_ we _tested_ in the terminal :-

  | Command Keyword | Purpose of Command                                    |
  | --------------- | ----------------------------------------------------- |
  | `ls`            | To list directory contents                            |
  | `cd`            | To change the directory                               |
  | `touch`         | To create a new empty file                            |
  | `echo`          | To send a message in the terminal                     |
  | `man`           | To display the manual for commands                    |
  | `ls -lh`        | To list directory contents in a human-readable format |
  | `cp`            | To copy the files or directories as a whole           |
  | `mv`            | To move / rename files or directories                 |
  | `chmod`         | To change certain file permissions                    |


> [!CAUTION]
> Keep in mind to be cautious when exploring the many commands of Linux, as some might entirely mess up the installation of Kali Linux, leading to a reinstallation.
---

- ## Installing and Setting Up Visual Studio Code in Kali Linux
  The following steps are to instruct the user into downloading and installing Visual Studio Code (VSCode) into Kali Linux, using Firefox in Kali Linux itself.

  1. Go to the official website of [Visual Studio Code](https://code.visualstudio.com/) and click on 'Other Platforms'. 
  2. Once in this page, download the `.deb` file, and store it somewhere accesible (like Downloads). <br>
     <img width="1856" height="1033" alt="Screenshot 2025-07-24 230535" src="https://github.com/user-attachments/assets/8a5756e9-1b2b-4033-9640-ec03c44a2675" />
  3. After downloading the file, open up the terminal.<br>
     <img width="1920" height="1080" alt="VirtualBox_kali-linux-2025 2-virtualbox-amd64_24_07_2025_23_08_47" src="https://github.com/user-attachments/assets/b0ca845f-e6e6-4bfb-a98d-55132c6b560b" />
  4. Now type `cd Downloads` to move to the Downloads directory and then `ls` to list the content present there.<br>
     <img width="1920" height="1080" alt="VirtualBox_kali-linux-2025 2-virtualbox-amd64_24_07_2025_23_10_56" src="https://github.com/user-attachments/assets/748bdecb-bb30-4ed4-a385-56de875270b8" />
  5. To install the package, type `sudo apt install ./code_1.102.2-1753187809_amd64.deb` and press Enter.<br>
     <img width="1920" height="1080" alt="VirtualBox_kali-linux-2025 2-virtualbox-amd64_24_07_2025_21_49_05" src="https://github.com/user-attachments/assets/e19dcad0-aa61-427e-aab3-33de7c95b894" /><br>
     <img width="1920" height="1080" alt="VirtualBox_kali-linux-2025 2-virtualbox-amd64_24_07_2025_21_54_22" src="https://github.com/user-attachments/assets/0bf14e58-a4cf-42b5-93ce-c2d0e0a7966f" />
  6. After installation, type `code` to launch VSCode from the terminal or open it from the start menu.<br>
     <img width="1920" height="1080" alt="VirtualBox_kali-linux-2025 2-virtualbox-amd64_24_07_2025_21_54_51" src="https://github.com/user-attachments/assets/0b8ee21c-0ae0-4b12-95ba-aafa54139d2b" />

     You can now run VSCode inside of Kali.

---

- ## How to Upgrade Kali to the Latest Version

  At times, it is needed to upgrade to the most recent version of Kali Linux to install certain modules, payload, packages, et cetera:- for our cybersecurity practices. Here is a step-by-step guide on safely upgrading Kali Linux.

  - First off, check your APT source list to ensure you're on the rolling release:

  ```bash
  sudo nano /etc/apt/sources.list
  ```
  - Now, you should replace the content with:

  ```bash
  deb http://http.kali.org/kali kali-rolling main non-free non-free-firmware contrib
  ```
  

  1. ###  Check Current Kali Version
     
  ```bash
  lsb_release -a
  ```

  2. ###  Update Package List
     
  ```bash
  sudo apt update
  ```

  3. ###  Upgrade Installed Packages
  For a regular upgrade, which is safer to do than a full upgrade:
  
  ```bash
  sudo apt upgrade -y
  ```
  > <ins>Note:</ins> For a full-scale distribution upgrade, which is usually recommended to resolve any conflicts when installing certain packages, you can run the following command:
  > ```bash
  > sudo apt full-upgrade -y
  > ```

  4. ###  Remove Unused Packages

  ```bash
  sudo apt autoremove -y
  ```

  5. ### Ensure Core Kali Tools are installed
 
  ```bash
  sudo apt install -y kali-linux-default
  ```

  6. ### Reboot Kali Linux
 
  ```bash
  sudo reboot
  ```
