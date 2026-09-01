# File Hierarchy
### Introduction:

**File System Hierarchy** is a method of organizing and storing data in a structured way
using files and folders. It arranges files into different levels of directories and sub-directories,
making data easy to manage, locate, access and retrieve.

Linux follows a hierarchical tree structure that makes navigation simple and logical.

---------

## Let's learn about all files and folder in this hierarchy:

  - /(root): It is main directory also referred as parent directory under which all files and folders reside
    ![root_dir](/file_hierarchy/Screenshots/root_dir.png)
  - /bin: This directory contains essential commands and binaries needed by all users. For example: cd, ls, pwd, cat, etc.
    ![bin](/file_hierarchy/Screenshots/bin.png)
  - /sbin: This directory contains administrative binaries like iptables, firewall, init, etc.
    ![sbin](/file_hierarchy/Screenshots/sbin.png)
  - /boot: This directory stores required to boot the operating system. GRUB files are located under /boot
  - /dev: This directory contains device files. These files acts as interface between hardware and software
  - /etc: This directory contains the system configuration files. For example: cron.d, apache, nginx, etc
  - /home: This directory contains the personal home directories of all non-root users.
  - /lib: This directory contains 32-bit libraries required by 32-bit applications to run. For example: systemd, init, apache2, etc
  - /lib64: This directory contains 64-bit libraries. For example: ld-linux-x86-64.so.2
  - /bin.usr-is-merged, /sbin.usr-is-merged and lib.usr-is-merged: These directories are created during system upgrades to prevent package manager conflicts.
  - /lost+found: This directory contains the corrupted data fragments that are stored by the system while system recovery.
  - /media: This directory contains automatic mount points for removable media. For example: USB, SSD, and CD
  - /mnt: Temporary mount point for administrators to manually mount the external storage device or filesystem.
  - /opt: This directory contains the third-party softwares and packages that are not the part of the default system
  - /proc: This directory contains information about all the running processes and  system resources.
  - /root: The independent home directory of super user also called root user.
  - /run: It stores last volatile runtime data since the last system boot.
  - /snap: The default mount point where files and folders for installed snap packages resides.
  - /srv: This directory contains the site-specific data that is served by this system. For example: Data and scripts that serve for web servers.
  - /sys: The virtual filesystem that exposes information about the system's hardware drivers and kernel configuration settings.
  - /tmp: This directory stores temporary files created during program execution.
  - /usr: The Unix System Resources folder. It serves as the second hierarchy for user utilities and software.
  - /var: These are the variable files that continuously change while the system runs.
