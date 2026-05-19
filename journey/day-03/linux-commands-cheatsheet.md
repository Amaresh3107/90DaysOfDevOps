# Linux Commands Cheat Sheet

A quick reference guide for daily Linux troubleshooting and DevOps work.

---

# 1. File System Commands

| Command | Usage |
|---------|--------|
| `pwd` | Show current directory |
| `ls -la` | List all files with permissions |
| `cd <dir>` | Change directory |
| `mkdir <name>` | Create new directory |
| `touch <file>` | Create empty file |
| `cp <src> <dest>` | Copy files/folders |
| `mv <src> <dest>` | Move or rename files |
| `rm -rf <name>` | Delete files/folders forcefully |
| `find / -name file.txt` | Search for a file |
| `du -sh *` | Check folder sizes |
| `df -h` | Show disk space usage |
| `cat <file>` | View file contents |
| `less <file>` | Read large files page by page |
| `head -n 10 <file>` | Show first 10 lines |
| `tail -f <file>` | Watch logs in real time |

---

# 2. Process Management Commands

| Command | Usage |
|---------|--------|
| `ps aux` | Show running processes |
| `top` | Live system monitoring |
| `htop` | Better interactive process viewer |
| `kill <PID>` | Stop a process by PID |
| `pkill <name>` | Kill process by name |
| `jobs` | Show background jobs |
| `bg` | Run job in background |
| `fg` | Bring job to foreground |
| `free -h` | Show memory usage |
| `uptime` | Show system uptime/load |

---

# 3. Networking Commands

| Command | Usage |
|---------|--------|
| `ping google.com` | Test internet connectivity |
| `ip addr` | Show IP addresses |
| `curl https://example.com` | Test HTTP request |
| `dig google.com` | DNS lookup |
| `netstat -tulnp` | Show listening ports |
| `ss -tulnp` | Modern alternative to netstat |
| `traceroute google.com` | Trace network path |
| `wget <url>` | Download files from internet |

---

# 4. Permissions & User Commands

| Command | Usage |
|---------|--------|
| `chmod 755 <file>` | Change file permissions |
| `chown user:user <file>` | Change file ownership |
| `whoami` | Show current user |
| `id` | Show user/group IDs |
| `sudo <command>` | Run command as admin |

---

# 5. System & Service Commands

| Command | Usage |
|---------|--------|
| `uname -a` | Show system information |
| `hostname` | Show system hostname |
| `systemctl status nginx` | Check service status |
| `systemctl start nginx` | Start service |
| `systemctl stop nginx` | Stop service |
| `journalctl -xe` | View system logs |

---

# Common DevOps Troubleshooting Flow

## Check System Health
```bash
top
free -h
df -h
uptime