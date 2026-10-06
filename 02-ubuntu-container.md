# Project 02 — Ubuntu 24.04 LXC Container

**Date:** October 2026
**ID:** CT 100 (`ubuntu-lab`)

## Objective

A lightweight Linux playground on the Proxmox host for learning the terminal,
Linux fundamentals, and general tinkering — without the overhead of a full VM.

## What I did

1. Created an LXC container from the Ubuntu 24.04 template via the Proxmox UI.
2. Started it and verified it via the built-in console.

## What I learned

- Containers vs. VMs: LXC shares the host kernel, so it's far lighter on RAM
  — important on a 4 GB host.
- When to use a container (lightweight Linux practice) vs. a full VM
  (Kali, which needs its own kernel and toolset).

## Next

Use this container for TryHackMe-style Linux drills: file permissions, users,
processes, networking commands, bash basics.
