# Project 01 — Proxmox VE Server Build

**Date:** October 2026
**Host:** Dell OptiPlex 990 (i5-2400, 4 cores / 4 GB RAM / 500 GB HDD)

## Objective

Turn an old office PC into a bare-metal virtualization host for security lab
work — the foundation everything else runs on.

## What I did

1. Installed Proxmox VE 9 from USB (Debian-based, `trixie`).
2. Hit the classic gotcha: Proxmox ships pointed at the **paid enterprise
   repositories**, so `apt update` fails without a subscription. Fixed it by
   removing the enterprise `.sources` files and adding the free
   **no-subscription** feed:
   `deb http://download.proxmox.com/debian/pve trixie pve-no-subscription`
3. Ran `apt update && apt full-upgrade -y` — 182 packages — and rebooted clean.
4. Node `pve` reachable on the LAN at `https://192.168.12.100:8006`.

## Networking

The Dell sits next to a Netgear EX6200 WiFi extender paired to the home
gateway, wired to the Dell via Ethernet. No monitor/keyboard — the box runs
**headless** and is managed entirely through the Proxmox web UI.

## What I learned

- The difference between Proxmox's enterprise vs. no-subscription repos (and
  that this version uses DEB822 `.sources` files, not the old `.list` format).
- Why a type-1 hypervisor beats VirtualBox for a 24/7 lab box.
- Headless management: if the web UI is up, the machine doesn't need a screen.

## Next

- RAM upgrade to 8 GB (current 4 GB is the binding constraint).
- Migrate Proxmox to a 256 GB SSD when budget allows.
