28/6
 **بسم الله الرحمن الرحيم** 

## 1- CCNA 200-301 Content
1- [Network Fundamentals --> OSI - MAC - IP - Network Components 20%]
2- [IP Services --> DHCP - NAT - DNS 10%]
3- [Security Fundamentals --> Cyber Security ( Network Security ) 15%]
[4- Network Access --> ==Switching== (VLANS) (STP)  20%]
5-[ IP Connectivity --> ==Routing== (OSPF) (FHRP) 25%]
6-[ Automation --> REST APIs  - (SDN)   15%]

-----
## 2- Notes
### ==What's Network ?== 
A network is a **connected collection of devices** that communicate with each other through **Switches** and/or **Servers**.
so what's difference ?

#### **Through Switch:**

- **Decentralized Administration**
    
    - Each device (e.g., PC) has **its own control** over its data and settings.
        
    - There is no single point of control or management for the devices.
        "CCNA" - "CCNP"

---
#### **Through Server:**

- **Centralized Administration**
    
    - A server provides services and controls the resources accessed by the connected devices (Clients).
        
    - The server manages:
        
        - User permissions.
            
        - File sharing.
            
        - Applications and updates.
            
        - Security and monitoring.
        -  "MCSA"
------
#### **Importance Of Network**

1- Sharing Of Resources
2- Modern Technology 
VOIP -- Video Conference- IOT - BYOD 
VOIP = Voice Over IP
BYOD = Bring Your Own Device
IOT = Internet Of Things
3- Cloud
#### **Components Of Network***
##### **1. Hardware**

**a. End Devices:**

- Devices used to access the network or its services.  
    Examples: PCs, Laptops, Servers, Printers, IP Phones.
    

**b. Network Devices = Central Points:**

- Devices that connect and manage communication within the network.  
    Examples: Routers, Switches, Access Points, Firewalls.
    

**c. Transmission Media:**

- The medium through which data is transferred.  
    Examples: Ethernet cables (wired), Wi-Fi, Bluetooth (wireless).
    

---

##### **2. Software**

**a. Network Operating System (NOS):**

- Manages network devices and operations.  
    Examples: Cisco IOS, Windows Server, Linux-based NOS.
    

**b. Protocols:**

- Set Of Rules 
    Examples: FTP - HTTP - HTTPS 

---

#### **ECNM**
Enterprise Composite Network Model
framework developed by **Cisco** for designing and organizing large, complex enterprise networks. Its purpose is to divide the network into layers or "modules" to simplify management, improve performance, and enhance security.
##### 1- Access Layer 
- The layer where users and devices connect to the network Through Switches
    
- Responsible for:
    
    - Connecting end devices (PCs, printers, etc.).
        
    - Providing functions like **VLANs**.
#####  2. Distribution Layer :
- Connects the **Access Layer** to the **Core Layer**.
- should @ Least Have 2 Distribution Layers for Back-Up 
    
- Responsible for:
    
    - Applying **security policies**.
        
    - Aggregating connections.
        
    - Data routing and forwarding.
    - CCNP Switching 
##### 3- Core Layer:
- The backbone of the network.
    
- Focuses on high-speed and efficient data routing across the network.
    
- Avoids additional tasks (like filtering) to ensure optimal performance.
- CCNP Routing
- CCNP Security 
- CCNP ISP
##### 4- Server Farmer Block
The Field Of Servers 

-------------------------------------
#### Firewall
**Filter Packets**  --> Allow - Deny
After We Connect The ECNM and This Called 
##### ( LAN ) -> Single Connection
A **Local Area Network (LAN)** is a network that connects devices within a small geographical area, like a home, office, or campus. ==Intranet== ==Inside== ==trusted==
Example : End Points

and We want Connect To The Internet
##### (WAN) -> Multi Connection
A **Wide Area Network (WAN)** connects multiple local networks (LANs) across large geographical areas like cities, countries, or even continents. ==Internet== ==Outside== ==Untrusted==
Example : Internet

