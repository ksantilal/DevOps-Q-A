# 🐳 Docker Interview Questions & Answers (DevOps)

---

# 🔹 BASIC DOCKER QUESTIONS

* Two Components of docker
    * Docker Client
    * Docker Server/Engine

## 1. What is Docker?
Docker is an open source tool that used to create, run, and manage containers.

---

## 2. What is a container?
A container is a lightweight environment that includes application + dependencies.
-> It's a running Instance, where you can deploy your application.


---

## 3. What is an image?
An image is a blueprint used to create containers.

---

## 4. Difference between image and container?
- Image = template
- Container = running instance

---

## 5. What is Dockerfile?
A file with instructions to build a Docker image.

---

## 6. What is Docker Hub?
A registry to store and share Docker images.

---

## 7. What is containerization?
Packaging app with dependencies so it runs anywhere.

---

## 8. What is virtualization vs containerization?
- VM = full OS
- Container = lightweight, shares OS

---

## 9. What is Docker Engine?
Core component that runs containers.

---

## 10. What is Docker CLI?
Command line tool to interact with Docker.

---

# 🔹 DOCKER COMMANDS

## 11. Build image
docker build -t app .

---

## 12. Run container
docker run -d -p 80:80 nginx

---

## 13. List containers
docker ps
docker ps -a

---

## 14. Stop container
docker stop id

---

## 15. Remove container
docker rm id

---

## 16. List images
docker images

---

## 17. Remove image
docker rmi image

---

## 18. View logs
docker logs id

---

## 19. Exec into container
docker exec -it id bash

---

## 20. Inspect container
docker inspect id

---

# 🔹 DOCKERFILE QUESTIONS

## 21. What are common Dockerfile instructions?
- FROM → base image
- RUN → execute command
- COPY → copy files
- CMD → default command
- ENTRYPOINT → main command

---

## 22. Difference between CMD and ENTRYPOINT?
- CMD = default (can override)
- ENTRYPOINT = fixed command

---

## 23. What is multi-stage build?
Using multiple steps to reduce image size.

---

## 24. How to optimize Docker image?
- Use small base image (alpine)
- Remove unnecessary files
- Use multi-stage builds

---

## 25. What is .dockerignore?
Ignore files while building image.

---

# 🔹 DOCKER NETWORKING

## 26. Types of networks?
- bridge
- host
- overlay

---

## 27. What is port mapping?
Mapping container port to host port.

Example:
docker run -p 8080:80 nginx

---

## 28. How containers communicate?
- Same network → direct communication
- Different network → needs configuration

---

# 🔹 DOCKER VOLUMES

## 29. What is volume?
Persistent storage for containers.

---

## 30. Types of storage?
- Volumes
- Bind mounts

---

## 31. Why use volumes?
To persist data after container stops.

---

# 🔹 DOCKER COMPOSE

## 32. What is Docker Compose?
Tool to run multi-container applications using YAML.

---

## 33. What is docker-compose.yml?
Configuration file for services.

---

## 34. Basic Compose example
version: "3"
services:
  web:
    image: nginx
    ports:
      - "80:80"

---

## 35. Commands
docker-compose up -d → start
docker-compose down → stop

---

## 36. Why use Compose?
- Manage multiple containers
- Simplify setup

---

# 🔹 DOCKER SWARM

## 37. What is Docker Swarm?
Docker’s native orchestration tool.

---

## 38. What is a node?
A machine in swarm cluster.

---

## 39. Types of nodes?
- Manager
- Worker

---

## 40. What is a service?
Defines how containers run in swarm.

---

## 41. What is scaling?
Running multiple container replicas.

---

## 42. What is load balancing?
Distributing traffic across containers.

---

## 43. Commands
docker swarm init
docker service create
docker service scale

---

# 🔹 ADVANCED QUESTIONS

## 44. What is orchestration?
Managing containers at scale.

---

## 45. Docker vs Kubernetes?
- Docker = container runtime
- Kubernetes = orchestration

---

## 46. What is health check?
Check if container is working.

---

## 47. What is logging driver?
Defines how logs are stored.

---

## 48. What is registry?
Storage for Docker images.

---

## 49. What is tagging?
Versioning images (app:v1)

---

## 50. What is overlay network?
Network for swarm communication.

---

# 🧪 REAL-TIME SCENARIOS

## 51. Container not starting?
- Check logs
- Check Dockerfile
- Check ports

---

## 52. Port not accessible?
- Check mapping
- Check firewall

---

## 53. Data lost after restart?
Use volumes

---

## 54. High CPU usage?
Check container stats

---

## 55. Image build slow?
Use caching & optimize Dockerfile

---

## 56. Multiple containers needed?
Use Docker Compose

---

## 57. Scale application?
Use Docker Swarm or Kubernetes

---

## 58. Debug container?
docker exec -it id bash

---

## 59. Cannot pull image?
Check network or Docker Hub

---

## 60. Production deployment?
Use orchestration + monitoring

---

