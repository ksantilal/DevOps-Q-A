# Ansible Cheat Sheet

## 📁 Inventory
- `ansible all -i hosts -m ping` → Test connectivity

## ⚡ Ad-hoc Commands
- `ansible all -m command -a "uptime"` → Run command
- `ansible web -m service -a "name=nginx state=started"` → Manage service

## 📜 Playbooks
- `ansible-playbook playbook.yml` → Run playbook

## 🔧 Variables
- `ansible-playbook playbook.yml -e "var=value"` → Pass variable

## 📊 Facts
- `ansible all -m setup` → Gather system info

## 📦 Roles
- `ansible-galaxy init role` → Create role