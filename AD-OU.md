# Active Directory Organizational Units and Groups (Matrix Lab Theme)

This document describes the creation of Organizational Units (OUs) and security groups within Active Directory.

A structured OU design is used to organise users, computers, and administrative groups.

---

## 1. Open Active Directory Users and Computers

The Active Directory management console must be opened:

- Server Manager\Tools\Active Directory Users and Computers

---

## 2. Create Root Organizational Unit Structure

A top-level OU structure must be created to organise the domain.

Recommended structure:

- OU: MATRIX
  - OU: HUMANS
  - OU: SYSTEMS
  - OU: AGENTS

---

## 3. Create Matrix-Themed Users (Example)

Inside the **HUMANS** OU, user accounts may be created.

Example users:
- Neo
- Trinity
- Morpheus

Each user must be created using:
- New\User
- Username and password must be assigned

---

## 4. Create Security Groups

Security groups must be created to control access.

Inside the **SYSTEMS** OU, the following group is created:

- Group Name: CENTINELS

Group settings:
- Group Scope: Global
- Group Type: Security

---

## 5. Add Users to Groups

Users must be assigned to groups for access control.

Example:

- CENTINELS\Neo
- CENTINELS\Trinity
- CENTINELS\Morpheous

---

## 6. Verify OU Structure

The final structure must appear as:

- MATRIX
  - HUMANS (Neo, Trinity, Morpheus)
  - SYSTEMS (CENTINELS)
  - AGENTS (reserved for future use)

---

## 7. Completion

The Active Directory environment now contains:

- Structured Organizational Units
- Themed user accounts
- Security group assignments

This confirms successful AD object organisation.