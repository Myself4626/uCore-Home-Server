# uCore Home Server (uHS)

> ⚠️ **Warning:** Early stage. Features may change or be missing. Backups recommended.

---

**uHS** is an Ansible deployed home server. It's goal is to make lightweight, reproducible, container-first systems.  
It’s built on top of [uBlue’s uCore](https://universal-blue.org/ucore/) and uses [PerfectMediaServer](https://perfectmediaserver.com/) principles.

Instead of locking you into an appliance-style NAS, **uHS** focuses on being **simple, transparent, and maintainable**.  
Disks, containers, and services are all managed directly on the host, without hiding them behind heavy VMs or custom middleware.

---

## What makes it different?

- **Immutable base** – Atomic updates, easy rollback, no update drift.
- **Standard tooling** — Podman, systemd, and Ansible. No proprietary daemons or custom web frameworks.
- **Container-first design** – Apps run as containers via Podman + systemd quadlets.  
- **Flexible storage** — Mix and match to fit your data needs. Btrfs, MergerFS, SnapRAID, and ZFS.
- **Automated configuration** – Ansible manages everything, versioned in Git, self-documenting.  
- **Lightweight management** – Cockpit provides a simple web UI for monitoring, logs, and one-off tasks.  

---

## What this repo is:
The **automation layer** for my uCore Home Server: a curated set of Ansible roles and inventories that configure apps and services on top of my uHS OS image. Containers are managed with systemd quadlets for durability and clean lifecycle management.

## What this repo is not:
This is **not** the OS image builder. Install uBlue/uCore, then switch to the uHS OS image and manage services here. See the [OS](https://github.com/Myself4626/uCore-Home-Server-OS) project for install/bootc image-mode details.

---

## Philosophy:

The project builds on the principles of [Perfect Media Server](https://perfectmediaserver.com/):
- Use **proven, upstream tools** instead of custom solutions.
- Keep the design **modular and understandable**.
- Make it **easy to replace** or rebuild any piece if needed.

---

## Getting Started:

1. Install **uHS OS** on your hardware.
2. Clone this [uCore Home Server](https://github.com/Myself4626/uCore-Home-Server) repository.
3. Configure Ansible to match your host.
4. Run ansible.

---

## Contribute:

Got an idea for a service, role, or improvement?  
Open an issue or submit a PR — contributions are welcome!
