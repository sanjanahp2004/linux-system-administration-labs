# Linux Introduction and Fundamentals..

## 1. What Is an Operating System?

An Operating System (OS) is system software that manages computer hardware and software resources and provides an interface between users, applications, and hardware.

### Main Responsibilities of an Operating System
- Process management
- Memory management
- File system management
- Device management
- Security and access control
- Resource allocation

**Examples:** Linux, Microsoft Windows, macOS, Android.

## 2. What Is Linux?

Linux is an open-source, Unix-like operating system family built around the Linux kernel. Linux-based operating systems are widely used in servers, cloud computing, networking, embedded systems, and software development.

Linux is especially popular for server administration because of its flexibility, security features, command-line tools, automation capabilities, and broad support for development and infrastructure software.

## 3. What Is Open Source?

Open-source software makes its source code available under a license that permits users to use, inspect, modify, and redistribute it according to the license terms.

### Advantages of Open Source
- Transparency and community collaboration
- Customization and flexibility
- Community-developed improvements and fixes
- Reduced dependence on a single vendor
- Opportunities to learn from source code

**Examples:** Linux, Git, Python, and many Apache projects.

## 4. What Is the Linux Kernel?

The kernel is the core component of an operating system. It manages communication between software and hardware and controls important system resources.

### Main Responsibilities
- Process scheduling
- Memory management
- Device and driver management
- File system operations
- Network communication
- System calls that allow applications to request kernel services

**Example:** When a program requests data from a file, the kernel coordinates the required file system and storage operations.

## 5. What Is a Shell?

A shell is a command interpreter that accepts commands, interprets them, and requests the operating system to perform the required operations.

### Types of Linux Shells

| Shell | Description |
|---|---|
| Bash | Bourne Again Shell; widely used for interactive commands and scripting |
| sh | Traditional Bourne-style shell interface; implementations vary |
| Zsh | Interactive shell with extensive customization |
| Ksh | KornShell, used for interactive work and scripting |
| Fish | Friendly Interactive Shell with helpful interactive features |

**Example:**

```bash
echo "Hello Linux"
```

This command prints `Hello Linux` to the terminal.

## 6. What Is a Terminal?

A terminal is the interface through which a user interacts with a shell by entering commands and viewing their output.

A terminal emulator provides this interface in a graphical environment. Examples include GNOME Terminal and Windows Terminal.

### Terminal vs. Shell

- **Terminal:** Provides the interface for entering and viewing commands.
- **Shell:** Interprets commands and runs the requested operations.

## 7. Linux Distributions

A Linux distribution combines the Linux kernel with system utilities, package management tools, libraries, and applications to provide a usable operating system.

### Common Linux Distributions

| Distribution | Package Management | Common Use |
|---|---|---|
| Amazon Linux | DNF / YUM-compatible tooling | AWS cloud servers |
| Ubuntu | APT | Servers, cloud, and desktops |
| Debian | APT | Stable server and general-purpose systems |
| Red Hat Enterprise Linux (RHEL) | RPM with DNF | Enterprise environments |
| Fedora | DNF | Desktop and server environments |
| Rocky Linux | DNF | Enterprise-compatible server environments |

Package managers and available commands can vary by distribution version.

## 8. Linux vs. Windows

| Feature | Linux | Windows |
|---|---|---|
| Source code | Open source in many distributions and components | Primarily proprietary |
| Licensing | Depends on the distribution and included software | Primarily commercial licensing |
| Interface | Command line and graphical interfaces | Graphical interface and command-line tools |
| Administration | Commonly uses shells and configuration files | Commonly uses graphical tools, PowerShell, and other utilities |
| Customization | Extensive | Customization depends on the component |
| Software installation | Distribution-specific package managers and other methods | Installers, package managers, and application stores |
| Server and cloud usage | Widely used | Also widely used |
| Automation | Shell scripting and many automation tools | PowerShell and other automation tools |

Neither operating system is universally better. The appropriate choice depends on workload, application compatibility, administration requirements, and organizational needs.

## 9. Why Do DevOps Engineers Use Linux?

Linux is widely used in DevOps because many cloud servers, CI/CD environments, containers, and infrastructure tools run on Linux.

