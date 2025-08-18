**sam‑OS** is a lightweight, open‑source Linux‑based operating system built entirely from scratch as a fun and experimental project.  
It embraces minimalism, the spirit of free software, and offers a transparent look into the process of building an OS from the ground up.

---

## ⚠️ Important Notice

**sam‑OS is designed to run *only* inside virtual machines** such as:

- VMware
- QEMU
- VirtualBox

It is **not intended for installation on real/physical hardware**.  
Running it outside a VM is not supported and may result in unexpected behavior.

---

## ✨ Features

- Built entirely from scratch for educational and experimental purposes
- Minimalist Linux‑based environment
- Fully open‑source under the GNU GPL v3 license
- Source code available for anyone to explore, modify, and share
- Lightweight footprint — ideal for VM experimentation

---

## 🛠 Getting Started

### 1. Download the sam‑OS Image
The latest `.img` file is available in the [**Releases**](../../releases) section of this repository.  
Download it to your computer before proceeding.

### 2. Run in a VM
#### Example with QEMU:
```bash
qemu-system-x86_64 -hda sam-os.img -m 1024 -vga qxl<(or virtio)> -device virtio-net-pci,netdev=netdev0   
