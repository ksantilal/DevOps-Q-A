# ☸️ Kubernetes Interview Questions & Answers (DevOps)

---

# 🔹 BASIC KUBERNETES QUESTIONS

## 1. What is Kubernetes?
Kubernetes is a container orchestration tool used to deploy, manage, and scale applications.

---

## 2. Why Kubernetes?
- Auto scaling
- High availability
- Self-healing
- Load balancing

---

## 3. What is a cluster?
A cluster is a group of machines (nodes) running Kubernetes.

---

## 4. What is a node?
A node is a machine (VM or physical) where containers run.

---

## 5. Types of nodes?
- Master (Control Plane)
- Worker

---

# 🔹 KUBERNETES ARCHITECTURE

## 6. What is Control Plane?
Manages the cluster.

---

## 7. Components of Control Plane?
- API Server
- Scheduler
- Controller Manager
- etcd

---

## 8. What is API Server?
Entry point for all commands.

---

## 9. What is etcd?
Key-value store for cluster data.

---

## 10. What is Scheduler?
Assigns pods to nodes.

---

## 11. What is Controller Manager?
Maintains desired state.

---

## 12. Worker node components?
- Kubelet
- Kube-proxy
- Container runtime

---

## 13. What is Kubelet?
Agent that runs on each node.

---

## 14. What is Kube-proxy?
Handles networking.

---

# 🔹 CORE OBJECTS

## 15. What is a Pod?
Smallest deployable unit (one or more containers).
wrapper to a container. 

---

## 16. What is Deployment?
Manages pod replicas and updates.

---

## 17. What is ReplicaSet?
Ensures required number of pods running.

---

## 18. What is StatefulSet?
Used for stateful apps (databases).

---

## 19. What is DaemonSet?
Runs one pod per node.

---

## 20. What is Job?
Runs task once.

---

## 21. What is CronJob?
Runs scheduled jobs.

---

# 🔹 SERVICES & NETWORKING

## 22. What is Service?
Exposes pods to network.

---

## 23. Types of Services?
- ClusterIP (internal)
- NodePort (external via node)
- LoadBalancer (cloud LB)

---

## 24. What is Ingress?
Manages external HTTP/HTTPS access.

---

## 25. What is DNS in Kubernetes?
Service discovery inside cluster.

---

## 26. What is CNI?
Container Network Interface plugin.

---

# 🔹 STORAGE

## 27. What is Persistent Volume (PV)?
Storage resource in cluster.

---

## 28. What is Persistent Volume Claim (PVC)?
Request for storage.

---

## 29. What is StorageClass?
Defines storage type dynamically.

---

# 🔹 CONFIGURATION

## 30. What is ConfigMap?
Stores configuration data.

---

## 31. What is Secret?
Stores sensitive data.

---

# 🔹 HELM

## 32. What is Helm?
Package manager for Kubernetes.

---

## 33. What is Helm chart?
Collection of Kubernetes YAML files.

---

## 34. Helm commands
helm install
helm upgrade
helm uninstall

---

## 35. Why use Helm?
- Reusable configs
- Easy deployments

---

# 🔹 CLUSTER TYPES

## 36. Types of clusters?
- On-premise
    - Self Managed
        * Kind (kubernetes in docker)
        * kubeadm
        * kops
        * minikube
- Cloud (EKS, AKS, GKE)
- Managed Kubernetes

---

## 37. What is EKS?
Managed Kubernetes by AWS.

---

## 38. What is AKS?
Managed Kubernetes by Azure.

---

## 39. What is GKE?
Managed Kubernetes by Google.

---

# 🔹 ADVANCED QUESTIONS

## 40. What is auto-scaling?
Automatically scale pods/nodes.

---

## 41. What is HPA?
Horizontal Pod Autoscaler.

---

## 42. What is rolling update?
Update pods gradually.

---

## 43. What is rollback?
Revert to previous version.

---

## 44. What is self-healing?
Restart failed containers automatically.

---

## 45. What is namespace?
Logical separation of resources.

---

## 46. What is RBAC?
Role-based access control.

---

## 47. What is kubeconfig?
File to connect to cluster.

---

## 48. What is sidecar container?
Helper container in same pod.

---

## 49. What is init container?
Runs before main container.

---

## 50. What is service mesh?
Manages communication (Istio).

---

# 🧪 REAL-TIME SCENARIOS

## 51. Pod not starting?
- Check logs
- Check describe pod
- Check image

---

## 52. Service not accessible?
- Check service type
- Check ports
- Check ingress

---

## 53. Pod crash loop?
- Check logs
- Fix config

---

## 54. High traffic?
Use HPA

---

## 55. Storage issue?
Check PVC/PV binding

---

## 56. Deployment failed?
Rollback deployment

---

## 57. Cannot connect to cluster?
Check kubeconfig

---

## 58. Node down?
Reschedule pods

---

## 59. Config issue?
Check ConfigMap/Secret

---

## 60. Debug production issue?
Logs → Metrics → Restart → Fix

---

