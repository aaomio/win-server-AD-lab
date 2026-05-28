# Windows Server 2022 Installation (Active Directory Lab)

This document describes the installation of Windows Server 2022 inside a VMware virtual machine.

This step follows VM creation and ISO configuration.

---

## 1. Boot from Installation Media

The virtual machine must be powered on.

During startup, the boot menu will appear.

The following option must be selected:

- VMware Virtual SATA CDROM Drive (1.0)

To proceed:
- Any key must be pressed to boot from the installation media

---

## 2. Windows Setup

The Windows Setup screen will load.

The following action must be performed:

- Select **Install Now**

---

## 3. Operating System Selection

The following edition must be selected:

- Windows Server 2022 Standard Evaluation (Desktop Experience)

Then:
- Select **Next**

---

## 4. Installation Type

The installation type must be selected:

- Custom: Install Windows only (advanced)

This option ensures a clean installation.

---

## 5. Disk Selection

The virtual disk created during VMware setup must be selected:

- Drive 0 (Unallocated Space)

Then:
- Select **Next** to begin installation

---

## 6. Installation Process

Windows Server will now be installed automatically.

During this stage:
- Files will be copied
- Features will be installed
- The system will restart multiple times

No user interaction is required.

---

## 7. Administrator Setup

After installation completes, the initial setup screen will be displayed.

The following must be configured:

- Administrator username is set
- A secure password is created and applied

Then:
- Sign-in is completed using the Administrator account

---

## 8. First Boot

After login:

- Windows Server desktop will load
- Initial system setup is considered complete

---
