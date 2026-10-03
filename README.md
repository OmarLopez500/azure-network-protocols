# Azure Network Traffic Analysis & ICMP Filtering

<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

## Project Overview

This project demonstrates how network traffic can be captured, identified, and controlled while working with virtual machines in Microsoft Azure.

For this lab, I used Wireshark to examine network traffic and focused on **ICMP communication** between systems. I also created a Linux firewall rule to block incoming ICMP traffic and observed how restricting a protocol can affect network communication.

The goal of the project is to demonstrate basic packet analysis and network security concepts using a hands-on virtual machine environment.

## Video Demonstration

* ### [YouTube: Azure Virtual Machines, Wireshark, and Network Security Groups](https://www.youtube.com)

## Technologies and Tools

The following technologies and tools were used during the lab:

* **Microsoft Azure** - Virtual machine hosting and networking
* **Remote Desktop** - Accessing the Windows virtual machine
* **Command-Line Tools** - Testing network connectivity and configuring the Linux system
* **Wireshark** - Capturing and analyzing network packets
* **Network Security Groups (NSGs)** - Azure network security and traffic control
* **ICMP** - Used for network connectivity testing
* **Linux Firewall** - Used to restrict incoming ICMP traffic

## Operating Systems

* **Windows 10 (21H2)**
* **Ubuntu Server 20.04**

---

# Lab Objectives

The main objectives of this lab were to:

1. Work with virtual machines hosted in Microsoft Azure.
2. Capture network traffic using Wireshark.
3. Identify and examine ICMP packets.
4. Configure a Linux rule to block incoming ICMP traffic.
5. Observe how restricting network traffic affects connectivity.

---

# High-Level Process

The lab was completed through the following steps:

### Step 1 - Prepare the Virtual Machines

The Windows and Ubuntu virtual machines were prepared in Microsoft Azure so that network communication could be tested between the systems.

### Step 2 - Capture Network Traffic

Wireshark was used to monitor network activity and capture packets moving between the virtual machines.

### Step 3 - Examine ICMP Traffic

ICMP traffic was identified within Wireshark to see how connectivity testing appears at the packet level.

### Step 4 - Block Incoming ICMP Traffic

A Linux firewall rule was created to prevent incoming ICMP traffic. The connection was then tested again to observe the effect of the rule.

---

# Actions and Observations

## 1. Capturing Network Traffic

<img width="1482" height="995" alt="Screenshot 2026-10-03 135219" src="https://github.com/user-attachments/assets/fce13ece-76fe-4e62-b3b0-7859ed082c3e" />

<p>

</p>

Wireshark was used to capture traffic generated during the lab. The packet capture provides a detailed view of network communication and allows individual packets to be examined.

This made it possible to see traffic between the virtual machines and identify the protocols being used.

---

## 2. Examining ICMP Traffic

<p>

<img width="1486" height="746" alt="Screenshot 2026-10-03 140257" src="https://github.com/user-attachments/assets/686b8080-e7dc-4a4e-a0f0-21e4708e62bc" />

</p>

The captured traffic was examined in Wireshark to identify **ICMP packets**. ICMP is commonly used for network connectivity testing, such as when using the `ping` command.

By examining the packets, I was able to see the source and destination systems and observe the ICMP communication taking place between them.

---

## 3. Blocking Incoming ICMP Traffic on Linux

<p>

<img width="1906" height="845" alt="Screenshot 2026-10-03 141619" src="https://github.com/user-attachments/assets/9ad52bc7-d083-4396-b618-c9d1efb83f8c" />

</p>

A firewall rule was created on the Linux virtual machine to block incoming ICMP traffic.

The purpose of this rule was to restrict a specific network protocol and observe how the change affected communication. After applying the rule, ICMP connectivity could be tested again to compare the results before and after the traffic was blocked.

---

# Key Takeaways

This lab provided hands-on experience with network traffic analysis and basic traffic filtering.

The main concepts demonstrated were:

* Wireshark can be used to capture and inspect network packets.
* Different protocols can be identified within a packet capture.
* ICMP is useful for testing network connectivity.
* Linux firewall rules can be used to control incoming traffic.
* Blocking a protocol can change how systems communicate with each other.
* Packet analysis can help explain why a network connection succeeds or fails.

---

# Conclusion

This project demonstrated how network communication can be monitored and controlled using a combination of Azure virtual machines, Wireshark, and Linux firewall rules.

By first observing ICMP traffic and then creating a rule to block incoming ICMP packets, I was able to see how a network security change can directly affect connectivity.

The lab provided practical experience with packet analysis, network protocols, and basic traffic filtering.
