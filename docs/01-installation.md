# Ubuntu Server Installation

This document explains how to prepare the dedicated monitoring virtual machine for Uptime Kuma deployment.

---

# System Requirements

| Resource | Minimum |
|---|---|
| CPU | 1 vCPU |
| RAM | 1 GB |
| Storage | 10 GB |
| Network | Bridged Adapter |

---

# Recommended Hypervisors

- Proxmox
- VirtualBox
- VMware Workstation

---

# Ubuntu Server Setup

## Download Ubuntu Server

Official website:

- Ubuntu Server 24.04 LTS

---

# VM Configuration

## Recommended Settings

| Setting | Value |
|---|---|
| OS Type | Ubuntu Linux |
| CPU | 1 Core |
| RAM | 1024 MB |
| Disk | 10 GB |
| Network | Bridged |

---

# Install Ubuntu Server

During installation:

## Recommended Packages
- OpenSSH Server

---

# Update System

```bash
sudo apt update && sudo apt upgrade -y
```
