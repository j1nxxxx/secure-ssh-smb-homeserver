# Secure Linux Server: SSH + SMB Setup

This project documents the setup and hardening of a Linux-based home server with:

- **SSH**: Secure shell access with key-based authentication, hardended config
- **SMB (Samba)**: Public and private shares for LAN clients

## Tech Stack
- Operating System: Debian Linux
- Bash Shell Scripting

## Features

- SSH with custom ports
- Samba share for easy access from Windows, Linux and Android clients
- UFW Firewall

## Use Cases

- Home NAS-style setup
- Remote file management

## Network Security
- Restricted SSH and SMB access to specific IP address ranges/subnets to limit exposure

## User Access Controls
- Configured Samba with valid users only; disbaled guest access to prevent unauthorised file sharing
- Hardened SSH access with key-based authentication and moved SSH to a non-standard port 2222 to reduce automated attacks

## Protocol Security
- Disbaled outdated and vulnerable protocols such as SMBv1 to enhance network security
- Applied strict global security policies on Samba to ensure encrypted and secure communications
