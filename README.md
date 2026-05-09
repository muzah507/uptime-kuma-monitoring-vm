# 🚀 Uptime Kuma Monitoring VM

A production-style homelab monitoring server built with Uptime Kuma, Docker, and Ubuntu Server.

This project simulates a dedicated monitoring infrastructure commonly used in small businesses, NOC environments, and self-hosted homelabs. The monitoring stack is deployed inside a standalone virtual machine to provide isolated and centralized service monitoring.

---

## 📌 Project Overview

This repository demonstrates how to deploy a lightweight but reliable monitoring solution capable of tracking:

- Server availability
- Router connectivity
- HTTP services
- SSH/TCP services
- Network uptime
- Telegram alert notifications

Unlike basic all-in-one homelab setups, this project uses a dedicated monitoring VM architecture similar to real-world infrastructure deployments.

---

# 🖥️ Infrastructure Stack

| Component | Technology |
|---|---|
| Hypervisor | Proxmox / VirtualBox / VMware |
| Operating System | Ubuntu Server 24.04 LTS |
| Monitoring Platform | Uptime Kuma |
| Container Runtime | Docker |
| Notification System | Telegram |
| Monitoring Scope | Router, Server, SSH, HTTP Services |

---

# 🌐 Network Topology

```text
                     INTERNET
                         │
                    ISP Router
                         │
                    MikroTik Router
                         │
         ┌───────────────┴───────────────┐
         │                               │
   Monitoring VM                   Other Devices
   Ubuntu Server                   NAS / Servers
   Docker + Kuma                   Web Applications
```

---

# 🖥️ VM Specification
| Resource | Value |
|---|---|
| vCPU | 1 |
| RAM |	1 GB |
| Storage |	10 GB |
|OS |	Ubuntu Server |
| Network |	Bridged |

This setup is lightweight and suitable for old laptops or mini PCs.
