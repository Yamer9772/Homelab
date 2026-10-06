# Homelab — Yousef Amer

Hands-on lab for CompTIA Security+ study and SOC Analyst (Tier 1) interview prep.
Built October 2026. Documented as I go — every project here is something I
actually built, broke, and fixed.

## The Lab

| Piece | Details |
|---|---|
| Hypervisor host | Dell OptiPlex 990 — i5-2400 (4 cores), 4 GB RAM, 500 GB HDD |
| Hypervisor | Proxmox VE 9 (node `pve`) |
| Network | Netgear EX6200 extender bridged to the Dell via Ethernet |
| Planned upgrades | 8 GB DDR3 RAM kit, 256 GB SATA SSD, CR2032 CMOS battery |

## Projects

| # | Project | Status |
|---|---|---|
| 01 | [Proxmox VE server build](projects/01-proxmox-server.md) | ✅ Done |
| 02 | [Ubuntu 24.04 LXC container](projects/02-ubuntu-container.md) | ✅ Done |
| 03 | [Kali Linux VM](projects/03-kali-vm.md) | ✅ Done |
| 04 | Vulnerable target VM (Metasploitable) for practice | 🔲 Planned |
| 05 | Splunk Free + BOTS dataset — learning SPL | 🔲 Planned |
| 06 | Jellyfin media server (self-hosted streaming) | 🔲 Planned |

## Roadmap

Working through a 6-month plan: Linux + networking foundations → Security+
certification → SOC analyst skills (alert triage, log analysis, incident
write-ups) → job hunt. One hour a day, lab-first.
