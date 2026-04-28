# 🐧 Linux File & Directory Management Lab

---

## 📋 Experiment Title / Aim
To perform file and directory management in Linux and understand file permissions and text editors.

---

## 🎯 Objective
* **Navigate** the Linux file system hierarchy.
* **Create and Manage** files and directories using the CLI.
* **Understand** and modify file permissions ($rwx$).
* **Master** terminal text editors like `nano` and `vi`.

---

## 📖 Theory 
**Linux File System:** Follows a hierarchical tree structure starting from the root `/`.


**Files & Directories:** * **Files:** Store data (text, scripts, programs).
* **Directories:** Organize files and other sub-directories.

**File Permissions:** Linux controls access using a three-tier model:
1.  **Read (r):** View contents.
2.  **Write (w):** Modify contents.
3.  **Execute (x):** Run files.
*Permissions are assigned to the **Owner**, **Group**, and **Others**.*

**Text Editors:**
* **nano:** Simple, modeless, and beginner-friendly.
* **vi:** Advanced, modal editor used globally in Linux systems.

---

## 🛠️ Step-by-Step Procedure

1.  **Login:** Logged into the Linux virtual machine and opened the **Terminal**.
2.  **Locate:** Displayed current path using `pwd` and listed files using `ls -l`.
3.  **Create:** Created a new directory named `linux_lab` and navigated into it:
    ```bash
    mkdir linux_lab && cd linux_lab
    ```
4.  **Generate:** Created two files: `file1.txt` and `file2.txt` using the `touch` command.
5.  **Edit (Nano):** Opened `file1.txt` using `nano`, typed text, saved with `Ctrl+O`, and exited with `Ctrl+X`.
6.  **Edit (Vi):** Opened `file2.txt` using `vi`, pressed `i` for Insert mode, typed text, and saved/exited with `Esc` then `:wq`.
7.  **View:** Displayed the contents of the files using the `cat` command.
8.  **Security:** Checked initial permissions with `ls -l`, then modified `file1.txt` permissions:
    ```bash
    chmod 755 file1.txt
    ```
9.  **Verify:** Confirmed updated permissions using `ls -l` and `stat`.

---

## 💻 Configuration Commands

| Command | Function |
| :--- | :--- |
| `pwd` | Print Working Directory |
| `ls -l` | List files with long format (permissions/size) |
| `cd` | Change Directory |
| `mkdir` | Make Directory |
| `touch` | Create empty file |
| `cat` | View file content |
| `nano` / `vi` | Terminal text editors |
| `chmod` | Change file mode/permissions |
| `stat` | Display detailed file/file system status |

---

## 📸Results 

* Files and directories were created successfully.
* Text files were edited and saved using both `nano` and `vi`.
* File permissions were successfully modified and verified.

---

## ✅ Conclusion
The experiment was successfully completed. Practical knowledge of the Linux CLI was gained, specifically in managing the file system and understanding the security implications of file permissions.

---
<div align="center">
  <b>End of Lab Report</b>
</div>
