# Experiment: Package Management in Linux using RPM and YUM

## Aim
To perform package management in Linux using RPM and YUM.

## Objective
* To understand package management in Linux.
* To install, query, and remove packages using `rpm`.
* To use `yum` for package installation and updates.
* To understand dependency management.

## Theory

### Package Management in Linux
A package is a compressed file containing software, configuration files, and metadata. Package managers automate the installation, updates, and removal of software.



### RPM (Red Hat Package Manager)
`rpm` is a low-level package manager used in Red Hat-based systems. It allows the installation, querying, and removal of packages but does not resolve dependencies automatically.

### YUM (Yellowdog Updater Modified)
`yum` is a high-level package manager that works on top of `rpm` and automatically handles dependencies by downloading required packages from repositories.



## Step-by-step Procedure

### A. Using RPM

1. **First, logged into the Linux system and opened the terminal.**
2. **Then, listed all installed RPM packages:**
   ```bash
   rpm -qa
   ```

3. **After that, checked package information:**
   ```bash
   rpm -qi bash
   ```

4. **Then, installed an RPM package:**
   ```bash
   sudo rpm -ivh package_name.rpm
   ```

5. **After that, verified installation:**
   ```bash
   rpm -qa | grep package_name
   ```

6. **Finally, removed the package:**
   ```bash
   sudo rpm -e package_name
   ```

### B. Using YUM

7. **Then, searched for a package:**
   ```bash
   yum search nano
   ```

8. **After that, installed the package:**
   ```bash
   sudo yum install nano
   ```

9. **Then, verified installation:**
   ```bash
   nano --version
   ```

10. **After that, listed installed packages:**
    ```bash
    yum list installed
    ```

11. **Then, removed the package:**
    ```bash
    sudo yum remove nano
    ```

12. **Finally, updated system packages:**
    ```bash
    sudo yum update
    ```

## Configuration Commands
The following commands were utilized during this experiment:
```bash
rpm -qa
rpm -qi
rpm -ivh
rpm -e
yum search
yum install
yum remove
yum update
yum list installed
```

## Observations / Results
* Installed packages listed successfully.
* Package information displayed correctly.
* Software installed and removed using `rpm` and `yum`.
* Dependencies resolved automatically using `yum`.
* System packages updated successfully.


## Conclusion
The experiment was successfully completed. Package management operations were performed using RPM and YUM. This experiment helped in understanding how to install, update, query, and remove software packages efficiently in Linux systems.
