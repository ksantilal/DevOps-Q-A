# Linux Cheat Sheet

## 📁 File & Directory Commands
- `ls -la` → List all files (including hidden) with details
- `pwd` → Show current directory
- `cd /path` → Change directory
- `mkdir dir` → Create directory
- `rm -rf file/dir` → Delete file or directory recursively
- `cp src dest` → Copy files/directories
- `mv src dest` → Move or rename files

## 📖 File Viewing
- `cat file` → Display file content
- `less file` → View file interactively (scrollable)
- `head -n 10 file` → First 10 lines
- `tail -f file` → Live file updates (logs)

## 🔐 Permissions
- `chmod +x file` → Make file executable
- `chown user:group file` → Change ownership

## 🔍 Search
- `find . -name file.txt` → Find file by name
- `grep "text" file` → Search text inside file

## 📊 System Monitoring
- `top` → Real-time processes
- `htop` → Better UI version of top
- `df -h` → Disk usage
- `free -m` → Memory usage

## 🌐 Networking
- `ping host` → Check connectivity
- `curl url` → Fetch data from URL
- `wget url` → Download file