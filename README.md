# Levan Khutsishvili (Tricksteridze)

**Linux · Monitoring · Networking · Infrastructure | Tbilisi, Georgia**

[Portfolio](https://tricksteridze.github.io/) · [LinkedIn](https://www.linkedin.com/in/levan-khutsishvili-0030b33a1) · [Email](mailto:levankhutsishvili@proton.me)

## About

I am a systems administration student and hands-on infrastructure builder focused on **Linux, monitoring, networking and operational troubleshooting**.

Alongside technical projects, I have **1.5+ years of experience in a 24/7 retail operation**, regularly working **3–4 consecutive 12-hour night shifts per week**. During those shifts I perform safe first-line checks of workstations, POS equipment, printers, power, cabling and local connectivity, document symptoms, follow remote IT instructions and escalate unresolved incidents with context.

I am looking to grow through real **MCR / NOC / monitoring / system administration** work where reliability, incident response and continuous learning matter.

## Verified Training & Credentials

- **Cisco Networking Academy — Linux Essentials** — completed, digital badge earned (Aug 2026)
- [Cisco Networking Academy — Operating Systems Basics](https://www.credly.com/badges/8d0d72ad-af80-441e-8965-692fa46e3388/public_url)
- [Cisco Networking Academy — Computer Hardware Basics](https://www.credly.com/badges/6422397e-60d1-4ffd-8da9-08899e3b1103/public_url)

## Core Skills

- **Linux / Unix:** Debian, Fedora, RHEL, Arch; CLI, systemd, users/groups, permissions, logs and basic troubleshooting
- **Monitoring / observability:** Prometheus, Grafana, Loki, Promtail, Telegraf
- **Networking:** TCP/IP, IPv4 addressing and subnetting, default gateways, ARP/MAC, DNS, DHCP, VLAN fundamentals, switching/routing concepts and troubleshooting
- **Cisco Packet Tracer:** hands-on labs with Cisco 1941 routers and 2960 switches; two-subnet routing, ARP/MAC-table behavior, gateway/mask/interface failures and diagnostic workflow
- **Infrastructure:** Docker, Docker Compose, Git, GitHub, KVM/libvirt
- **Automation:** Bash and Python
- **Windows:** Windows 10/11, Windows Server, Active Directory fundamentals, workstation/peripheral troubleshooting

## Featured Projects

### [Linux Observability Stack](https://github.com/Tricksteridze/linux-observability-stack)
Self-hosted monitoring for a Linux host built with **Telegraf → Prometheus → Grafana** for metrics and **Promtail → Loki → Grafana** for container logs.

- Docker Compose deployment with automatic Grafana datasource/dashboard provisioning
- Persistent Prometheus, Loki and Grafana data using named volumes; Prometheus retention set to 15 days
- Startup script generates the Grafana admin password and detects the host Docker socket GID automatically
- Services bind to localhost by default; remote access is documented through Tailscale/WireGuard instead of exposing monitoring services directly to the Internet
- Docker socket permissions handled with `group_add`; SELinux-aware mounts; no `privileged` containers
- Includes troubleshooting notes for failed Telegraf targets, Docker socket permission problems and stopped/restarting containers

### [Asterisk Gemini Voice Assistant](https://github.com/Tricksteridze/asterisk-gemini-voice)
Self-hosted SIP voice assistant built with **Asterisk PBX, Python FastAGI and Docker Compose**.

- Configured a PJSIP endpoint and Asterisk call flow
- Python FastAGI server handles calls over TCP and processes concurrent calls in separate threads
- DTMF menu selects Russian or English
- Complete voice pipeline: **Asterisk recording → speech recognition → Gemini → gTTS/ffmpeg → Asterisk playback**
- Added retry/error handling around external AI requests and call hangup handling

### [Termux Debian Workstation](https://github.com/Tricksteridze/termux-debian-workstation)
Automated deployment of a full **Debian XFCE environment on Android without root**.

- Bash installer deploys Debian with `proot-distro` and installs/configures XFCE, Termux-X11, VirGL and PulseAudio
- Generates a reusable startup script for graphics, audio and desktop-session startup
- Includes environment configuration, package setup and a check for Android's Phantom Process Killer
- Designed as a reproducible one-command setup rather than a manual installation guide

### [Official RimWorld Georgian Localization](https://github.com/Ludeon/RimWorld-Georgian)
Long-running open-source work on the official Georgian localization maintained under the **Ludeon Studios GitHub organization**.

- Worked across **34,000+ translated lines and 100+ XML files** and used Python/XML automation for repetitive processing
- Submitted a **merged pull request** that migrated the repository from the old flat structure to the current multi-DLC layout (`Core`, `Royalty`, `Ideology`, `Biotech`, `Anomaly`, `Odyssey`)
- Practical experience with Git branches, pull requests, repository restructuring and maintaining structured data at scale

## Troubleshooting Approach

**Confirm symptoms → define scope → check physical/connectivity state → inspect logs/resources/configuration → apply the safest reversible action → verify recovery → document and escalate with evidence.**

That is the same process I use in both live operational issues and personal infrastructure projects.

## Current Direction

My current focus is **Linux/Unix fundamentals, monitoring, networking and incident response**, with the goal of developing through real 24/7 infrastructure operations and later moving deeper into system administration and infrastructure engineering.
