# 🏗️ Terraform Interview Questions & Answers (DevOps)

---

# 🔹 BASIC TERRAFORM QUESTIONS

## 1. What is Terraform?
Terraform is a tool used to create and manage infrastructure using code.

---

## 2. What is Infrastructure as Code (IaC)?
Managing infrastructure (servers, networks) using code instead of manual setup.

---

## 3. Who created Terraform?
HashiCorp

---

## 4. What is a provider?
A plugin that allows Terraform to interact with APIs (AWS, Azure, GCP).

---

## 5. What is a resource?
A component of infrastructure (EC2, S3, VM).

---

## 6. What is a Terraform configuration?
A set of `.tf` files defining infrastructure.

---

## 7. What is Terraform CLI?
Command-line tool to run Terraform commands.

---

## 8. What is `terraform init`?
Initializes project and downloads providers.

---

## 9. What is `terraform plan`?
Shows changes before applying.

---

## 10. What is `terraform apply`?
Creates or updates infrastructure.

---

# 🔹 CORE CONCEPTS

## 11. What is state file?
File that stores current infrastructure state.

---

## 12. Why is state important?
Tracks resources and prevents duplication.

---

## 13. What is desired state?
The configuration you define in code.

---

## 14. What is actual state?
Real infrastructure in cloud.

---

## 15. What is drift?
Difference between desired and actual state.

---

## 16. What is `terraform destroy`?
Deletes all resources.

---

## 17. What is dependency in Terraform?
Order of resource creation.

---

## 18. What is output?
Value returned after apply.

---

## 19. What is variable?
Input value for configuration.

---

## 20. What is locals?
Reusable internal variables.

---

# 🔹 VARIABLES & FILES

## 21. Types of variables?
- string
- number
- bool
- list
- map

---

## 22. What is `terraform.tfvars`?
File to define variable values.

---

## 23. How to pass variables?
terraform apply -var="name=value"

---

## 24. What is sensitive variable?
Hidden value (passwords).

---

## 25. What is interpolation?
Using variables in code.

Example:
${var.name}

---

# 🔹 STATE MANAGEMENT

## 26. What is remote state?
State stored remotely (S3, Azure Blob).

---

## 27. Why use remote state?
- Team collaboration
- Backup
- Locking

---

## 28. What is state locking?
Prevent multiple users from modifying state.

---

## 29. What is `terraform state` command?
Manage state manually.

---

## 30. What is state file risk?
Sensitive data exposure.

---

# 🔹 MODULES

## 31. What is module?
Reusable Terraform code.

---

## 32. Types of modules?
- Root module
- Child module

---

## 33. Why use modules?
- Reusability
- Clean code

---

## 34. What is module registry?
Collection of reusable modules.

---

## 35. How to call module?
module "name" { source = "..." }

---

# 🔹 ADVANCED TERRAFORM QUESTIONS

## 36. What is provisioner?
Run scripts after resource creation.

---

## 37. Types of provisioners?
- local-exec
- remote-exec

---

## 38. What is backend?
Where state is stored.

---

## 39. What is workspace?
Separate environments (dev, prod).

---

## 40. What is lifecycle?
Control resource behavior.

---

## 41. What is `count`?
Create multiple resources.

---

## 42. What is `for_each`?
Loop over resources.

---

## 43. Difference between count and for_each?
- count = index-based
- for_each = key-based

---

## 44. What is data source?
Fetch existing resources.

---

## 45. What is import?
Bring existing infra into Terraform.

---

# 🔹 CLOUD & DEVOPS USAGE

## 46. Terraform with AWS?
Used to create EC2, S3, VPC.

---

## 47. Terraform with CI/CD?
Used in pipelines for automation.

---

## 48. Terraform vs CloudFormation?
- Terraform = multi-cloud
- CloudFormation = AWS only

---

## 49. Terraform vs Ansible?
- Terraform = provisioning
- Ansible = configuration

---

## 50. Terraform workflow?
init → plan → apply → destroy

---

# 🧪 REAL-TIME SCENARIOS

## 51. Infrastructure not updating?
Check plan and state file.

---

## 52. State file corrupted?
Restore from backup.

---

## 53. Multiple users working?
Use remote state with locking.

---

## 54. Resource already exists?
Use import.

---

## 55. Secret exposed?
Use sensitive variables or vault.

---

## 56. Wrong resource created?
Fix config and re-apply.

---

## 57. Need multiple environments?
Use workspaces.

---

## 58. Dependency issue?
Use depends_on.

---

## 59. Need reusable code?
Use modules.

---

## 60. Production deployment?
Use CI/CD pipeline.

---
