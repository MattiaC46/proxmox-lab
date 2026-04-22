![Proxmox](https://img.shields.io/badge/Proxmox-VE-orange)
![Docker](https://img.shields.io/badge/Docker-Container-blue)
![Active Directory](https://img.shields.io/badge/AD-Domain_Controller-purple)
![Firewall](https://img.shields.io/badge/Firewall-NethSecurity-red)
![VPN](https://img.shields.io/badge/VPN-Remote_Access-blue)
![DNS](https://img.shields.io/badge/DNS-Configured-informational)
![Monitoring](https://img.shields.io/badge/Monitoring-Grafana%20%2B%20Prometheus-orange)
![NAS](https://img.shields.io/badge/Storage-NAS-blueviolet)
![NFS](https://img.shields.io/badge/Storage-NFS-blue)
![HA](https://img.shields.io/badge/HA-Enabled-success)
![Veeam](https://img.shields.io/badge/Backup-Veeam-green)
# PROXMOX VE Infrastructure Projects

This repository provides an overview of my projects focused on system administration, networking, virtualization, and backup strategies.

The lab is built using real-world technologies to simulate enterprise environments and practice production-like scenarios.

---

## Projects Overview

### 🖥️ 1. Enterprise Network Lab with Firewall and Active Directory

A virtual enterprise network designed to simulate a real corporate environment with network segmentation, firewalling, and centralized identity management.

#### Key Features:
- Firewall-based network segmentation (WAN / LAN)
- Internal network (10.10.10.x) separated from external network (192.168.x.x)
- Windows Server configured as Domain Controller
- Windows 10 client joined to Active Directory domain
- DHCP managed by firewall
- DNS resolution using Pi-hole and Active Directory
- Remote access via VPN (RDP to internal machines)

#### Technologies:
- Proxmox VE (virtualization platform)
- NethSecurity (firewall)
- Windows Server (Active Directory, DNS)
- Pi-hole (DNS filtering and local records)
- Docker (monitoring and services)

---

### 🖥️ 2. Proxmox Cluster Lab with High Availability and Backup

A multi-node virtualization cluster built to simulate enterprise-grade infrastructure with shared storage, high availability, and disaster recovery.

#### Key Features:
- 3-node Proxmox cluster with quorum
- Shared storage using NFS (NAS)
- Migration of VMs from local storage to shared storage
- High Availability (HA) with automatic failover
- Backup infrastructure using Veeam
- Cross-node VM recovery testing

#### Backup & Recovery:
- Veeam Backup & Replication deployed on Windows Server
- Backup repository hosted on NAS (NFS)
- Full VM backup and restore
- Cross-node restore (disaster recovery scenario)

#### High Availability:
- VM failover between nodes in case of node failure
- HA configuration with automatic restart policies

---

## Goals of the Lab & Real-World Context

These projects were developed during an internship in a company environment with the goal of evaluating a potential migration from Hyper-V to Proxmox VE.

The lab infrastructure was used to simulate real-world scenarios including:

- Multi-node virtualization cluster
- High Availability (HA) and failover behavior
- Shared storage using NFS
- Backup and disaster recovery using Veeam
- Network segmentation and Active Directory integration

This project therefore represents not only a learning experience, but also a practical proof-of-concept for a production environment.

---


---

## 📄 Author

Personal lab projects focused on learning and practicing system administration and infrastructure design.