### Common Reasons
- **Server administration:** Manage users, permissions, processes, and services.
- **Cloud infrastructure:** Connect to and manage Linux virtual machines on platforms such as AWS.
- **Automation:** Use Bash scripts and command-line tools to automate repetitive tasks.
- **CI/CD pipelines:** Operate build and deployment tools such as Jenkins.
- **Containers:** Work with Linux-based container images and container runtimes.
- **Monitoring and troubleshooting:** Inspect logs, processes, network connectivity, and system resources.
- **Infrastructure management:** Use tools such as Ansible and Terraform alongside Linux environments.

## 10. Basic Linux Commands

### System Information

| Command | Purpose |
|---|---|
| `uname -a` | Display kernel and system information |
| `cat /etc/os-release` | Display distribution information |
| `whoami` | Display the current username |
| `hostname` | Display the system hostname |
| `date` | Display the system date and time |
| `uptime` | Display uptime and load information |

### Navigation Commands

| Command | Purpose |
|---|---|
| `pwd` | Print the current working directory |
| `ls` | List directory contents |
| `ls -la` | List entries, including hidden files, with details |
| `cd /path` | Change to a specified directory |
| `cd ..` | Move to the parent directory |
| `cd ~` | Change to the user's home directory |

### File and Directory Operations

| Command | Purpose |
|---|---|
| `mkdir test` | Create a directory |
| `touch file.txt` | Create an empty file if it does not exist |
| `cp source destination` | Copy a file |
| `mv source destination` | Move or rename a file |
| `rm file.txt` | Remove a file |
| `rmdir test` | Remove an empty directory |

**Caution:** `rm` can permanently remove files. Check the target before executing destructive commands.

### Viewing and Searching Files

| Command | Purpose |
|---|---|
| `cat file.txt` | Display file contents |
| `less file.txt` | View file contents interactively |
| `head file.txt` | Display the first lines |
| `tail file.txt` | Display the last lines |
| `grep "error" file.txt` | Search for matching text |
| `find /path -name "file.txt"` | Search for a filename under a path |

### Permissions and Processes

| Command | Purpose |
|---|---|
| `ls -l` | View file permissions and ownership |
| `chmod 644 file.txt` | Change file permissions |
| `chown user file.txt` | Change file ownership; normally requires appropriate privileges |
| `ps aux` | List processes |
| `top` | Monitor processes and resource usage |
| `kill PID` | Send a signal to a process by its process ID |

### Disk and Network Information

| Command | Purpose |
|---|---|
| `df -h` | Display filesystem disk space |
| `du -sh directory` | Display the total size of a directory |
| `free -h` | Display memory usage |
| `ip addr` | Display network interface addresses |
| `ip route` | Display routing information |
| `ss -tuln` | Display listening TCP and UDP sockets |

### Help Commands

| Command | Purpose |
|---|---|
| `man ls` | Open the manual page for a command |
| `ls --help` | Display command usage information |
| `history` | Display command history in supported shells |

Some options and utilities differ across distributions.

## 11. Practical Exercise

Run the following commands on a Linux machine and observe the output.

```bash
whoami
hostname
pwd
uname -a
cat /etc/os-release
ls -la
df -h
free -h
ip addr
uptime
```

### Verification Checklist

- [ ] Identified the Linux distribution.
- [ ] Checked the kernel and hostname.
- [ ] Navigated directories and listed files.
- [ ] Inspected disk and memory usage.
- [ ] Examined network interfaces.
- [ ] Read the help or manual for an unfamiliar command.

## 12. Key Takeaways

- An operating system manages hardware and software resources.
- Linux distributions use the Linux kernel together with system utilities and applications.
- The shell interprets commands, while a terminal provides an interface to interact with the shell.
- Linux is widely used in cloud computing, server administration, and DevOps workflows.
- Understanding commands and verifying their output is an essential foundation for Linux administration.

## References

- [The Linux Kernel Archives](https://www.kernel.org/)
- [GNU Bash Manual](https://www.gnu.org/software/bash/manual/)
- [Linux man-pages project](https://www.kernel.org/doc/man-pages/)

---

**Repository:** Linux System Administration & Troubleshooting Labs  
**Author:** Sanjana H.P.
