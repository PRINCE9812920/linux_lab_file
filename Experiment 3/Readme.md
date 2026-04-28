# Experiment: File and Directory Management in Linux

## Aim
To perform file and directory management in Linux and understand file permissions and text editors.

## Objective
* To learn navigation in the Linux file system.
* To create and manage files and directories.
* To understand file permissions.
* To use text editors like `nano` and `vi`.

## Theory

### Linux File System
Linux follows a hierarchical structure starting from the root directory `/`. All files and directories are organized in a tree-like format, which helps in efficient management and security.

### Files and Directories
* **Files** store data such as text, scripts, or programs.
* **Directories** organize files and other directories.

### File and Directory Permissions
Linux uses a permission model to control access:
* **Read (r)** – View contents
* **Write (w)** – Modify contents
* **Execute (x)** – Run files

Permissions are assigned to: **Owner**, **Group**, and **Others**.

### Text Editors
* `nano` – Simple and beginner-friendly editor.
* `vi` – Advanced and powerful editor used in Linux systems.

## Step-by-step Procedure

1. **First, logged into the Linux virtual machine.**
2. **Then, opened the terminal.**
3. **After that, displayed the current directory:**
   ```bash
   pwd
   ```

4. **Then, listed files and directories:**
   ```bash
   ls
   ls -l
   ```

5. **After that, created a new directory and moved into it:**
   ```bash
   mkdir linux_lab
   cd linux_lab
   ```

6. **Then, created files inside the directory:**
   ```bash
   touch file1.txt file2.txt
   ```

7. **After that, edited a file using nano editor:**
   ```bash
   nano file1.txt
   ```
   * Typed some text.
   * Saved using <kbd>Ctrl</kbd> + <kbd>O</kbd>.
   * Exited using <kbd>Ctrl</kbd> + <kbd>X</kbd>.

8. **Then, edited another file using vi editor:**
   ```bash
   vi file2.txt
   ```
   * Pressed <kbd>i</kbd> to enter insert mode.
   * Typed text.
   * Pressed <kbd>Esc</kbd>, then typed `:wq` to save and exit.

9. **After that, displayed file contents:**
   ```bash
   cat file1.txt
   ```

10. **Then, checked file permissions:**
    ```bash
    ls -l
    ```

11. **After that, changed file permissions:**
    ```bash
    chmod 755 file1.txt
    ```

12. **Finally, verified updated permissions:**
    ```bash
    ls -l file1.txt
    ```

## Configuration Commands
The following commands were utilized during this experiment:
```bash
pwd
ls
ls -l
cd
mkdir
rmdir
touch
cat
nano
vi
chmod
stat
```

## Observations / Results
* Files and directories created successfully.
* Text files edited using `nano` and `vi`.
* File contents displayed correctly.
* File permissions viewed and modified successfully.


## Conclusion
The experiment was successfully completed. File and directory management commands were executed properly, and file permissions were understood and modified. Practical knowledge of text editors and Linux file handling was gained.
