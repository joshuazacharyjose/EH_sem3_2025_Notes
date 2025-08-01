#  Networks and its Related Terms

In these notes, we will be discussing mainly about **<ins>networks</ins>**, and the many _terminologies_ related to it, like **_subnet_**, **_IP/MAC address_**, **_TCP/UDP_**, etc:-, as well as its _correlation_ with _ethical hacking_.
- ## Network
  A network is a system of interconnected or related things, such as computers, devices, people, or organizations, that can communicate and share resources. In the context of computing, a network is a collection of devices that can communicate with each other to share data and resources. Networks enable the exchange of data, resources, and information, facilitating various applications like email, file sharing, and internet access. In fact, The Internet itself is a vast network of networks, connecting countless devices globally.

  <img width="1800" height="1210" alt="network_95" src="https://github.com/user-attachments/assets/56d90b4d-1120-4526-893d-88c1b99ebfee" />


  The different types of networks that we have come across in earlier classes are as follows:
    
  1. ### <ins>Local Area Network (LAN):</ins> <br>
 
     - A LAN connects devices within a limited geographical area, such as a home, office, or school. 
     - Typically used for sharing resources like printers, files, and internet access among connected devices. 

  2. ### <ins>Wide Area Network (WAN):</ins> <br>

     - A WAN spans a large geographical area, potentially across cities, countries, or even continents. 
     - Connects multiple LANs or other networks, often using leased lines or other telecommunication infrastructure. The internet is the most prominent example of a WAN. 
        
  3. ### <ins>Metropolitan Area Network (MAN):</ins> <br>

     - A MAN covers a larger geographic area than a LAN but smaller than a WAN, typically a city or a large metropolitan area. 
     - Connects multiple LANs within the city or metropolitan area. 
   
  4. ### <ins>Personal Area Network (PAN):</ins> <br>

     - A PAN is a network that connects devices within the range of an individual, typically a few meters. 
     - Examples include connecting a smartphone to a headset, or a computer to a printer. 
   
  6. ### <ins>Wireless Local Area Network (WLAN):</ins> <br>
  
     - A WLAN is a LAN that uses wireless communication (like Wi-Fi) to connect devices. 
     - Extends the reach of a LAN without the need for physical cables. 

  6. ### <ins>Virtual Private Network (VPN):</ins> <br>

     - A VPN creates a secure, encrypted connection over a public network (like the internet). 
     - Used to access private networks remotely or to enhance online security and privacy. 

  7. ### <ins>Storage Area Network (SAN):</ins> <br>
  
     - A SAN is a specialized network designed for high-speed access to storage devices. 
     - Often used in data centers and large organizations for centralized storage and data management. 

  8. ### <ins>Campus Area Network (CAN):</ins> <br>

     - A CAN is a network that connects multiple LANs within a limited geographical area like a university campus or a corporate complex. 
     - It can be seen as a larger version of a LAN or a smaller version of a MAN.

- ## Subnet
  A subnet, or subnetwork, is a logical subdivision of an IP network. Subnetting allows a large network to be broken down into smaller, more manageable networks, improving efficiency and organization. This segmentation helps to streamline network traffic and simplifies management. It offers several benefits like:
  - <ins>_Improved efficiency:_</ins> By dividing a network, traffic can be routed more directly, reducing congestion and improving network speeds.
  - <ins>_Simplified management:_</ins> Smaller subnets are easier to manage and troubleshoot than a single, large network.
  - <ins>_Enhanced security:_</ins> Subnets can be used to isolate different departments or groups within an organization, limiting access and improving security.
 
    <img width="1053" height="594" alt="network-subnetting-example-single-subnet-size" src="https://github.com/user-attachments/assets/f4ce3b13-ff34-49c8-b33c-cf7ac34e619a" />
