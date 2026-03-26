# homelab

This repository documents a personal homelab built around a NAS (Network Attached Storage) system using Debian, OpenMediaVault, Docker, and Tailscale.  
The project demonstrates hands-on experience with Linux administration, containerized services, and secure remote networking.  
Primary use case: managing large Blender projects across multiple devices.

---

## Hardware

| Component     | Specs / Software     |
| ------------- | -------------------- |
| CPU           | i7-2600              |
| RAM           | 32GB                 |
| Storage       | 128GB SSD, 500GB SSD |
| OS            | Debian               |
| NAS Mgmt      | OpenMediaVault       |
| Containers    | Docker + Portainer   |
| Remote Access | Tailscale VPN        |

---

## Software Stack

- Debian (base OS)
- OpenMediaVault (NAS management)
- Docker (containerization)
- Portainer (container management UI)
- Tailscale (secure remote networking)

---

## Current Features

- Network-attached storage accessible across local network
- Secure remote access using Tailscale VPN
- Web-based management via OpenMediaVault
- Docker environment for running additional services
- Container management through Portainer
- Syncthing for automated file synchronization

---

## Planned Features

- Flamenco for distributed Blender rendering management
- Automated backup workflows
- Additional monitoring and system automation tools

---

## System Design

The system is designed as a central storage and service node:

- Workstations connect to the NAS over LAN or Tailscale
- Files are stored and accessed from a single centralized location
- Docker containers run additional services on top of the base system

---

## Lessons Learned

- Hands-on experience with Linux system setup and configuration
- Learned how to configure secure remote networking using Tailscale
- Explored Docker container management using Portainer
- Understood the basics of NAS systems and centralized storage

---

## Future Improvements

- Expand into a full homelab with monitoring and automation
- Improve system reliability with backup strategies
- Optimize performance for large file transfers and rendering workflows
- Remove Syncthing from using relay servers while on LAN

---
