# 🏠 Home Network Diagram – May 2025

![NetworkDiagram](./img/NetworkDiagram.png)

This diagram outlines my current home network and workstation setup. My goal is to simulate a small office/home office (SOHO) environment and create a home lab environment for testing, monitoring, and managing various system administration tasks.

## 🛜 Network Overview

My home network consists of both wired and wireless components. The network is managed through an ASUS Wi-Fi router with firewall enabled. The Asus router receives its uplink from a TP-Link Ethernet Gigabit Media Converter (ISP-provided), which is connected to a fiber network.

### 🔗 Wired Infrastructure
- **PC 1 – Windows 11 Pro**  
  Primary admin workstation for daily operations, system configuration, and running Linux VMs (e.g., Ubuntu Server, CentOS 9) for testing.
- **PC 2 – Windows 10 Home (Dual Boot Linux)**  
  Used for Linux practice, OS deployment testing, and backup system management.
- **Synology DS224+ NAS**  
  Configured for file backup, data redundancy, and centralized storage management using SMB/AFP protocols.

### 🖥️ Peripheral and Display Management
- **2-Port KVM Switch**  
  Manages keyboard, mouse, and dual-display setup between both PCs.
  Using the KVM switch allows me to switch between PCs while I practice and test my home lab environment. 
- **USB Hub, External HDD (Seagate)**  
  For expanded I/O to support backup operations and connectivity with additional IoT or USB-powered devices.

### 📡 Wireless Devices 
- **MacBook Air, iPhone**  
  Primarily used as personal devices, but available for occasional testing of connectivity, VPN access, and remote file syncing across non-Windows platforms.
- **Smart TV, Speaker, PS4**  
  Consumer devices connected to the network for daily use. While they are not part of the lab environment, they can be referenced for basic network visibility, segmentation, or bandwidth management if needed.

## 🧵 Cable & Media Legend
The diagram uses visual indicators for clarity:
- 🟢 **Fiber Cable** – ISP uplink
- 🟤 **Cat 6 Ethernet** – Wired LAN
- ⚫ **HDMI / DisplayPort** – Video signal
- 🔵 **USB A / Micro B** – Peripheral connection
- ▫️ **Wi-Fi** – Wireless network

## 🔐 Network Services & Security
- **Firewall Enabled** – ASUS router configured for SPI/NAT protection
- **DHCP Server** – Internal IP distribution
- **Static IP Mapping** – Reserved IP for NAS and lab VMs
- **VM Testing** – Linux VMs launched via VirtualBox for patch testing, automation scripts, and basic network segmentation trials

---

### ✅ Key System Administrator Skills Demonstrated
- Small network topology design and documentation
- Router and firewall configuration
- OS deployment and dual boot setup
- Shared resource access and storage centralization (NAS)
- KVM switch and peripheral management
- Cross-platform device integration (Windows, macOS, Linux)
- Basic virtualization and lab automation workflows

---

This hands-on environment not only supports personal projects, but also simulates real-world sysadmin scenarios in a structured and maintainable way.
