# ⚙️ Ansible Interview Questions & Answers (DevOps)

---

# 🔹 BASIC ANSIBLE QUESTIONS

## 1. What is Ansible?
Ansible is an automation tool used for configuration management, application deployment, and task automation.

---

## 2. Who developed Ansible?
Red Hat

---

## 3. Why use Ansible?
- Agentless
- Simple YAML syntax
- Easy automation

---

## 4. What is agentless?
No software needed on target machines, uses SSH.

---

## 5. What is Ansible architecture?
- Control node (where Ansible runs)
- Managed nodes (servers)

---

## 6. What is inventory?
List of target servers.

---

## 7. What is module?
Reusable unit that performs tasks.

---

## 8. What is playbook?
YAML file with automation tasks.

---

## 9. What is task?
Single action in playbook.

---

## 10. What is role?
Reusable structure for playbooks.

---

# 🔹 INVENTORY & VARIABLES

## 11. Types of inventory?
- Static
- Dynamic

---

## 12. What is host group?
Group of servers in inventory.

---

## 13. What is variable?
Used to store values.

---

## 14. Types of variables?
- host vars
- group vars
- extra vars

---

## 15. How to pass variables?
ansible-playbook playbook.yml -e "key=value"

---

## 16. What is fact?
System info collected automatically.

---

## 17. What is register?
Store output of task.

---

## 18. What is condition?
Run tasks based on condition (when).

---

## 19. What is loop?
Repeat tasks.

---

## 20. What is template?
Dynamic file using Jinja2.

---

# 🔹 PLAYBOOKS

## 21. Structure of playbook?
- hosts
- tasks
- vars

---

## 22. Example playbook
- hosts: web
  tasks:
    - name: install nginx
      apt:
        name: nginx
        state: present

---

## 23. What is idempotency?
Running playbook multiple times gives same result.

---

## 24. What is handler?
Triggered task (e.g., restart service).

---

## 25. What is notify?
Triggers handler.

---

# 🔹 MODULES

## 26. Common modules?
- apt / yum
- service
- copy
- file

---

## 27. What is command module?
Run shell commands.

---

## 28. Difference between command and shell?
- command = safer
- shell = supports pipes

---

## 29. What is file module?
Manage files.

---

## 30. What is copy module?
Copy files to remote server.

---

# 🔹 ROLES

## 31. What is role structure?
roles/
  tasks/
  handlers/
  templates/
  vars/

---

## 32. Why use roles?
- Reusability
- Clean structure

---

## 33. What is Ansible Galaxy?
Repository of roles.

---

## 34. Command
ansible-galaxy init role_name

---

## 35. How to use role?
Include in playbook.

---

# 🔹 ADVANCED QUESTIONS

## 36. What is vault?
Encrypt sensitive data.

---

## 37. What is become?
Run tasks as root.

---

## 38. What is tags?
Run specific tasks.

---

## 39. What is delegate_to?
Run task on another host.

---

## 40. What is async?
Run tasks asynchronously.

---

## 41. What is serial?
Run tasks in batches.

---

## 42. What is strategy?
Control execution (linear, free).

---

## 43. What is callback plugin?
Custom output format.

---

## 44. What is dynamic inventory?
Fetch hosts from cloud.

---

## 45. What is connection type?
SSH, local, etc.

---

# 🔹 DEVOPS USAGE

## 46. Ansible vs Terraform?
- Ansible = config
- Terraform = infra

---

## 47. Ansible vs Chef/Puppet?
- Simpler
- Agentless

---

## 48. Ansible in CI/CD?
Used for deployment automation.

---

## 49. Ansible with Docker?
Used to configure containers.

---

## 50. Ansible with Kubernetes?
Manage cluster setup.

---

# 🧪 REAL-TIME SCENARIOS

## 51. Playbook failed?
Check logs and fix errors.

---

## 52. Task not running?
Check conditions or tags.

---

## 53. SSH issue?
Check connectivity and keys.

---

## 54. Variable not working?
Check scope and syntax.

---

## 55. Sensitive data?
Use Ansible Vault.

---

## 56. Multiple environments?
Use group_vars.

---

## 57. Large deployment?
Use roles and modular structure.

---

## 58. Slow execution?
Use parallel execution.

---

## 59. Service not restarting?
Check handler.

---

## 60. Debug issue?
Use -vvv for verbose output.

---