### Running Website

#### Physical Servers
* Vmware

### Hypervisors

### Containers
* Containers are portable
* Containers are lightweight

# Docker

* Docker was named after dock workers.
* Docker was a side project ina company called as dotcloud
* Solomon Hykes had first demonstrated docker in a pycon and it become overnight success.

* 🐳 Docker Interview Questions + Answers
🟢 1. What is Docker?

Answer:
Docker is a containerization platform that packages an application with all its dependencies into a container, ensuring it runs consistently across environments.

🟢 2. What is a container?

Answer:
A container is a lightweight, isolated environment that runs an application using the host OS kernel.

🟢 3. Docker vs Virtual Machine?

Answer:

Docker	VM
Lightweight	Heavy
Shares OS kernel	Full OS
Fast startup	Slow startup
🟢 4. What is a Docker Image?

Answer:
A Docker image is a read-only template used to create containers.

🟢 5. What is a Dockerfile?

Answer:
A Dockerfile is a script with instructions to build a Docker image.

Example:

FROM node:18
WORKDIR /app
COPY . .
RUN npm install
CMD ["npm", "start"]
🟡 6. Image vs Container?

Answer:

Image = blueprint
Container = running instance
🟡 7. Common Docker commands?

Answer:

docker build -t app .
docker run -d -p 3000:3000 app
docker ps
docker stop <id>
docker rm <id>
🟡 8. What is port mapping?

Answer:
It connects container ports to host ports.

Example:

docker run -p 8080:80 nginx
🟡 9. What are Docker volumes?

Answer:
Volumes are used to persist data outside the container lifecycle.

🟡 10. Bind mount vs Volume?

Answer:

Bind mount → specific host folder
Volume → managed by Docker
🟡 11. What is Docker networking?

Answer:
Docker provides networking types like:

bridge (default)
host
overlay
🔵 12. What is Docker Compose?

Answer:
A tool to define and run multi-container applications using a YAML file.

Example:

version: "3"
services:
  web:
    image: nginx
    ports:
      - "8080:80"
🔵 13. What is multi-stage build?

Answer:
A technique to reduce image size by using multiple build steps and copying only necessary files.

🔵 14. What is Docker Swarm?

Answer:
Docker’s native tool for clustering and orchestration of containers.

🔵 15. What is container lifecycle?

Answer:
create → run → pause → stop → remove

🔴 16. How do you reduce Docker image size?

Answer:

Use Alpine base image
Remove unnecessary files
Use multi-stage builds
Use .dockerignore
🔴 17. How do you debug a container?

Answer:

docker logs <container_id>
docker exec -it <container_id> bash
🔴 18. How to pass environment variables?

Answer:

docker run -e APP_ENV=prod myapp
🔴 19. How to persist data?

Answer:
Use volumes:

docker run -v mydata:/data myapp
🔴 20. Explain Docker architecture

Answer:

Client → sends commands
Daemon → runs containers
Registry → stores images
⚡ 21. Docker vs Kubernetes?

Answer:

Docker → container runtime
Kubernetes → container orchestration platform
⚡ 22. How Docker is used in CI/CD?

Answer:

Build image
Run tests
Deploy container
🎯 Final Tip (VERY IMPORTANT)

In interviews:
👉 Don’t just define — give examples

Example:

“We used Docker to containerize a Node.js app and deployed it using Docker Compose.”