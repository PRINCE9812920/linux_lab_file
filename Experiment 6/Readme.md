# Experiment: Exploring Virtual Terminals, Display Managers, and the X Window System

## Aim
To explore virtual terminals, display managers, X Window System, and switching between text and graphical interfaces in Linux.

## Objective
* To understand virtual terminals in Linux.
* To switch between multiple terminals.
* To study display managers and graphical login.
* To identify X clients and window managers.

## Theory

### Virtual Terminals
Linux provides multiple virtual terminals (VTs) that allow multiple sessions to run simultaneously in text mode. These are useful for troubleshooting and system recovery.

**Common shortcuts:**
* <kbd>Ctrl</kbd> + <kbd>Alt</kbd> + <kbd>F1</kbd> to <kbd>F6</kbd> – Text terminals
* <kbd>Ctrl</kbd> + <kbd>Alt</kbd> + <kbd>F7</kbd> – Graphical interface



### Display Manager
A display manager provides a graphical login interface and manages user sessions.
* **Examples:** GDM, LightDM, SDDM

### X Window System (X11)
The X Window System handles graphical display, keyboard, and mouse input. It allows graphical applications to run in Linux.

### X Clients
X clients are graphical applications such as terminals, browsers, and editors that interact with the X server.

### Window Manager
A window manager controls the appearance and behavior of windows.
* **Examples:** GNOME, KDE, Xfce, Openbox

## Step-by-step Procedure

1. **First, logged into the Linux system.**
2. **Then, opened the terminal.**
3. **After that, checked the current terminal:**
   ```bash
   tty
   ```

4. **Then, switched to another virtual terminal using:**
   * <kbd>Ctrl</kbd> + <kbd>Alt</kbd> + <kbd>F2</kbd>

5. **After that, logged in again and verified terminal access.**

6. **Then, switched back to graphical mode using:**
   * <kbd>Ctrl</kbd> + <kbd>Alt</kbd> + <kbd>F1</kbd> OR <kbd>Ctrl</kbd> + <kbd>Alt</kbd> + <kbd>F7</kbd>

7. **After that, checked logged-in users:**
   ```bash
   who
   w
   ```

8. **Then, checked display manager status:**
   ```bash
   systemctl status gdm
   ```

9. **After that, verified X session variable:**
   ```bash
   echo $DISPLAY
   ```

10. **Finally, listed X-related processes:**
    ```bash
    ps -e | grep X
    ```

## Configuration Commands
The following commands were utilized during this experiment:
```bash
tty
who
w
systemctl
echo $DISPLAY
ps
startx
```

## Observations / Results
* Successfully switched between virtual terminals.
* Current terminal identified using `tty`.
* Logged-in users displayed correctly.
* Display manager status checked successfully.
* X session variable verified.
* Running X processes displayed.


## Conclusion
The experiment was successfully completed. Virtual terminals, display managers, X clients, and window managers were explored. This experiment provided practical understanding of Linux system interfaces and graphical session management.
