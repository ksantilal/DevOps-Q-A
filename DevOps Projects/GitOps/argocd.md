# 🔄 GitOps & Argo CD Interview Questions and Answers

---

# 🔹 BASIC GITOPS QUESTIONS

## 1. What is GitOps?
GitOps is a way of managing infrastructure and applications using Git as the source of truth.

---

## 2. What is the main idea of GitOps?
Everything is stored in Git and automatically applied to systems.

---

## 3. What are benefits of GitOps?
- Automation
- Version control
- Easy rollback
- Transparency

---

## 4. GitOps vs CI/CD?
- CI/CD = pipeline-driven deployment
- GitOps = Git-driven deployment

---

## 5. What is source of truth?
Git repository that stores desired state.

---

## 6. What is desired state?
Configuration defined in Git.

---

## 7. What is actual state?
Current state in cluster.

---

## 8. What is drift?
Difference between desired and actual state.

---

## 9. How GitOps works?
1. Update code in Git
2. Tool detects change
3. Applies to cluster

---

## 10. What tools support GitOps?
- Argo CD
- Flux

---

# 🔹 ARGO CD BASICS

## 11. What is Argo CD?
Argo CD is a GitOps tool for Kubernetes deployments.

---

## 12. How Argo CD works?
It monitors Git repo and syncs changes to Kubernetes.

---

## 13. What is Argo CD architecture?
- API Server
- Repo Server
- Application Controller
- UI

---

## 14. What is Application in Argo CD?
Defines what to deploy and where.

---

## 15. What is sync?
Apply changes from Git to cluster.

---

## 16. What is auto-sync?
Automatically sync when changes detected.

---

## 17. What is manual sync?
User triggers deployment.

---

## 18. What is health status?
Indicates app condition (Healthy/Degraded).

---

## 19. What is sync status?
Indicates if app is in sync with Git.

---

## 20. What is rollback?
Revert to previous version using Git history.

---

# 🔹 ARGO CD ADVANCED

## 21. What is declarative configuration?
Define everything in YAML.

---

## 22. What is Helm in Argo CD?
Use Helm charts for deployment.

---

## 23. What is Kustomize?
Tool to customize Kubernetes YAML.

---

## 24. What is multi-cluster support?
Manage multiple Kubernetes clusters.

---

## 25. What is RBAC in Argo CD?
Role-based access control.

---

## 26. What is application grouping?
Organizing apps using projects.

---

## 27. What is sync policy?
Defines how syncing happens.

---

## 28. What is hook in Argo CD?
Run tasks before/after deployment.

---

## 29. What is pruning?
Remove unused resources.

---

## 30. What is self-healing?
Automatically fix drift.

---

# 🔹 GITOPS WORKFLOW

## 31. Typical workflow?
1. Developer commits code
2. Push to Git
3. Argo CD detects change
4. Deploys to cluster

---

## 32. GitOps vs traditional deployment?
GitOps is automated and Git-driven.

---

## 33. How to rollback in GitOps?
Revert commit in Git.

---

## 34. How to handle secrets?
Use external secret managers.

---

## 35. How to manage environments?
Separate branches or folders.

---

# 🔹 KUBERNETES + GITOPS

## 36. Why GitOps for Kubernetes?
Simplifies deployments and scaling.

---

## 37. How Argo CD interacts with Kubernetes?
Uses API server to apply configs.

---

## 38. What is namespace usage?
Separate environments.

---

## 39. What is config drift?
Mismatch between Git and cluster.

---

## 40. How to fix drift?
Sync application.

---

# 🔹 SECURITY

## 41. How to secure GitOps?
- RBAC
- Secrets management
- HTTPS repos

---

## 42. What is least privilege?
Minimal access required.

---

## 43. What is audit trail?
Git history for tracking changes.

---

# 🧪 REAL-TIME SCENARIOS

## 44. Deployment not updating?
Check sync status and logs.

---

## 45. App out of sync?
Run sync or enable auto-sync.

---

## 46. Wrong config deployed?
Rollback using Git.

---

## 47. Cluster drift detected?
Enable self-healing.

---

## 48. Multiple environments?
Use branches or directories.

---

## 49. Secrets exposed?
Use Vault or external tools.

---

## 50. Helm chart not working?
Check values.yaml.

---

## 51. Cannot connect to repo?
Check credentials and access.

---

## 52. Sync failing?
Check logs and permissions.

---

## 53. Application unhealthy?
Check pod logs and events.

---

## 54. Manual override needed?
Disable auto-sync.

---

## 55. CI/CD integration?
CI builds → Git push → Argo CD deploys

---

## 56. Multi-cluster deployment?
Configure multiple clusters in Argo CD.

---

## 57. Namespace issue?
Check namespace config.

---

## 58. Deployment slow?
Check cluster resources.

---

## 59. Pod crash?
Check logs.

---

## 60. Production issue?
Rollback + fix Git config.

---
