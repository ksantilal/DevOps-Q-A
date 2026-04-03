# Running Website & Server Infrastructure

##  Idea
* Understand how **websites run on servers**
* Learn about **infrastructure layers**
   

---

## 🖥️ Physical Servers

### 📌 Overview
- Traditional way of hosting applications
- One server = one operating system = one workload

### ⚠️ Problems
- Resource wastage
- Hard to scale
- Expensive

---

## 🧩 Hypervisors (Virtualization)

### 📌 Overview
- Software that creates **virtual machines (VMs)**
- Allows multiple OS on one physical machine

### ✅ Benefits
- Better resource utilization
- Isolation between systems

### ❌ Limitations
- Heavy (each VM has its own OS)

---

## 📦 Containers

### 📌 Overview
- Lightweight alternative to VMs
- Share the host OS kernel

### 🚀 Key Points
- Very **fast and portable**
- Use fewer resources
- Ideal for modern applications

---

## 🐳 Docker

### 📌 What is Docker?
- A platform to **build, ship, and run containers**

### 🏗️ History
- Named after **dock workers (shipping container analogy)**
- Started as a side project at **dotCloud**
- Created by **Solomon Hykes**
- First demo at **PyCon → became an overnight success**
- Company renamed to **Docker Inc.**

---

## 🧬 Evolution of Containers
- Containers existed in **Linux (late 1990s)**
- But:
  - Required **low-level coding**
  - Hard to use
  - Used by companies like **Google**

### 🔥 Breakthrough
- Docker **simplified containers**
- Made them accessible to everyone

---

## 🪟 Windows & Containers
- Microsoft updated Windows to support containers

### Supported in:
- Windows 10+
- Windows Server 2016+

---

## 💡 Summary

| Technology        | 특징 |
|------------------|------|
| Physical Servers | Inefficient |
| Virtual Machines | Better but heavy |
| Containers       | Lightweight & fast |
| Docker           | Made containers easy & popular |