##### (MAN) 
A **Metropolitan Area Network (MAN)** connects multiple local area networks (LANs) within a city or metropolitan area, offering higher speeds and broader coverage than LANs but smaller than Wide Area Networks (WANs).
##### DMZ -> Demilitarized Zone
A **DMZ** in networking is a **buffer zone** between an internal network (LAN) and external networks (like the Internet). It contains publicly accessible services while protecting the internal network from direct exposure to external threats.


![[Pasted image 20250628195321.png]]

![[Pasted image 20250628194948.png]]

-------
#### Fault Tolerance

**Fault Tolerance** refers to a system's ability to continue operating properly even when one or more of its components fail. It ensures high availability, reliability, and resilience in networks, hardware, or software systems.

NO : Single Point Of Failure

---

##### **How Fault Tolerance Works:**

1. **Redundancy:**
    
    - Duplicating critical components (e.g., Routing - Switching) to prevent total failure.
        
2. **Failover Mechanisms:**
    
    - Automatically switching to a backup system when the primary system fails.
        
3. **Load Balancing:**
    
    - Distributing workloads across multiple systems to avoid overloading a single point.
        
4. **Data Replication:**
    
    - Keeping identical copies of data in multiple locations to recover from a failure.
        

---

##### **Examples in Networking:**

1. **Redundant Links:**
    
    - Multiple network paths using protocols like **Spanning Tree Protocol (STP)**.
        
2. **High Availability (HA):**
    
    - Using multiple servers in a cluster to ensure continuous service.
        
3. **RAID (Redundant Array of Independent Disks):**
    
    - Protecting data storage with mirroring or parity techniques.
        

---

##### **Advantages of Fault Tolerance:**

- Minimizes downtime.
    
- Protects against data loss.
    
- Improves system reliability.
    

---

##### **Example Scenario:**

- **Without Fault Tolerance:**  
    A server crash disrupts business operations entirely.
    
- **With Fault Tolerance:**  
    A backup server takes over seamlessly, ensuring operations continue without interruption.

![[Pasted image 20250628204238.png]]

----------
#### Characteristics of a Perfect Network
Security - Scalability - Fault Tolerance - Speed - Performance
QoS --> Quality Of Service (VOIP)

![[Pasted image 20250628204103.png]]

----
#### Network Security
Any Network To Be Secure Should Have 3 Things
==C== Confidentiality *MITM*
==I== Integrity 
==A== Availability 

-----
### Physical And Logical Topology
### **1. Physical Topology:**

- **Definition:**  
    This refers to the actual physical arrangement of devices and cables in the network. In other words, it represents how devices are physically connected.
    
- **Examples:**
    
    - **Bus Topology:** All devices are connected to a single main cable.
        
    - **Star Topology:** All devices are connected to a central device like a switch or router.
        
    - **Mesh Topology:** Each device is connected to every other device.
        
- **Focus:**
    
    - Location of devices.
        
    - Types of cables used.
        
    - Physical devices like routers, switches, etc.
        
- **Importance:**  
    Determines the physical layout and how signals travel through the network.
    

---

### **2. Logical Topology:**

- **Definition:**  
    This refers to how data flows between devices in the network, regardless of the physical connections. In other words, it represents the network from a data transmission perspective.
    
- **Examples:**
    
    - **Logical Bus:** Even if devices are physically connected in a star topology, data can flow as if in a bus topology.
        
    - **Logical Ring:** Data flows in a circular manner logically, regardless of physical connections.
        
- **Focus:**
    
    - Network protocols (e.g., Ethernet, Token Ring).
        
    - How data moves and is managed.
        
- **Importance:**  
    Defines the rules for data transfer and how collisions are handled.
    

---

### **Key Differences:**


|     | Physical                              | Logical                    |
| --- | ------------------------------------- | -------------------------- |
|     | Physical arrangement of devices\|<br> | Data flow between devices. |


---

### **Important Note:**

Physical topology and logical topology can differ.  
For example:  
A network physically connected in a **Star** topology might operate logically as a **Bus** topology.
