# Linux Cheat Sheet

# 🐧 Linux Commands Cheat Sheet

## 📂 Navigation
- `pwd` – Print working directory  
- `ls` – List files and directories  
- `cd` – Change directory  
- `tree` – Show directory structure  
- `history` – Command history  

---

## 📁 Files (File Management Basics)
- `touch` – Create a new file  
- `cp` – Copy files/directories  
- `mv` – Move/rename files  
- `rm` – Remove files/directories  
- `mkdir` – Create directories  

---

## 📄 View Files
- `cat` – Display file content  
- `less` – View file (scrollable)  
- `more` – View file (paged)  
- `head` – First lines of file  
- `tail` – Last lines of file  

---

## 🔍 Search
- `grep` – Search text in files  
- `find` – Search files/directories  
- `locate` – Quickly find files  
- `which` – Show command path  
- `whereis` – Locate binary/source  

---

## 🔐 Permissions
- `chmod` – Change file permissions  
- `chown` – Change file owner  
- `chgrp` – Change group ownership  

---

## 📊 System Monitoring
- `top` – Real-time processes  
- `htop` – Interactive process viewer  
- `df` – Disk space usage  
- `du` – Directory size  
- `free` – Memory usage  
- `uptime` – System uptime  

---

## ⚙️ Process Management
- `ps` – Show running processes  
- `kill` – Kill process by PID  
- `killall` – Kill by name  
- `bg` – Run process in background  
- `fg` – Bring process to foreground  

---

## 🌐 Network
- `ping` – Check connectivity  
- `curl` – Transfer data from URL  
- `wget` – Download files  
- `netstat` – Network stats  
- `ss` – Socket statistics  

---

## 📦 Archive
- `tar` – Archive files  
- `zip` – Compress files  
- `unzip` – Extract zip files  

---

## 💾 Disk & Storage
- `mount` – Mount filesystem  
- `umount` – Unmount filesystem  
- `lsblk` – List block devices  

---

## 👤 Users
- `whoami` – Current user  
- `id` – User ID info  
- `useradd` – Add new user  

---

## 📜 Package & Logs (DevOps Foundation)
- `apt` – Package manager (Debian/Ubuntu)  
- `yum` – Package manager (RHEL/CentOS)  
- `journalctl` – View system logs  

---

# 🔐 Linux File Permissions Cheat Sheet

## 📊 Permission Types

| Symbol | Meaning        | Value |
|--------|---------------|-------|
| r      | Read          | 4     |
| w      | Write         | 2     |
| x      | Execute       | 1     |
| -      | No permission | 0     |

---

## 👥 User Types

| Symbol | User Type |
|--------|----------|
| u      | User (Owner) |
| g      | Group |
| o      | Others |

---

## 📁 Permission Structure

Example: `-rwxr-xr--`

| Position | Meaning |
|----------|--------|
| 1        | File type (`-` file, `d` directory) |
| 2-4      | User (Owner) permissions |
| 5-7      | Group permissions |
| 8-10     | Others permissions |

---

## 🔢 Numeric (Octal) Permissions

| Number | Permission | Meaning |
|--------|------------|--------|
| 7      | rwx        | Full access |
| 6      | rw-        | Read + Write |
| 5      | r-x        | Read + Execute |
| 4      | r--        | Read only |
| 3      | -wx        | Write + Execute |
| 2      | -w-        | Write only |
| 1      | --x        | Execute only |
| 0      | ---        | No access |

---

## 📌 Common Permission Examples

| Command            | Meaning |
|--------------------|--------|
| `chmod 777 file`   | Full access to everyone |
| `chmod 755 file`   | Owner full, others read + execute |
| `chmod 644 file`   | Owner read/write, others read |
| `chmod 700 file`   | Only owner has full access |

---

## ⚙️ Symbolic Mode (chmod)

| Command                  | Meaning |
|--------------------------|--------|
| `chmod u+x file`         | Add execute to user |
| `chmod g-w file`         | Remove write from group |
| `chmod o+r file`         | Add read to others |
| `chmod u=rwx,g=rx,o=r`   | Set exact permissions |

---

## 📂 Special Permissions

| Permission | Symbol | Numeric | Description |
|------------|--------|--------|------------|
| SUID       | s      | 4xxx   | Run as file owner |
| SGID       | s      | 2xxx   | Run as group |
| Sticky Bit | t      | 1xxx   | Only owner can delete |

Example:
```bash
chmod 4755 file   # SUID
chmod 2755 dir    # SGID
chmod 1755 dir    # Sticky Bit