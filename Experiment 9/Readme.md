# Lab: Mounting and Unmounting File Systems in Linux

## 🎯 Objective
To identify storage devices, perform manual mount and unmount operations, and understand the role of the unified root directory structure in Linux system administration.

## 📖 Theory
Linux operates on a **single-root directory structure** (`/`). Unlike other operating systems that assign letters to drives (like `C:` or `D:`), Linux treats storage hardware as files located in the `/dev` directory.

### Key Concepts
* **Device Files:** Representations of hardware (e.g., `/dev/sda` for disks, `/dev/sda1` for partitions).
* **Mount Point:** A directory (e.g., `/mnt`, `/media`) where a physical device is logically attached to the file system.
* **Unmounting:** The critical process of safely detaching a device to flush write buffers and prevent data corruption.

---

## 🛠️ Command Toolkit
| Command | Purpose | Priority |
| :--- | :--- | :--- |
| `lsblk` | List block devices and their structure | High |
| `sudo fdisk -l` | Detailed partition table information | High |
| `sudo mkdir` | Create a mount point directory | Medium |
| `sudo mount` | Attach a device to the file system | **Critical** |
| `df -h` | Check mounted devices and disk space | High |
| `sudo umount` | Detach a device safely | **Critical** |

---

## 🚀 Procedure
### Step A: Identification
Run `lsblk` or `sudo fdisk -l` to find your target device (e.g., `/dev/sdb1`).

### Step B: Setup & Mounting
1. Create the mount point: `sudo mkdir /mnt/usb`
2. Mount the device: `sudo mount /dev/sdb1 /mnt/usb`
3. Verify using `df -h`.

### Step C: Safe Removal
1. Exit the mount directory: `cd ~`
2. Unmount the device: `sudo umount /mnt/usb`

---

## 📝 Observations
* Storage devices are only accessible after being mapped to a directory.
* Safe unmounting is a prerequisite for maintaining data integrity.
* The `df -h` command provides a human-readable summary of filesystem usage.

## ✅ Conclusion
Mounting is a fundamental skill in Linux file management, providing controlled access to storage and serving as a critical task for system administrators and cybersecurity professionals.
