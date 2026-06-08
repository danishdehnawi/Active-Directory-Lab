# Active-Directory-Lab
Built an enterprise-style Active Directory lab using Windows Server 2019 and VirtualBox. Configured a Domain Controller, DNS, DHCP, and RRAS/NAT, automated the provisioning of 1,000 users with PowerShell, and integrated Windows 10 clients into the domain.


# Active Directory Home Lab

## Overview

Built a Windows Server 2019 Active Directory home lab in VirtualBox. The lab includes Active Directory Domain Services (AD DS), DNS, DHCP, Routing and Remote Access (NAT), a Windows 10 client joined to the domain, and PowerShell automation to create over 1,000 users.

---

## Network Topology

The lab consists of a Windows Server 2019 Domain Controller and a Windows 10 client connected through an internal network.

![Network Diagram](Screenshots/network-diagram.png)

---

## Server Configuration

Configured Windows Server 2019 with the required roles and services.

- Active Directory Domain Services (AD DS)
- DNS
- DHCP
- Routing and Remote Access (RRAS/NAT)

![Server Overview](Screenshots/server-overview.png)

---

## Domain Controller

Promoted the server to a Domain Controller for the domain:

**mydomain.com**

![Domain Controller](Screenshots/domain-controller.png)

---

## PowerShell User Automation

Used a PowerShell script to automatically create over 1,000 Active Directory users from a names.txt file.

Files used:

- Create-Users.ps1
- names.txt

![PowerShell User Creation](Screenshots/powershell-user-creation.png)

---

## Active Directory Users

Verified successful creation of user accounts inside the _USERS Organizational Unit.

![Active Directory Users](Screenshots/active-directory-users.png)

---

## DHCP Configuration

Configured DHCP scope and verified clients received IP addresses automatically.

![DHCP Leases](Screenshots/dhcp-leases.png)

---

## Domain-Joined Client

Joined a Windows 10 client workstation to the Active Directory domain.

![Client Object](Screenshots/client-domain-object.png)

---

## Successful Domain Login

Verified successful login using the domain account.

![Client Domain Login](Screenshots/client-domain-joined.png)

---

## Skills Demonstrated

- Active Directory Administration
- Windows Server 2019
- DNS Configuration
- DHCP Configuration
- Routing and Remote Access (RRAS)
- Network Address Translation (NAT)
- PowerShell Scripting
- User Provisioning Automation
- Windows 10 Domain Join
- Troubleshooting
- VirtualBox Virtualization
