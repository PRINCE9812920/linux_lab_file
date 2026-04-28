
# 🔬 **Experiment: Introduction to Linux Commands and System Targets**

---

## **1. Course Outcome Mapping**

* **CO1:** Familiarity with Linux environment, command-line interface, and system utilities.

---

## **2. Learning Outcomes**

After completing this experiment, the student will be able to:

* **LO1:** Execute basic Linux system and user-level commands.
* **LO2:** Understand Linux run levels (systemd targets).
* **LO3:** Use Linux help utilities to learn command syntax and options.
* **LO4:** Improve efficiency using command auto-completion.

---

## **3. Theory**

### **3.1 Linux Command Line Interface (CLI)**

The Linux CLI allows users to interact with the operating system by typing commands. It provides precise control over system operations and is often faster and more powerful than graphical interfaces.

---

### **3.2 System Run Levels / Targets**

Modern Linux systems use **systemd targets** instead of traditional run levels to define system states.

**Common targets:**

* **graphical.target** – Multi-user mode with GUI
* **multi-user.target** – Multi-user mode without GUI
* **rescue.target** – Single-user rescue mode
* **poweroff.target** – Shutdown system
* **reboot.target** – Restart system

---

### **3.3 Linux Help Utilities**

Linux provides built-in tools for learning commands:

* **man** – Displays detailed manual pages
* **--help** – Shows short command usage
* **Tab auto-completion** – Automatically completes commands and filenames

These tools help users become independent and efficient.

---

## **4. Commands Used**

| Command     | Description                         |
| ----------- | ----------------------------------- |
| `pwd`       | Display current working directory   |
| `ls`        | List files and directories          |
| `cd`        | Change directory                    |
| `whoami`    | Display current user                |
| `date`      | Show system date and time           |
| `uptime`    | Show system running time            |
| `man`       | Display manual pages                |
| `--help`    | Show command help                   |
| `systemctl` | Manage system services and targets  |
| `runlevel`  | Show previous and current run level |
| `clear`     | Clear terminal screen               |

---

## **5. Procedure**

1. Log in to the Linux virtual machine.

2. Open the Terminal.

3. Execute basic commands:

   ```bash
   pwd
   ls
   whoami
   date
   uptime
   ```

4. Navigate directories:

   ```bash
   cd /home
   cd ~
   ```

5. Use manual pages:

   ```bash
   man ls
   man cd
   ```

   Press **q** to exit.

6. Use help options:

   ```bash
   ls --help
   systemctl --help
   ```

7. Check system run level / target:

   ```bash
   runlevel
   systemctl get-default
   ```

8. Switch system targets:

   ```bash
   systemctl isolate multi-user.target
   systemctl isolate graphical.target
   ```

9. Using traditional run levels:

   ```bash
   sudo init 3
   sudo init 5
   ```

10. Practice auto-completion:

* Type partial command and press **Tab**

11. Clear terminal:

```bash
clear
```

---

## **6. Expected Output**

* Successful execution of Linux commands
* Display of manual pages and help information
* Identification of current run level or target
* Improved command-line efficiency

---

## **7. Result**

Basic Linux commands, system targets, and help utilities were successfully executed. The experiment provided practical understanding of the Linux command-line interface and improved user efficiency.

---

