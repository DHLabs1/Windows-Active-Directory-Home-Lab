# Active Directory Home Lab (Cybersecurity Focus)

## Overview
This project demonstrates the setup and configuration of a Windows Active Directory environment
using VirtualBox. The lab simulates an enterprise domain environment commonly encountered in
help desk and SOC roles.

## Technologies Used
- VirtualBox
- Windows Server 2025
- Windows 11 Enterprise
- Active Directory Domain Services (AD DS)
- DNS & DHCP
- PowerShell
- Group Policy

## Lab Architecture
- Domain Controller with dual NICs (NAT + Internal Network)
- Windows 11 client joined to the domain
- Isolated internal network for AD communication

## Key Skills Demonstrated
- Active Directory installation and domain promotion
- DNS and DHCP configuration
- Organizational Units (OUs) and Group Policy
- User and group management
- PowerShell automation for bulk user creation
- Windows domain joining and troubleshooting


Step1. Create the Virtual Machine for the Domain Controller with the hardware and storage requirements. Then provision the Network settings with two Adapaters.

Adapter 1 - Attached to NAT
Adapter 2 - Attached to Internal Network

This networking design supports external network access through host-based NAT while enabling isolated communication between virtual machines on the internal network.

![DC Adapter Settings1](https://github.com/user-attachments/assets/179948f7-543f-4186-a08e-7c9f143b574e)

![DC Adapter Settings2](https://github.com/user-attachments/assets/cf5f04ec-dce9-4a2a-ac26-9540b3886824)

