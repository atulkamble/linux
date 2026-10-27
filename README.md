## 1. Introduction to Linux Operating System

### What is Linux?

1. Linux is an open-source, Unix-like operating system family.
2. Linux was created by Linus Torvalds in 1991.
3. The Linux kernel manages hardware and system resources.
4. Linux supports CLI (Command Line Interface) and GUI (Graphical User Interface).
5. Linux is widely used in servers, cloud computing, DevOps, networking, and cybersecurity.

### Linux Operating System Architecture

```
        +----------------------------------+
        |              User                |
        |     Administrator / Developer    |
        +----------------------------------+
                        |
                        v
        +----------------------------------+
        |       Applications / Shell       |
        |         CLI / GUI / Bash         |
        +----------------------------------+
                        |
                        v
        +----------------------------------+
        |          Linux Kernel            |
        | Process / Memory / Device Mgmt   |
        +----------------------------------+
                        |
                        v
        +----------------------------------+
        |            Hardware              |
        |    CPU / RAM / Storage / Network |
        +----------------------------------+
```

Points to Remember:

1. User: Interacts with the Linux system.
2. Applications / Shell: Provides interfaces and executes user commands.
3. Linux Kernel: Manages processes, memory, devices, and system resources.
4. Hardware: Physical or virtual resources such as CPU, RAM, storage, and networking.

### Uses of Linux

| Area            | Examples                    |
| --------------- | --------------------------- |
| Cloud Computing | AWS EC2, Azure VM, GCP      |
| DevOps          | Jenkins, Docker, Kubernetes |
| Web Servers     | Apache, Nginx               |
| Databases       | MySQL, PostgreSQL           |
| Automation      | Bash, Ansible               |
| Cybersecurity   | Kali Linux                  |

Points to Remember

- Linux kernel was created in 1991.
- Linux is open-source.
- Linux supports multiple users and processes.
- Linux is commonly used for cloud and DevOps workloads.

## 2. Features of Linux

| Feature            | Description                                              |
| ------------------ | -------------------------------------------------------- |
| Open Source        | Source code is publicly available                        |
| Multiuser          | Multiple users can access a system                       |
| Multitasking       | Runs multiple processes simultaneously                   |
| Security           | Supports users, groups, permissions, and access controls |
| Stability          | Suitable for long-running workloads                      |
| Portability        | Supports multiple hardware architectures                 |
| CLI & GUI          | Supports command-line and graphical interfaces           |
| Networking         | Supports SSH, HTTP, DNS, and other protocols             |
| Automation         | Supports shell scripting                                 |
| Package Management | Supports tools such as apt and dnf                       |

Points to Remember

1. Linux is commonly used for server administration.
2. Linux supports automation using shell scripts.
3. Linux provides file permissions and user management.
4. Linux supports remote access through SSH.
5. Linux runs on physical servers, virtual machines, and cloud infrastructure.

## 3. Flavors of Linux (Linux Distributions)

### Types of Linux

| Linux Distribution    | Family / Ecosystem | Package Manager | Usage                  |
| --------------------- | ------------------ | --------------- | ---------------------- |
| Ubuntu                | Debian             | apt             | Cloud, DevOps, desktop |
| Debian                | Debian             | apt             | Servers                |
| Kali Linux            | Debian             | apt             | Cybersecurity          |
| RHEL                  | Red Hat            | dnf             | Enterprise servers     |
| Fedora                | Red Hat ecosystem  | dnf             | Development            |
| Rocky Linux           | RHEL-compatible    | dnf             | Enterprise servers     |
| AlmaLinux             | RHEL-compatible    | dnf             | Enterprise servers     |
| Amazon Linux 2023     | AWS-maintained     | dnf             | AWS EC2                |
| SUSE Linux Enterprise | SUSE               | zypper          | Enterprise workloads   |
| Arch Linux            | Arch               | pacman          | Advanced Linux users   |
| Alpine Linux          | Independent        | apk             | Lightweight containers |

### Linux Distribution Family Diagram

Linux Kernel

Debian

Ubuntu, Kali, Debian

Red Hat Ecosystem

RHEL, Fedora, Rocky

SUSE

SLES, openSUSE

Arch

Arch Linux, Manjaro

Other: Amazon Linux, Alpine Linux

### Types Based on Usage

| Type              | Example                    |
| ----------------- | -------------------------- |
| Desktop Linux     | Ubuntu Desktop, Linux Mint |
| Server Linux      | Ubuntu Server, RHEL        |
| Cloud Linux       | Amazon Linux, Ubuntu       |
| Enterprise Linux  | RHEL, SUSE                 |
| Security Linux    | Kali Linux                 |
| Lightweight Linux | Alpine Linux               |

