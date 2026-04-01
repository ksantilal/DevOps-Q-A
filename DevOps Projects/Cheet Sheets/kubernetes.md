# Kubernetes Cheat Sheet

## 🧠 Cluster
- `kubectl cluster-info` → Cluster details
- `kubectl get nodes` → List nodes

## 📦 Pods
- `kubectl get pods` → List pods
- `kubectl describe pod name` → Pod details
- `kubectl delete pod name` → Delete pod

## 🚀 Deployments
- `kubectl get deployments` → List deployments
- `kubectl apply -f file.yaml` → Create/update resources
- `kubectl delete -f file.yaml` → Delete resources

## 🌐 Services
- `kubectl get svc` → List services
- `kubectl expose deployment app` → Expose app

## 📜 Logs & Access
- `kubectl logs pod` → View logs
- `kubectl exec -it pod -- bash` → Access container

## 📂 Namespaces
- `kubectl get ns` → List namespaces
- `kubectl create ns dev` → Create namespace