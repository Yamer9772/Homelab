# Project 03 — Kali Linux VM

**Date:** October 2026
**ID:** VM 101 (`kali`)

## Objective

A dedicated offensive-security workstation for ethical hacking practice —
staying strictly inside my own lab network.

## What I did

1. Downloaded the Kali Linux installer ISO (~4 GB) to the Proxmox host.
2. Created the VM: **2 CPU cores, 2 GB RAM, 32 GB disk**, Kali ISO attached.
3. Installed via **Graphical Install** with defaults:
   - Hostname `kali`, no domain (home lab — not needed)
   - Guided partitioning, entire virtual disk, all files in one partition
4. Shut down the Ubuntu container first so Kali had the RAM to itself
   (4 GB host — only one heavy guest runs comfortably at a time).

## What I learned

- Sizing VMs against real hardware constraints: 2 GB of 3.7 GB usable means
  one guest at a time until the RAM upgrade.
- The Kali installer flow: hostname, domain (skip it), user setup,
  partitioning choices and what they mean.

## Next

- Deploy a deliberately vulnerable target (Metasploitable) and practice
  scanning it with Nmap from Kali — all inside the lab.
- Connect Kali to TryHackMe via OpenVPN to bypass the free-tier AttackBox
  time limit.
