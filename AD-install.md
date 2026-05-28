# Active Directory Domain Services Installation (Domain Controller Setup)

This document describes the installation of Active Directory Domain Services (AD DS) and the promotion of the server to a domain controller.

This step follows initial server setup and preparation.

---

## 1. Display Configuration (Optional)

The display resolution may be adjusted for usability.

Recommended:
- 1440 × 900

---

## 2. Open Server Manager

The AD DS installation process is initiated through Server Manager.

Steps:

- Open **Server Manager** 
- Select **Manage**
- Click **Add Roles and Features**

---

## 3. Install Active Directory Domain Services

The following role must be selected:

- Active Directory Domain Services (AD DS)

When prompted:
- Required features must be added
- Installation must be completed

The window must remain open after installation.

---

## 4. Promote Server to Domain Controller

After installation:

- Select **Promote this server to a domain controller**

---

## 5. Create New Forest

In the Active Directory Domain Services Configuration Wizard:

The following option must be selected:

- Add a new forest

A domain name must be specified.

Example:
- lab.local
- company.local

---

## 6. Functional Level Configuration

The following functional levels must be selected:

- Forest functional level: Windows Server 2016
- Domain functional level: Windows Server 2016

---

## 7. Domain Controller Options

The following options must be configured:

- DNS Server: Enabled (default)
- Global Catalog: Enabled (default)

A Directory Services Restore Mode (DSRM) password must be set.

---

## 8. NetBIOS Name

The NetBIOS name will be automatically generated.

This may be reviewed before continuing.

---

## 9. Installation and Restart

The configuration will be validated and installed.

During this process:
- The server will be promoted to a domain controller
- The system will restart automatically
- The Administrator session will be logged off

---

## 10. First Login After Promotion

After restart:

- The domain login screen will appear
- Login must be performed using the domain Administrator account

