# VMware Workstation Setup (Create Virtual Machine)

This document explains how to create a new virtual machine in VMware Workstation for a Windows Server 2022 lab environment.

---

## 1. Create a New Virtual Machine

A new virtual machine must be created in VMware Workstation.

The following option must be selected:

- Create a new virtual machine
- I will install the operating system later (The VM will be created with a blank virtual disk)

This option ensures full manual control over the installation process.

---

## 2. Select Guest Operating System

The following selection must be made:

- Guest Operating System: Microsoft Windows
- Version: Windows Server 2022

This ensures correct default hardware compatibility settings are applied.

---

## 3. Choose Virtual Machine Name and Location

A name must be assigned to the virtual machine.

Example:
- DC01
- AD-Server
- DomainController

A dedicated folder must be selected to store the virtual machine files.

Recommended:
- Separate folder per lab environment
- Avoid default Documents location

---

## 4. Configure Virtual Disk

A virtual hard disk must be created for the operating system installation.

Recommended configuration:

- Disk size: 60–100 GB
- Store virtual disk as a single file (recommended for performance and simplicity)
- Provisioning: Thin provisioned (recommended for lab environments)

---

## 5. Finish Virtual Machine Creation

The setup must be completed by selecting:

- Finish

At this stage:
- The virtual machine is created
- No operating system is installed yet
- A blank virtual disk is attached

---

## 6. Attach Windows Server ISO

The virtual machine must be configured to boot from installation media.

Steps:

- Select the virtual machine
- Open **Edit virtual machine settings**
- Select **CD/DVD (SATA)**
- Enable **Use ISO image file**
- Browse and select the Windows Server 2022 ISO
- Ensure the following is enabled:
  - Connect at power on

This allows the VM to boot directly into Windows Setup.

---

## 7. Hardware Review (Recommended Check)

Before powering on, virtual hardware should be reviewed.

Recommended minimum configuration:

- CPU: 2–4 cores
- Memory: 4–8 GB RAM
- Network: NAT or Host-only (depending on lab design)
- Disk: 60–100 GB

Adjustments may be made based on host system performance.

---

## 8. Power On Virtual Machine

The virtual machine can now be powered on.

Expected result:
- Windows Server installation media should boot
- Windows Setup screen should appear

