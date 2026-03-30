📄 k8s-commands-cheatsheet.md
# ☸️ Kubernetes Commands Cheat Sheet

---

## 🧱 Cluster Commands

```bash
kubectl cluster-info
kubectl get nodes -o wide
kubectl version
kubectl top nodes
kubectl get componentstatuses
📦 Pod Commands
kubectl get pods
kubectl get pods -o wide
kubectl get pod -l <label>=<value>
kubectl describe pod <name>
kubectl logs <pod>
kubectl exec -it <pod> -- <command>
kubectl delete pod <name>
kubectl explain pod --recursive
kubectl cp <pod>:<path> <local_path>

🚀 Deployment Commands
kubectl create deployment <name> --image=<image>
kubectl get deployments
kubectl describe deployment <name>
kubectl scale deployment <name> --replicas=<number>
kubectl rollout restart deployment <name>
kubectl apply -f deployment.yaml
kubectl apply -f deployment.yaml

🌐 Service Commands
kubectl get services
kubectl describe service <name>
kubectl expose pod <name>
kubectl delete service <name>
kubectl get secrets
kubectl describe configmap <name>
kubectl port-forward svc/<name> <local_port>:<service_port>

🗂️ Namespace Commands
kubectl get namespaces
kubectl create namespace <name>
kubectl delete namespace <name>
kubectl config set-context --current --namespace=<name>
kubectl config get-contexts

📊 Resource Commands
kubectl apply -f <file>
kubectl get <type>
kubectl edit <type> <name>
kubectl delete <type> <name>
kubectl describe <type> <name>
kubectl label <type> <name> <key>=<value>

📈 Stats & Events Commands
kubectl top nodes
kubectl top pods
kubectl get events
kubectl describe events

🔐 Permission Commands
kubectl get roles
kubectl get rolebindings
kubectl auth can-i <action> <resource>

🎯 Quick Notes
<type> → pod, deployment, service, etc.
<name> → resource name
<file> → YAML configuration file

🚀 One-Line Summary
Pods → kubectl get pods
Deployments → kubectl get deployments
Services → kubectl get services
Logs → kubectl logs <pod>
Debug → kubectl describe <resource>

💡 Interview Tips
Know difference between Pod, Deployment, Service
Practice kubectl get, describe, logs
Understand YAML + apply

---

# ✅ How to use in VS Code

1. Create file → `k8s-commands-cheatsheet.md`  
2. Paste the content  
3. Preview:
```bash
Ctrl + Shift + V