- ## Internet Protocol Address (IP Address)
  An IP address, or Internet Protocol address, is a unique numerical label assigned to each device connected to a computer network that uses the internet protocol for communication. Essentially, it's a network address that allows devices to send and receive data, much like a postal address for the internet. Every device on the internet needs an IP address to be uniquely identified and reachable for communication. IP adaddresses are based on the Internet Protocol (IP), which is a set of rules governing how data is transmitted over the internet or local networks. They location information, allowing data to be routed to the correct destination. <br><br>
  Some examples of how public IPs can look like are : `192.168.1.1`, `203.0.113.43` or `17.172.224.47`, and the like. <br><br>

  IP addresses can be public (visible to the internet) or private (used within a local network). They can also be static (fixed) or dynamic (changing), with dynamic addresses often used for home internet connections. Also, there two versions of IP addresses: IPv4 (using 32-bit addresses) and IPv6 (using 128-bit addresses).

  - ### Difference between IPv4 and IPv6

  |      ***Feature***         |            ***IPv4 Address***         |                   ***IPv6 Address***                |
  | -------------------------- | ------------------------------------- | --------------------------------------------------- |
  |       Address Length       |             32-bit address            |                    128-bit address                  |
  |       Address Format       |  Decimal format (e.g., 192.168.0.1)   |       Hexadecimal format (e.g., 2001:0db8::1)       |
  |       Configuration        |      Manual and DHCP configuration    |      Auto-configuration and renumbering supported   |
  |    Connection Integrity    |  End-to-end integrity is unachievable |          End-to-end integrity is achievable         |
  |          Security          |         No built-in security;         | IPSec is built-in for encryption and authentication |
  |       Fragmentation        |    Performed by sender and routers    |             Performed only by the sender            |
  |     Transmission Scheme    |             Supports broadcast        |       Uses multicast and anycast; no broadcast      |
  |         Header Size        |           Variable: 20–60 bytes       |                     Fixed: 40 bytes                 |
  |         Conversion         |         Can be converted to IPv6      |    Not all IPv6 addresses can be converted to IPv4  |
  |           Example          |               192.168.1.1             |        2001:0000:3238:DFE1:0063:0000:0000:FEFB      |
  
> [!CAUTION]
> Do ***NOT*** share your private IP address with anyone on the internet or personally, unless you trust them completely.

- ## Media Access Control Address (MAC Address)
  A MAC address, or Media Access Control address, is a unique identifier assigned to network interfaces for communication within a network segment. It's a 12-digit hexadecimal number (48 bits) often found on a device's network interface card (NIC). Essentially, it's a hardware address that allows devices on a local network to communicate with each other. Every network interface, whether it's an Ethernet card, Wi-Fi adapter, or Bluetooth module, has a unique MAC address. It is a hardware address, meaning it's hardcoded into the device during the manufacturing of the machine. <br>

  MAC addresses are used at the data link layer of the OSI model to ensure data packets are delivered to the correct device on the local network. They are typically  written as six groups of two hexadecimal digits, separated by colons or hyphens (e.g., 00:1A:2B:3C:4D:5E). You can find your device's MAC address through your operating system's network settings or by using command-line tools like `getmac /v` or `ipconfig /all` on Windows machnies.

  <img width="1880" height="938" alt="Screenshot 2025-07-28 211916" src="https://github.com/user-attachments/assets/4ca3253e-6f4c-4e05-95af-61b74434a58e" />

- ## Transmission Control Protocol (TCP) / User Datagram Protocol (UDP)
  - ### TCP:
    TCP (Transmission Control Protocol) is one of the main protocols of the Internet protocol suite. It lies between the Application and Network Layers which are used in providing reliable delivery services. It is a connection-oriented protocol for communications that helps in the exchange of messages between different devices over a network. The Internet Protocol (IP), which establishes the technique for sending data packets between computers, works with TCP. It keeps track of the segments being transmitted or received by assigning numbers to every single one of them. Flow control limits the rate at which a sender transfers data. This is done to ensure reliable delivery. TCP implements an error control mechanism for reliable data transfer, and takes into account the level of congestion in the network.

  - ### UDP:
    User Datagram Protocol (UDP) is a Transport Layer protocol. UDP is a part of the Internet Protocol suite, referred to as the UDP/IP suite. Unlike TCP, it is an unreliable and connectionless protocol. So, there is no need to establish a connection before data transfer. The UDP helps to establish low-latency and loss-tolerating connections establish over the network. The UDP enables process-to-process communication. Used for simple request-response communication when the size of data is less and hence there is lesser concern about flow and error control. It is a suitable protocol for multicasting as UDP supports packet switching. UDP is used for some routing update protocols like RIP(Routing Information Protocol). Normally used for real-time applications which can not tolerate uneven delays between sections of a received message.
