# 🐧 Linux Interview Questions & Answers (DevOps)

---

# 🔹 BASIC LINUX QUESTIONS

## 1. What is Linux?
Linux is an open-source operating system used for servers, cloud, and DevOps environments.

---

## 2. What is a kernel?
The kernel is the core of Linux that manages hardware and system resources.

---

## 3. What is a shell?
A shell is a command-line interface to interact with the system.

Examples: bash, sh, zsh

---

## 4. What is the root user?
The root user has full administrative access.

---

## 5. What is a file system?
Structure used to store and organize files.

---

## 6. What is a process?
A running program.

---

## 7. What is PID?
Process ID — unique number for each process.

---

## 8. What is a directory?
A folder that contains files.

---

## 9. What is absolute vs relative path?
- Absolute: `/home/user/file`
- Relative: `../file`

---

## 10. What is sudo?
Allows normal user to run admin commands.

---

# 🔹 COMMAND QUESTIONS

## 11. List files
ls -la → list all files with details

---

## 12. Change directory
cd /path → move to directory

---

## 13. Create file
touch file.txt

---

## 14. Delete file
rm file.txt

---

## 15. Copy file
cp file1 file2

---

## 16. Move file
mv file1 file2

---

## 17. View file
cat file

---

## 18. Search text
grep "text" file

---

## 19. Find file
find / -name file.txt

---

## 20. Check disk usage
df -h

---

# 🔹 PERMISSIONS & USERS

## 21. What are file permissions?
Control access (read, write, execute).

---

## 22. What is chmod?
Change permissions.

Example:
chmod 755 file

---

## 23. What is chown?
Change ownership.

---

## 24. What are user types?
- Root
- Normal user
- Service user

---

## 25. Add user
useradd username

---

## 26. Switch user
su username

---

# 🔹 PROCESS MANAGEMENT

## 27. View processes
ps aux

---

## 28. Real-time processes
top / htop

---

## 29. Kill process
kill PID

---

## 30. Kill force
kill -9 PID

---

## 31. Background process
command &

---

## 32. What is daemon?
Background service process.

---

# 🔹 NETWORKING

## 33. Check IP
ip a

---

## 34. Ping server
ping google.com

---

## 35. Check ports
netstat -tuln

---

## 36. Curl
curl url → test API

---

## 37. SSH
ssh user@host → remote login

---

# 🔹 PACKAGE MANAGEMENT

## 38. Install package
apt install nginx

---

## 39. Remove package
apt remove nginx

---

## 40. Update system
apt update && apt upgrade

---

# 🔹 LOGS & MONITORING

## 41. View logs
tail -f /var/log/syslog

---

## 42. What is log rotation?
Managing log file size automatically.

---

## 43. Check memory
free -m

---

## 44. Check CPU
top

---

# 🔹 ADVANCED DEVOPS QUESTIONS

## 45. What is cron job?
Scheduled task.

Example:
crontab -e

---

## 46. What is systemctl?
Manage services.

Example:
systemctl start nginx

---

## 47. What is environment variable?
Key-value pair used by system/apps.

---

## 48. What is soft vs hard link?
- Soft link = shortcut
- Hard link = actual file reference

---

## 49. What is swap memory?
Extra memory using disk.

---

## 50. What is inode?
Metadata of a file.

---

# 🧪 REAL-TIME SCENARIO QUESTIONS

## 51. Disk is full, what will you do?
- Check: df -h
- Find large files: du -sh *
- Clean logs

---

## 52. Server is slow?
- Check CPU: top
- Check memory: free -m
- Check logs

---

## 53. Service not starting?
- Check status: systemctl status
- Check logs

---

## 54. Port not accessible?
- Check firewall
- Check service running
- Check port: netstat

---

## 55. High memory usage?
- Identify process
- Restart or optimize

---

## 56. Cannot SSH into server?
- Check network
- Check SSH service
- Check firewall

---

## 57. File permission issue?
- Fix using chmod/chown

---

## 58. Process stuck?
- kill or restart

---

## 59. Application logs not generating?
- Check log path
- Check permissions

---

## 60. Debug production issue?
- Logs → Metrics → Restart → Fix

---

# 🎯 BEST PRACTICES

- Use least privilege (security)
- Monitor system regularly
- Automate tasks using scripts
- Keep backups

---
