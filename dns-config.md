# DNS Configuration (Active Directory Lab)

This document describes the DNS configuration required for a functioning Active Directory environment.

DNS must be correctly configured for domain resolution and authentication to work properly.

---

## 1. DNS Role Confirmation

After Active Directory installation, the DNS role is automatically installed on the Domain Controller.

Verification can be completed using:

- Server Manager\Tools\DNS

---

## 2. Verify DNS Server Binding

The DNS server must be bound to the Domain Controller network interface.

Ensure:
- DNS service is running
- The correct server IP is listed

---

## 3. Configure DNS on Domain Controller

The Domain Controller must use itself for DNS resolution. IPv4 settings must be configured by going to ncpa.cpl from Run:

- Preferred DNS: Domain Controller IP address

To identify the correct IP address:
- Open Command Prompt
- Run:
```cmd
ipconfig /all
```

- Locate the adapter VMNET and Note the values listed for:
```
Default Gateway
Primary WINS Server
```
These should match the IP address assigned to the Domain Controller.

Do NOT use:
- 127.0.0.1
- ::1
- External DNS (e.g. 8.8.8.8)

---

## 4. Verify Forward Lookup Zone

The forward lookup zone must exist for the domain in DNS app.

Check:
- Domain name zone (e.g. matrix.local)
- A records for Domain Controller

---

## 5. Test DNS Resolution

DNS resolution must be tested using:

```cmd
nslookup lab.local
```
Expected result:
- Domain Controller IP is returned
- Correct DNS server is shown as the Domain Controller
