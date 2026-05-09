# Monitoring Targets

This document explains recommended monitoring targets for the homelab environment.

---

# Router Monitoring

## MikroTik Router

Method:
- Ping

Purpose:
- Detect router downtime
- Detect gateway failure

---

# Server Monitoring

## Ubuntu Server

Methods:
- Ping
- TCP Port
- SSH Port

Purpose:
- Detect server availability
- Detect SSH issues

---

# Web Service Monitoring

## HTTP/HTTPS Services

Examples:
- Nginx
- Apache
- CasaOS
- Nextcloud

Method:
- HTTP(s)

Purpose:
- Detect web service outages

---

# Docker Service Monitoring

Examples:
- Jellyfin
- Pi-hole
- Portainer

Method:
- HTTP
- TCP Port

Purpose:
- Monitor self-hosted services

---

# Internet Monitoring

## External Website Check

Examples:
- google.com
- cloudflare.com

Method:
- HTTP(s)

Purpose:
- Verify internet connectivity

---

# Recommended Naming Convention

| Service | Example Name |
|---|---|
| Router | MikroTik Gateway |
| Server | Ubuntu Docker Host |
| NAS | Home NAS |
| Internet | Internet Connectivity |

---

# Suggested Monitor Intervals

| Service Type | Interval |
|---|---|
| Router | 20 seconds |
| Server | 30 seconds |
| HTTP Services | 60 seconds |

---

# Monitoring Best Practices

- Use descriptive names
- Group related services
- Enable notifications
- Avoid excessive intervals
- Regularly review uptime reports
