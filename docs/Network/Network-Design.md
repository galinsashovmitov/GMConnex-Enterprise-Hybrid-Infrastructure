# Network Design

## Project Information

Project: GMConnex Enterprise Hybrid Infrastructure

Target Environment:
Enterprise (100–150 users)

---

# Public Domain

gmconnex.com

---

# Internal Active Directory Domain

ent.gmconnex.com

---

# IP Addressing


## Network

10.10.10.0/24

## Default Gateway

10.10.10.1

## DNS Servers

DC01 - 10.10.10.12

DC02 - 10.10.10.13

## DHCP Scope

10.10.10.100 - 10.10.10.200

## Static IP Allocation

| Device | IP Address |
|---------|------------|
| ESX01 | 10.10.10.10 |
| VC01 | 10.10.10.11 |
| DC01 | 10.10.10.12 |
| DC02 | 10.10.10.13 |
| FS01 | 10.10.10.14 |
| MGMT01 | 10.10.10.15 |

---

# Physical Infrastructure

Internet
    │
ISP Router
    │
Managed Switch
   ├── ESX01
   └── ENG01

---

# Planned Server Roles

- Domain Controller 01 - DC01
- Domain Controller 02 - DC02
- File Server - FS01
- Management Server - MGMT01
- vCenter Server (later) - VC01
- Windows Admin Center (later) - WAC01
---

# Azure Services

- Microsoft Entra ID
- Azure Arc
- Azure Backup (later)
- Microsoft Entra Connect (later)
---

# Notes

Version: 1.0

Initial implementation uses a single subnet (10.10.10.0/24).

The network will be expanded in future phases by introducing VLANs and additional subnets through documented change requests.