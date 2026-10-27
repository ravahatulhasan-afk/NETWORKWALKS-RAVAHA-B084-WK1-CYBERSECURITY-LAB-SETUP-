# NETWORKWALKS-RAVAHA-B084-WK1-CYBERSECURITY-LAB-SETUP-

1ST TASK : LAB ENVIRONMENT SETUP. 

**Creating a cybersecurity environment for pen testing and ethical hacking.**

## OVERVIEW:

This project involves creating a virtual cybersecurity lab using VirtualBox and Kali Linux. The lab will be used to practice cybersecurity tasks such as scanning networks, finding devices, checking for security weaknesses, and testing security tools.

The lab will run on a private virtual network to keep testing separate from normal networks. More virtual machines can be added later to act as target systems for practicing penetration testing safely and legally.

---

## OBJECTIVES:

-Install VirtualBox and set up Kali Linux as a virtual machine on oracle VirtualBox.
-Create a private NAT Network and configure Kali’s network settings with a fixed IP address.
-Test the internet connection and DNS to make sure the network is working.
-Save a VM snapshot so the system can be restored if something goes wrong.
-Document the setup and prepare the lab for future cybersecurity testing and tasks.

---

## PURPOSE:

-Network reconnaissance
-Port scanning
-Vulnerability assessment
-Packet analysis
-Web security testing
-Exploitation practice
-Security-tool experimentation

---

## ARCHITECTURE:

<img width="2558" height="1383" alt="image" src="https://github.com/user-attachments/assets/ac61e0e0-e3c3-43e5-93bf-f5f70495820a" />

---

## LAB CONFIGS:

|    Component       |   Configuration    |
| ------------------ | ------------------ |
|    Host OS         | Windows 11         |
|    Host RAM        | 16 GB              |
|    Processor       | Intel Core i5 12g  |
|    Hypervisor      | VirtualBox 7.2.20  |
|    Security OS     | Kali Linux 2026.2  |
|    Kali RAM        | 2048 MB            |
|    Virtual Network | NATNetwork         |
|    Network Address | 10.0.0.0/24        |
|    Kali IP Address | 10.0.0.2/24        |
|    Default Gateway | 10.0.0.1           |
|    DNS Server      | 8.8.8.8            |
|    Future VM Range | 10.0.0.3–10.0.0.99 |

---

## SETUP PROCEDURE: 

## Step 1: Install a file extractor.

For the first step of the procedure i used the winrar file extractor by which the kali linux files were extracted before installation.

Tool used: WINRAR

---

## Step 2: Install Oracle VirtualBox

VirtualBox 7.2.20 was installed to simulate a virtual working environment for the Linux Operating system.

Tool used: Virtualbox 7.2.20

---

## Step 3: NAT Network Creation


Configuration:
Network Name: NatNetwork
IPv4 Prefix:  10.0.0.0/24
DHCP:         Enabled
IPv6:         Disabled

<img width="2558" height="1385" alt="image" src="https://github.com/user-attachments/assets/146c4a1f-5367-482c-86f9-b51d1130c993" />


A NAT Network was chosen so that multiple virtual machines connected to the same NAT Network can communicate with each other.
This will allow future attacker and target VMs to communicate within the lab.

---

## Step 4: Importing Kali Linux

The Kali Linux files were downloaded from the linux website then extracted using winrar, after that the files were then imported to the virtualbox. 

```text
Adapter 1:
Attached to:  NAT Network
Network:      NatNetwork
Adapter Type: Intel PRO/1000 MT Desktop
RAM: 2048
```

<img width="1441" height="1185" alt="image" src="https://github.com/user-attachments/assets/7e2b4104-5063-40e9-99d7-da8a59aadb3a" />

---

## Step 5: Kali Network Configuration

The Kali Linux network was configured using a IPv4 address.

```text
IP Address: 10.0.0.2
Subnet Mask: 255.255.255.0
Gateway: 10.0.0.1
DNS: 8.8.8.8
```

<img width="826" height="628" alt="image" src="https://github.com/user-attachments/assets/3a1da3fd-b37c-462a-8637-ae248d105a4f" />


## Step 6: VM Snapshot Creation

After completing the initial configuration, a VirtualBox snapshot was created so if anything happens to the machine it can load to a saved state made by the snapshot.

Snapshot name:
```text
KALI
```

<img width="904" height="563" alt="image" src="https://github.com/user-attachments/assets/a1ab9c9f-f777-45fa-b2aa-e7df9d021820" />


---

## Learning Outcomes:

Through this task assigned to me, I learned how to create and configure a virtual environment for cybersecurity practice using kali linux and oracle virtualbox along with IP settings.

### 1. Oracle and Linux installation

I learned how to install oracle virtual box and kali linux files in order to simulate the linux operating system virtually for my cybersecurity journey.

### 2. NAT Network

i learned about NAT network as it was chosen so that multiple virtual machines connected to the same NAT Network can communicate with each other.
This will allow future attacker and target VMs to communicate within the lab.

### 3. Virtual Machine Networking

I learned how VirtualBox network adapters connect virtual machines to networks and how network settings control communication between them.

### 4. Static IP Configuration

I learned how to setup, configure and verify IPv4 addressing, subnet masks, gateways, and DNS settings in the network section for Kali Linux.

### 5. VM Snapshots

I learned how a snapshot should be taken just in-case a crisis arises, as having a backup state helps if something happens to the machine.
This provides a known-good recovery point for future cybersecurity exercises.

### 6. Documentation

I learned that documenting commands, configuration, screenshots, problems, and solutions is an important part of a professional cybersecurity project.

---

## Tools Used:
1- winrar
2- Oracle VirtualBox
3- Kali Linux files

---

Ravaha-Tul-Hasan | Cybersecurity week 1 | VirtualBox Setup

