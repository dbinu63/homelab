# System Architecture

This document provides a detailed overview of the homelab’s technical design and component interactions.

## Components

**NAS Server**
- Hardware: Dell Optiplex 790, i7-2600, 32GB RAM, 128GB + 500GB SSD
- OS: Debian
- NAS Management: OpenMediaVault

**Containerization**
- Docker Engine
- Portainer (web UI for container management)

**Networking**
- LAN for local workstation connections
- Tailscale VPN for remote access from MacBook or other devices

## Connections & Data Flow

Workstations interact with the NAS as follows:

- PC Workstation → LAN → NAS
- MacBook → Tailscale VPN → NAS
- Docker containers run on NAS and provide additional services to connected workstations

### Diagram
   (PC Workstation)
         |
         | LAN
         v
   (NAS Server)---(Docker Containers)
         ^
         | Tailscale VPN
         |
   (MacBook / Remote)


## Current Functionality

- Centralized storage accessible locally and remotely
- Containerized services deployed on NAS
- Secure VPN connections for offsite access

## Future Expansion

- Syncthing for automated cross-device file synchronization
- Flamenco for distributed Blender rendering
- Automated backup and system monitoring
- Additional containerized services for workflow optimization
