# Experiment: User and Group Management, File Ownership, and Permissions

## Aim
To perform user and group management in Linux and understand file ownership and permissions.

## Objective
* To create and manage user accounts.
* To create and manage groups.
* To understand file ownership and permissions.# Experiment: User and Group Management, File Ownership, and Permissions

## Aim
To perform user and group management in Linux and understand file ownership and permissions.

## Objective
* To create and manage user accounts.
* To create and manage groups.
* To understand file ownership and permissions.
* To apply special permissions like sticky bit.

## Theory

### Users in Linux
Each user in Linux has a username, UID, home directory, and default shell.
* **Types of users:**
  * **Root user** – Full access
  * **Normal users** – Limited access

### Groups in Linux
Groups are collections of users used for managing permissions efficiently. Each file belongs to an owner and a group.

### File Ownership


Ownership defines access rights to files. Commands like `chown` and `chgrp` are used to change ownership.

### Sticky Bit
Sticky bit is a special permission used in shared directories to prevent users from deleting others’ files.
**Example:**
```bash
chmod +t directory_name
```


## Step-by-step Procedure

1. **First, logged into the Linux system.**
2. **Then, opened the terminal.**
3. **After that, created a new user:**
   ```bash
   sudo useradd testuser
   sudo passwd testuser
   ```

4. **Then, verified the user:**
   ```bash
   id testuser
   ```

5. **After that, created a new group:**
   ```bash
   sudo groupadd testgroup
   ```

6. **Then, added the user to the group:**
   ```bash
   sudo usermod -aG testgroup testuser
   ```

7. **After that, checked group membership:**
   ```bash
   groups testuser
   ```

8. **Then, created a shared directory:**
   ```bash
   mkdir shared_dir
   ```

9. **After that, changed group ownership and permissions:**
   ```bash
   sudo chgrp testgroup shared_dir
   sudo chmod 770 shared_dir
   ```

10. **Then, applied sticky bit:**
    ```bash
    sudo chmod +t shared_dir
    ```

11. **Finally, changed file ownership:**
    ```bash
    sudo chown testuser:testgroup shared_file.txt
    ```

## Configuration Commands
The following commands were utilized during this experiment:
```bash
useradd
passwd
usermod
userdel
groupadd
groupdel
groups
chown
chgrp
chmod
id
```

## Observations / Results
* Users and groups created successfully.
* Users added to groups correctly.
* File and directory ownership modified.
* Permissions applied correctly.
* Sticky bit enabled for secure sharing.

## Conclusion
The experiment was successfully completed. User and group management operations were performed, and file ownership and permissions were understood. This experiment helped in learning how to securely manage access to system resources in Linux.
* To apply special permissions like sticky bit.

## Theory

### Users in Linux
Each user in Linux has a username, UID, home directory, and default shell.
* **Types of users:**
  * **Root user** – Full access
  * **Normal users** – Limited access

### Groups in Linux
Groups are collections of users used for managing permissions efficiently. Each file belongs to an owner and a group.

### File Ownership


Ownership defines access rights to files. Commands like `chown` and `chgrp` are used to change ownership.

### Sticky Bit
Sticky bit is a special permission used in shared directories to prevent users from deleting others’ files.
**Example:**
```bash
chmod +t directory_name
```


## Step-by-step Procedure

1. **First, logged into the Linux system.**
2. **Then, opened the terminal.**
3. **After that, created a new user:**
   ```bash
   sudo useradd testuser
   sudo passwd testuser
   ```

4. **Then, verified the user:**
   ```bash
   id testuser
   ```

5. **After that, created a new group:**
   ```bash
   sudo groupadd testgroup
   ```

6. **Then, added the user to the group:**
   ```bash
   sudo usermod -aG testgroup testuser
   ```

7. **After that, checked group membership:**
   ```bash
   groups testuser
   ```

8. **Then, created a shared directory:**
   ```bash
   mkdir shared_dir
   ```

9. **After that, changed group ownership and permissions:**
   ```bash
   sudo chgrp testgroup shared_dir
   sudo chmod 770 shared_dir
   ```

10. **Then, applied sticky bit:**
    ```bash
    sudo chmod +t shared_dir
    ```

11. **Finally, changed file ownership:**
    ```bash
    sudo chown testuser:testgroup shared_file.txt
    ```

## Configuration Commands
The following commands were utilized during this experiment:
```bash
useradd
passwd
usermod
userdel
groupadd
groupdel
groups
chown
chgrp
chmod
id
```

## Observations / Results
* Users and groups created successfully.
* Users added to groups correctly.
* File and directory ownership modified.
* Permissions applied correctly.
* Sticky bit enabled for secure sharing.

## Conclusion
The experiment was successfully completed. User and group management operations were performed, and file ownership and permissions were understood. This experiment helped in learning how to securely manage access to system resources in Linux.
