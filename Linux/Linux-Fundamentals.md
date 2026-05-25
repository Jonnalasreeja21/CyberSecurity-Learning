# Linux Fundamentals for Freshers

## Introduction

Linux is a free and open-source operating system that is widely used in servers, cloud computing, cybersecurity, software development, and networking. It was created by Linus Torvalds in 1991 and has become one of the most important technologies in the IT industry.

Unlike proprietary operating systems, Linux allows users to view, modify, and distribute its source code freely.

---

# What is an Operating System?

An Operating System (OS) is software that acts as a bridge between the user and computer hardware.

Responsibilities of an Operating System:

- Managing files and folders
- Running applications
- Managing memory
- Handling hardware devices
- Providing security
- Managing users

Examples:

- Windows
- macOS
- Linux
- Android

---

# Why Learn Linux?

Linux is a critical skill for IT and cybersecurity professionals because most servers and cloud platforms run Linux.

Benefits:

- Open Source
- Free to use
- Highly secure
- Fast performance
- Stable and reliable
- Powerful command-line interface

Industries using Linux:

- Cybersecurity
- Cloud Computing
- Networking
- DevOps
- Software Development
- Data Centers

---

# Linux in Real World

Many popular services run on Linux:

- Google
- Facebook
- Amazon
- Netflix
- YouTube

Cloud Platforms:

- AWS
- Microsoft Azure
- Google Cloud Platform

Cybersecurity Platforms:

- Kali Linux
- Parrot OS

---

# Linux Distributions (Distros)

A Linux distribution is a version of Linux that includes the Linux kernel, utilities, package manager, and desktop environment.

## Popular Linux Distributions

### Ubuntu

- Beginner-friendly
- Large community support
- Popular for development

### Kali Linux

- Designed for cybersecurity
- Includes penetration testing tools
- Used by ethical hackers

### Debian

- Extremely stable
- Commonly used for servers

### Fedora

- Cutting-edge features
- Popular among developers

### Parrot OS

- Security and privacy focused
- Used for penetration testing

---

# Linux Architecture

Linux consists of several layers:

## Hardware

Physical components:

- CPU
- RAM
- Hard Disk
- Network Card

## Kernel

The core component of Linux.

Functions:

- Memory Management
- Process Management
- Device Management
- Security Management

## Shell

Acts as an interface between the user and kernel.

Examples:

- Bash
- Zsh
- Sh

## Applications

Programs used by users.

Examples:

- Firefox
- VS Code
- Wireshark

---

# GUI vs CLI

## GUI (Graphical User Interface)

Uses:

- Mouse
- Icons
- Windows

Advantages:

- Easy to learn
- User-friendly

Example:

Ubuntu Desktop

---

## CLI (Command Line Interface)

Uses text commands.

Advantages:

- Faster
- Powerful
- Automation support
- Preferred by cybersecurity professionals

Example:

```bash
ls
pwd
cd
```

---

# Linux File System

Linux uses a hierarchical file structure.

Top-level directory:

```bash
/
```

This is called the Root Directory.

Everything in Linux starts from the root directory.

---

# Important Linux Directories

## /home

Stores user files.

Example:

```bash
/home/sreeja
```

---

## /root

Home directory of the root user.

---

## /etc

Stores system configuration files.

Example:

```bash
/etc/passwd
```

---

## /bin

Contains essential system commands.

Examples:

```bash
ls
cp
mv
```

---

## /var

Stores logs and variable data.

---

## /tmp

Stores temporary files.

---

# Linux Users

Linux supports multiple users.

Types:

## Normal User

Limited permissions.

Used for everyday tasks.

## Root User

Administrator account.

Has full control over the system.

Example:

```bash
sudo apt update
```

---

# Understanding sudo

sudo means:

```text
Super User Do
```

Allows a normal user to execute commands with administrative privileges.

Example:

```bash
sudo apt install nmap
```

---

# Basic Linux Commands

## pwd

Print Working Directory.

Displays current location.

```bash
pwd
```

Output:

```bash
/home/sreeja
```

---

## ls

Lists files and folders.

```bash
ls
```

Detailed view:

```bash
ls -l
```

---

## cd

Changes directory.

```bash
cd Documents
```

Go back:

```bash
cd ..
```

---

## mkdir

Creates a directory.

```bash
mkdir CyberLab
```

---

## touch

Creates an empty file.

```bash
touch notes.txt
```

---

## rm

Removes a file.

```bash
rm notes.txt
```

---

## cp

Copies files.

```bash
cp source.txt backup.txt
```

---

## mv

Moves or renames files.

Rename:

```bash
mv old.txt new.txt
```

Move:

```bash
mv file.txt Documents/
```

---

# File Permissions

Linux protects files using permissions.

Example:

```bash
-rw-r--r--
```

Meaning:

Owner:
- Read
- Write

Group:
- Read

Others:
- Read

Permission Types:

| Symbol | Meaning |
|----------|----------|
| r | Read |
| w | Write |
| x | Execute |

---

# Networking Commands

## ping

Checks connectivity.

```bash
ping google.com
```

---

## ip a

Displays IP address information.

```bash
ip a
```

---

## ifconfig

Shows network interfaces.

```bash
ifconfig
```

---

## netstat

Displays network connections.

```bash
netstat
```

---

# Package Management

Package managers help install software.

Ubuntu:

```bash
sudo apt update
sudo apt install nmap
```

Fedora:

```bash
sudo dnf install nmap
```

Arch:

```bash
sudo pacman -S nmap
```

---

# Process Management

A process is a running program.

Useful commands:

## ps

Shows active processes.

```bash
ps
```

## top

Displays system resource usage.

```bash
top
```

## kill

Terminates a process.

```bash
kill PID
```

---

# Environment Variables

Store system information.

Display home directory:

```bash
echo $HOME
```

Display username:

```bash
echo $USER
```

---

# Linux Security Features

Linux provides:

- User authentication
- File permissions
- Firewalls
- Encryption
- Access controls

Firewall status:

```bash
ufw status
```

---

# Linux in Cybersecurity

Linux is the preferred operating system for cybersecurity because:

- Open Source
- Powerful networking tools
- Script automation
- Security-focused distributions

Popular Security Tools:

- Nmap
- Wireshark
- Metasploit
- Burp Suite
- John the Ripper

---

# Beginner Practice Lab

Create a Cyber Lab:

```bash
mkdir CyberLab
cd CyberLab

mkdir logs
mkdir reports
mkdir tools

touch notes.txt

ls -l
```

Expected Output:

```bash
logs
reports
tools
notes.txt
```

---

# Career Opportunities

Linux knowledge is essential for:

- Cybersecurity Analyst
- SOC Analyst
- Ethical Hacker
- Security Engineer
- DevOps Engineer
- Cloud Engineer
- System Administrator
- Network Engineer

---

# Key Takeaways

- Linux is a powerful open-source operating system.
- Most servers and cloud systems use Linux.
- The command line is an essential skill.
- Linux security features make it ideal for cybersecurity.
- Understanding files, users, permissions, networking, and processes is fundamental.
- Linux is a must-have skill for IT, cloud, DevOps, and cybersecurity careers.

---

# Learning Progress

- [x] Linux Fundamentals
- [ ] Linux File Permissions
- [ ] Bash Scripting
- [ ] Process Management
- [ ] Networking Commands
- [ ] User Management
- [ ] Linux Security
