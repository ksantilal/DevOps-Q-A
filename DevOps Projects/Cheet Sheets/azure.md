# Azure Cheat Sheet

## 🔑 Login
- `az login` → Authenticate

## 📁 Resource Groups
- `az group list` → List groups
- `az group create --name rg --location uk` → Create group

## 💻 VM
- `az vm create --name vm --resource-group rg --image UbuntuLTS` → Create VM
- `az vm start --name vm --resource-group rg` → Start VM
- `az vm stop --name vm --resource-group rg` → Stop VM

## 📦 Storage
- `az storage account list` → List storage accounts

## ☸️ AKS
- `az aks create --name aks --resource-group rg` → Create cluster
- `az aks get-credentials --name aks --resource-group rg` → Configure kubectl
