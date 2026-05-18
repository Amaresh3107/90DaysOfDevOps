# Day 02 - Linux Architecture, Processes & systemd

## What is Linux?

Linux is an operating system used in most servers, cloud platforms, and production systems.

It helps the computer:
- Run applications
- Manage hardware
- Handle memory and files
- Run multiple tasks together

Linux is very important in DevOps because most production servers run on Linux.

---

# Core Components of Linux

## 1. Kernel

Kernel is the heart of Linux.

It directly communicates with the hardware and manages:
- CPU
- Memory
- Devices
- Processes
- File systems

Example:
When we open Chrome, Docker, or VS Code, the kernel helps them use system resources.

---

## 2. User Space

User space is the area where users and applications run.

Applications cannot directly access hardware.  
They request help from the kernel.

Examples:
- Terminal
- Browser
- VS Code
- Docker

---

## 3. Init / systemd

systemd is the first process started by Linux after booting.

Its Process ID (PID) is `1`.

systemd is responsible for:
- Starting services
- Stopping services
- Restarting failed services
- Managing background processes
- Handling system boot process

Examples of services:
- nginx
- docker
- ssh

---

# What is a Process?

A process is simply a running program.

Examples:
- Opening Spotify creates a process
- Running `python app.py` creates a process

Every process in Linux gets a unique ID called PID (Process ID).

---

# How Processes are Created

Linux creates processes like this:

1. Parent process creates a child process
2. Linux assigns a PID
3. Process starts running

Example:
Opening terminal starts a bash process.

---

# Process States in Linux

## Running
Process is actively using CPU.

## Sleeping
Process is waiting for input or resources.

## Stopped
Process is paused manually.

## Zombie
Process finished execution but still exists in process table.

## Orphan
Parent process is terminated before child process.

---

# What is systemd?

systemd is a service manager in Linux.

It helps Linux:
- Start services during boot
- Monitor services
- Restart crashed services
- Manage logs and background services

systemd is important because almost every modern Linux server uses it.

---

# Useful systemd Commands

## Check service status

```bash
systemctl status nginx
```

## Start a service

```bash
systemctl start nginx
```

## Stop a service

```bash
systemctl stop nginx
```

## Restart a service

```bash
systemctl restart nginx
```

## Enable service after reboot

```bash
systemctl enable nginx
```

---

# 5 Linux Commands I Will Use Daily

## View running processes

```bash
ps aux
```

## Monitor CPU and memory usage

```bash
top
```

## Better interactive process viewer

```bash
htop
```

## Manage Linux services

```bash
systemctl
```

## View system and service logs

```bash
journalctl
```

---

# Why This Matters for DevOps

Understanding Linux helps in:
- Troubleshooting servers
- Fixing crashed applications
- Managing services confidently
- Monitoring CPU and memory
- Reading logs during incidents

Linux is the foundation of most production systems, so learning these basics is very important for a DevOps Engineer.