- ## Broadcast
  In networking, broadcast refers to the transmission of data from one source to all devices on a network. It's a one-to-all communication method where a single sender sends a message that is received by every device within a defined broadcast domain. This contrasts with unicast (one-to-one) and multicast (one-to-many) communication. A broadcast message is sent from a single source to every device on the network segment. The sender doesn't need to know or specify the individual addresses of the intended recipients; the message is intended for all. The scope of a broadcast is limited to a broadcast domain, which is a logical or physical network segment. <br><br>
  To achieve the process of broadcasting, a special broadcast address is used at the network layer (e.g., IP address) or data link layer (e.g., MAC address). For example, in Ethernet networks, a broadcast message is identified by a specific MAC address, and it's used in protocols like ARP (Address Resolution Protocol). Thr purpose of broadcasting is that it can be useful for tasks like sending network configuration updates or discovery requests, where all devices on the network need to be informed.

- ## Network Address Translator (NAT)
  Network Address Translation (NAT) is a method used by network devices, like routers, to translate IP addresses of devices within a private network to a single public IP address for internet communication. This allows multiple devices to share a single public IP, enhancing security by hiding the internal network structure. NAT modifies IP packet headers as they pass through the router or firewall. Private IP addresses are used within a local network (e.g., 192.168.x.x), while public IP addresses are globally unique and used for internet communication. NAT acts as a translator, converting private IP addresses to a public IP address when a device on the private network needs to access the internet.

  ![lolings](https://github.com/user-attachments/assets/8bc5a81c-7155-41da-9d58-fccddc2092d5)
- ## Port Forwarding
  Port forwarding is a networking technique that allows external devices to connect to specific devices or services within a private network. Itworks by redirecting communication requests from an external IP address and port to an internal IP address and port on the private network, such as a home or office network. This allows you to access devices like security cameras, gaming consoles, or remote desktops from outside the local network. Here are the steps on how port forwarding works: <br>
  1. Devices on a private network (like your home or office) have private IP addresses and use ports to communicate with each other and with the internet.
  2. Your router or firewall acts as a gateway between your private network and the public internet.
  3. You configure your router to forward specific types of traffic (identified by port numbers) to a particular device within your private network.
  4. When an external device sends a request to your public IP address and a designated port, the router intercepts the request.
  5. Instead of the router handling the request itself, it forwards the request to the specific device on your private network, based on the port forwarding rule.
  6. The device on your private network responds to the external request, and the router sends that response back to the external device.
 
- ## nmap
  Nmap (Network Mapper) is a powerful, free, and open-source utility designed for network discovery and security auditing. It's widely used by network administrators, security professionals, and even ethical hackers to gain insights into network infrastructure. Some features include host discovery, port scanning, operating system detection, firewall testing, et cetera. <br>

  Below is a list of important flags in an nmap command, that could be useful in the field of hacking:-
  
  ```bash
  nmap -Pn -A -sV -O -oN scan.txt --script vuln -vv -p 1-1000 -sS -T4 192.168.1.10
  ```
  
  | Flag            | Description                                        |
  | --------------- | -------------------------------------------------- |
  | `-Pn`           | Skip host discovery                                |
  | `-A`            | Aggressive scan (OS, versions, traceroute, script) |
  | `-sV`           | Service/version detection                          |
  | `-O`            | OS detection                                       |
  | `-oN scan.txt`  | Output to a file in normal format                  |
  | `--script vuln` | Use vulnerability detection scripts                |
  | `-vv`           | Very verbose output                                |
  | `-p 1-1000`     | Scan ports 1–1000                                  |
  | `-sS`           | Stealth SYN scan                                   |
  | `-T4`           | Faster scan timing                                 |
  | `192.168.1.10`  | Target IP address                                  |

- ## [haveibeenpwned](haveibeenpwned.com)
  This website helps check whether you e-mail address has been exposed in a data breach, and that your passwords or other sensitive information have been out on the internet.

  <img width="1843" height="1023" alt="Screenshot 2025-07-29 051921" src="https://github.com/user-attachments/assets/45603bac-82a1-450f-be00-867aeefb71ac" />

- ## [The Wayback Machine](https://web.archive.org/)
  This website helps you to 'go back in time' in the internet to visit different snapshots of websites, which can be useful to ethical hackers for various purposes.

  <img width="1856" height="1033" alt="Screenshot 2025-07-29 052919" src="https://github.com/user-attachments/assets/65ddd487-25f7-4ec9-b49d-738bff574b18" />