Points to Remember

1. Ubuntu and Debian use `apt`.
2. RHEL and Amazon Linux 2023 use `dnf`.
3. SUSE uses `zypper`.
4. Arch Linux uses `pacman`.
5. Amazon Linux 2023 is used for today's AWS EC2 practical.

## 4. Difference Between Linux and Windows

| Parameter        | Linux                  | Windows                      |
| ---------------- | ---------------------- | ---------------------------- |
| Source Code      | Open-source kernel     | Proprietary                  |
| Developer        | Community and vendors  | Microsoft                    |
| Interface        | CLI and GUI            | GUI and CLI                  |
| File System      | ext4, XFS              | NTFS, ReFS                   |
| Path Separator   | `/`                    | `\`                          |
| Shell            | Bash, Zsh              | CMD, PowerShell              |
| Package Manager  | apt, dnf               | winget, MSI                  |
| Case Sensitivity | Usually case-sensitive | Usually case-insensitive     |
| Remote Access    | SSH                    | RDP, SSH                     |
| Usage            | Servers, cloud, DevOps | Desktop, enterprise, servers |

### Linux vs Windows Commands

| Operation         | Linux    | Windows CMD |
| ----------------- | -------- | ----------- |
| Current Directory | `pwd`    | `cd`        |
| List Files        | `ls`     | `dir`       |
| Change Directory  | `cd`     | `cd`        |
| Clear Screen      | `clear`  | `cls`       |
| Current User      | `whoami` | `whoami`    |
| Create Directory  | `mkdir`  | `mkdir`     |
| Copy File         | `cp`     | `copy`      |
| Delete File       | `rm`     | `del`       |

Points to Remember

1. Linux uses `/` for file paths.
2. Windows commonly uses `\` for file paths.
3. Linux commonly uses Bash.
4. Windows commonly uses PowerShell and CMD.
5. Both Linux and Windows support server administration.

## 5. Components of Linux – Shell & Kernel

### Linux Architecture

User

Shell (Bash / Zsh)

Command Interpretation

Linux Kernel

Process Management

Memory Management

Device Management

File System Management

Hardware

CPU / RAM / Disk / Network

### Kernel

1. Core component of the Linux operating system.
2. Manages CPU and memory.
3. Manages processes.
4. Controls hardware devices through drivers.
5. Provides file-system and networking services.

### Shell

1. Command interpreter.
2. Accepts commands from users.
3. Launches programs.
4. Supports shell scripting.
5. Common shells: Bash, Zsh, Sh, Fish.

### Kernel vs Shell

| Kernel                     | Shell                   |
| -------------------------- | ----------------------- |
| Core OS component          | Command interpreter     |
| Manages hardware resources | Processes user commands |
| Runs in kernel space       | Runs in user space      |
| Example: Linux kernel      | Example: Bash           |

### Practical Commands

```
# Check kernel name
uname

# Check kernel release
uname -r

# Check login shell
echo $SHELL

# Check current shell
echo $0
```

Points to Remember

- Kernel = Core of operating system.
- Shell = Command interpreter.
- Bash = Bourne Again Shell.
- Terminal = Interface for interacting with a shell.

## 6. AWS EC2 Login Demo

### AWS EC2 SSH Architecture

Local Laptop / Terminal

SSH – TCP Port 22

AWS Cloud

VPC / Public Subnet

Security Group

Allow TCP 22 from trusted IP

EC2 – Amazon Linux 2023

Public IPv4 / ec2-user

### EC2 Launch Configuration

| Setting        | Value                   |
| -------------- | ----------------------- |
| Service        | AWS EC2                 |
| Instance Name  | linux-training-server   |
| AMI            | Amazon Linux 2023       |
| Instance Type  | t3.micro                |
| Key Pair       | linux-key.pem           |
| Public IP      | Enabled                 |
| Security Group | SSH TCP 22 from your IP |
| Username       | ec2-user                |

### Steps to Launch EC2

1. Login to AWS Console.
2. Open EC2 → Instances.
3. Click Launch instances.
4. Enter instance name.
5. Select Amazon Linux 2023 AMI.
6. Select instance type.
7. Create or select key pair.
8. Configure security group and public IP.
9. Launch instance.
10. Copy public IPv4 address.

### SSH Login Commands

```
# Navigate to key location
cd ~/Downloads

# Secure private key
chmod 400 linux-key.pem

