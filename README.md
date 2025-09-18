# CyberWatchDoug
Engineer by mind and of heart. I consider my work to be at the crossroads of infrastructure, security, and DevOps.

In the mind of an engineer working in IT, every error is a puzzle waiting to teach something new. 

What others see as failure, I see as feedback. It’s not just about solving the problem. It’s about becoming better with every line of code that didn’t work the first time.

I also run a blog at [https://blog.cyberwatchdoug.com](https://blog.cyberwatchdoug.com)

## Homelab

Everything starts and stops with my homelab. It's where I get to break, fix, and rebuild in a continuous cycle to learn and harnes my craft of working in IT engineering.

### Version 1

My original homelab was designed for resilience, automation, and security-first networking.

- The backbone features on OPNsense firewall running on a Protectli Vault Pro.
- Proxmox running on a Dell Optiplex 3080 (i5-10500T, 16GB RAM, dual NICs)
  - I added an additional NIC for my management VLAN
  - This runs VMs and LXCs
- Proxmox running on my old custom PC (will add stats soon)
  - Multiple NICs for management VLAN
  - Runs VMs and LXCs

Main services in my homelab include:
- Omada SDN, running in Podman on a Fedora VM. Provides centralized management for VLANs and my wireless network.
  - Tied into my TP-Link TL-SG2008 V3, and TP-Link AX5400 AP
- Pihole, running in Debian-based LXC
- Docmost, running in Debian-based LXC
- Caddy, running in Debian-based LXC (my reverse proxy for accessing services/apps)
- Proxmox Backup Server (PBS) running as a VM inside Proxmox, with a dedicated passthrough hard drive.
- OpenMediaVault (OMV) running as a VM inside Proxmox, with a dedicated passthrough hard drive
- Ansible, running from Fedora VM to manage various configurations.

Network Segmentation
- I primarily use VLANs to segment out my network
  - Management VLAN
  - IoT VLAN
  - Work VLAN
  - Default VLAN

## Projects

**homelab_ansible**

  a collection of Ansible playbooks and scripts designed to automate the setup, configuration, backup, and management of services in a personal homelab environment. It includes automation for user bootstrapping, lightweight Kubernetes (k3s) deployment, Paperless-NGX backup routines, and secure credential management using Ansible Vault, with a focus on Fedora Linux and OpenMediaVault systems.

<!-- insert cool links here and trackers -->

<!-- ## Projects
A high-level overview of each of my github projects.  

###  -->
<!--
**cyberwatchdoug/cyberwatchdoug** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

For markdown formatting reference:
https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#alerts

For emoji-cheat-sheet reference:
https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md
-->
