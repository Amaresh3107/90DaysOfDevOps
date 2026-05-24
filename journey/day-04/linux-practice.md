# Day 04 – Linux Practice: Processes and Services

## Process Checks

### ps -ef
Displays all currently running processes in the system.

### top
Shows real-time CPU, memory usage, and active processes.

---

## Service Checks

### systemctl status ssh
Checks whether the SSH service is active, inactive, or failed.

### systemctl list-units --type=service
Lists all active systemd services running on the system.

---

## Log Checks

### journalctl -u ssh
Displays logs related to the SSH service.

### tail -n 50 /var/log/syslog
Shows the latest 50 lines from the system log file.

---

## Mini Troubleshooting Steps

### systemctl status ssh
Verified whether the SSH service was running properly.

### journalctl -u ssh
Checked SSH logs for errors or warnings.

### ps -ef | grep ssh
Verified that the SSH process was running in the background.