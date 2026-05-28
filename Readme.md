# Windows Server Active Directory Lab (VMware + DNS + AD DS)

This repository provides a structured step-by-step lab for building a Windows Server 2022 Active Directory environment using VMware Workstation.

The lab includes virtual machine setup, Windows installation, Active Directory configuration, DNS setup, and organizational unit management.

---

## Lab Workflow

Follow the steps in order.

---

## 1. Server Preparation

Preparation of required tools and installation media.

- [Server Preparation](./server-prep.md)

Includes:
- VMware Workstation download
- Windows Server 2022 ISO download
- Lab prerequisites

---

## 2. VMware Virtual Machine Setup

Creation and configuration of the virtual machine.

- [VMware Setup](./vmware-setup.md)

Includes:
- Virtual machine creation
- Guest OS selection (Windows Server 2022)
- Virtual disk configuration
- ISO attachment

---

## 3. Windows Server Installation

Installation of Windows Server inside the virtual machine.

- [Windows Server Installation](./win-server-install.md)

Includes:
- Boot from ISO
- Installation process
- Administrator account setup

---

## 4. Active Directory Installation

Installation and promotion of the server to a Domain Controller.

- [Active Directory Setup](./AD-install.md)

Includes:
- AD DS role installation
- Forest creation
- Domain controller promotion
- DSRM configuration

---

## 5. DNS Configuration

Configuration and verification of DNS for Active Directory.

- [DNS Configuration](./dns-config.md)

Includes:
- DNS verification
- nslookup testing
- DNS service validation
- Resolution troubleshooting

---

## 6. Active Directory Organizational Units

Creation of users, groups, and organizational structure.

- [Active Directory OUs](./AD-OU.md)

Includes:
- OU structure design
- User creation
- Security groups
- Group assignment

---

## Repository Structure

```text id="tree2"
server-prep.md
vmware-setup.md
win-server-install.md
AD-install.md
dns-config.md
AD-OU.md
```
