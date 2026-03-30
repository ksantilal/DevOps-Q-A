# 🐧 Linux Commands Cheat Sheet

---

## 📁 File & Directory Commands

| Command | Description | Example |
|--------|------------|--------|
| `ls` | List files/directories | `ls` |
| `ls -l` | Detailed list | `ls -l` |
| `ls -la` | Show hidden files | `ls -la` |
| `ls -lart` | Sorted by time | `ls -lart` |
| `cd` | Change directory | `cd /home` |
| `pwd` | Show current directory | `pwd` |
| `mkdir` | Create directory | `mkdir test` |
| `rm` | Delete file/directory | `rm file.txt` |
| `rm -r` | Delete directory | `rm -r folder` |
| `cp` | Copy files | `cp file1 file2` |
| `mv` | Move/rename files | `mv old new` |

---

## 📄 File Content Commands

| Command | Description | Example |
|--------|------------|--------|
| `cat` | View file content | `cat file.txt` |
| `echo` | Print text/variable | `echo "Hello"` |
| `grep` | Search pattern | `grep "error" file.txt` |
| `find` | Find files | `find / -name file.txt` |

---

## 👤 User & Permission Commands

| Command | Description | Example |
|--------|------------|--------|
| `whoami` | Show current user | `whoami` |
| `chmod` | Change permissions | `chmod 755 file` |
| `chown` | Change ownership | `chown user file` |

---

## ⚙️ Process Management

| Command | Description | Example |
|--------|------------|--------|
| `ps` | Show running processes | `ps aux` |
| `top` | Real-time processes | `top` |
| `kill` | Kill process by PID | `kill 1234` |

---

## 💾 Disk & Memory

| Command | Description | Example |
|--------|------------|--------|
| `df` | Disk usage | `df -h` |
| `du` | Directory size | `du -h` |
| `free` | Memory usage | `free -h` |

---

## 🖥️ System Info

| Command | Description | Example |
|--------|------------|--------|
| `uptime` | System running time | `uptime` |
| `uname -a` | System details | `uname -a` |

---

## 🌐 Network Commands

| Command | Description | Example |
|--------|------------|--------|
| `ifconfig` | Network config | `ifconfig` |
| `netstat` | Network stats | `netstat -tuln` |
| `ssh` | Remote login | `ssh user@ip` |
| `scp` | Copy files remotely | `scp file user@ip:/path` |
| `rsync` | Sync files | `rsync -av file dest` |

---

## 📦 Archive & Download

| Command | Description | Example |
|--------|------------|--------|
| `tar` | Archive files | `tar -cvf file.tar dir/` |
| `wget` | Download files | `wget url` |
| `curl` | Transfer data | `curl url` |

---

## 🔧 Environment Variables

| Command | Description | Example |
|--------|------------|--------|
| `env` | Show variables | `env` |
| `export` | Set variable | `export VAR=value` |
| `source` | Run script | `source file.sh` |
| `alias` | Shortcut command | `alias ll='ls -l'` |

---

## ⏰ Scheduling

| Command | Description | Example |
|--------|------------|--------|
| `crontab -e` | Edit cron jobs | `crontab -e` |

---

## 🔥 Service Management

| Command | Description | Example |
|--------|------------|--------|
| `systemctl` | Manage services | `systemctl start nginx` |
| `journalctl` | View logs | `journalctl -u nginx` |

---

## ✍️ Editors

| Editor | Command |
|-------|--------|
| `vi` / `vim` | `vi file.txt` |
| `nano` | `nano file.txt` |

### 🔹 VI Editor Shortcuts
- `Esc + :wq` → Save & exit  
- `Esc + :q!` → Exit without saving  

---

## 📜 History

| Command | Description |
|--------|------------|
| `history` | Show previous commands |

---

## 🎯 Quick Commands (Important)

```bash
free -h   # Memory usage (human readable)
df -h     # Disk usage
du -h     # Folder size