# Connect to EC2
ssh -i linux-key.pem ec2-user@<PUBLIC-IP>
```

Replace `<PUBLIC-IP>` with the actual public IPv4 address.

### Verify Login

```
whoami
hostname
pwd
uname -a
cat /etc/os-release
```

Points to Remember

1. SSH = Secure Shell.
2. Default SSH port = 22.
3. Amazon Linux default user = `ec2-user`.
4. `.pem` file = Private SSH key.
5. Restrict SSH access to trusted IPs.
6. Terminate unused EC2 lab instances to avoid charges.

## 7. Essential Linux Commands – pwd, ls, cd, whoami, uname

### 7.1 Command Summary

| Command  | Meaning                 | Purpose                           |
| -------- | ----------------------- | --------------------------------- |
| `pwd`    | Print Working Directory | Show current directory            |
| `ls`     | List                    | List files and directories        |
| `cd`     | Change Directory        | Navigate directories              |
| `whoami` | Who Am I                | Display effective username        |
| `uname`  | Unix Name               | Display system/kernel information |

### 7.2 pwd – Print Working Directory

```
pwd
```

Example output:

```
/home/ec2-user
```

### 7.3 ls – List Files and Directories

| Command  | Purpose                            |
| -------- | ---------------------------------- |
| `ls`     | List visible files                 |
| `ls -l`  | Detailed listing                   |
| `ls -a`  | Show hidden files                  |
| `ls -la` | Detailed listing with hidden files |
| `ls -lh` | Human-readable sizes               |
| `ls -lt` | Sort by modification time          |
| `ls -R`  | Recursive listing                  |

```
ls
ls -l
ls -a
ls -la
ls -lh
ls /etc
```

### 7.4 cd – Change Directory

| Command       | Purpose                   |
| ------------- | ------------------------- |
| `cd /`        | Go to root directory      |
| `cd ~`        | Go to home directory      |
| `cd ..`       | Go one directory up       |
| `cd -`        | Go to previous directory  |
| `cd /home`    | Go to home directory path |
| `cd /var/log` | Go to logs directory      |

```
pwd
cd /
pwd
cd /home
pwd
cd ~
pwd
cd /var/log
pwd
cd ..
pwd
cd -
```

### 7.5 whoami – Current User

```
whoami
```

Example output:

```
ec2-user
```

### 7.6 uname – System Information

| Command    | Purpose                          |
| ---------- | -------------------------------- |
| `uname`    | Kernel name                      |
| `uname -a` | All available system information |
| `uname -r` | Kernel release                   |
| `uname -m` | Machine architecture             |
| `uname -s` | Kernel name                      |
| `uname -n` | Network node hostname            |

```
uname
uname -a
uname -r
uname -m
```

Points to Remember

1. `pwd` – Current directory.
2. `ls` – List files.
3. `ls -la` – Include hidden files.
4. `cd ..` – Parent directory.
5. `cd ~` – Home directory.
6. `whoami` – Effective username.
7. `uname -r` – Kernel release.
8. `uname -m` – Machine architecture.

## 8. Hands-on Practice – Day 1

```
# 1. Check current user
whoami

# 2. Check current directory
pwd

# 3. List files
ls

# 4. List hidden files
ls -la

# 5. Check kernel
uname -a

# 6. Check kernel release
uname -r

# 7. Check architecture
uname -m

# 8. Check Linux distribution
cat /etc/os-release

# 9. Go to root directory
cd /

# 10. List root directories
ls

# 11. Go to home
cd /home

# 12. Go to current user's home
cd ~

# 13. Go to logs
cd /var/log

# 14. List log files
ls -lh

# 15. Return to previous directory
cd -
```

## 9. Day 1 Assignment

1. Define Linux Operating System.
2. List any five features of Linux.
3. List ten Linux distributions.
4. Explain Debian and Red Hat Linux families.
5. Write five differences between Linux and Windows.
6. Draw Linux Kernel and Shell architecture.
7. Launch Amazon Linux 2023 EC2 instance.
8. Connect to EC2 using SSH.
9. Execute `pwd`, `ls`, `cd`, `whoami`, `uname`.
10. Submit screenshots of executed commands.

## 10. Quick Revision – Important Points

| Topic             | Key Point                       |
| ----------------- | ------------------------------- |
| Linux Creator     | Linus Torvalds                  |
| Linux Year        | 1991                            |
| Linux             | Open-source Unix-like OS family |
| Kernel            | Core of operating system        |
| Shell             | Command interpreter             |
| Bash              | Bourne Again Shell              |
| Ubuntu            | Debian-based distribution       |
| RHEL              | Enterprise Linux                |
| Amazon Linux 2023 | AWS-focused distribution        |
| SSH               | Secure Shell                    |
| SSH Port          | 22                              |
| Default EC2 User  | ec2-user                        |
| `pwd`             | Current directory               |
| `ls`              | List files                      |
| `cd`              | Change directory                |
| `whoami`          | Current effective username      |
| `uname -r`        | Kernel release                  |
