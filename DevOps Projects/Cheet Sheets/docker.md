# Docker Cheat Sheet

## 📦 Images
- `docker build -t name .` → Build image
- `docker images` → List images
- `docker pull image` → Download image
- `docker rmi image` → Remove image

## 📦 Containers
- `docker run -d -p 80:80 image` → Run container (detached)
- `docker ps` → Running containers
- `docker ps -a` → All containers
- `docker stop id` → Stop container
- `docker rm id` → Remove container

## 🖥 Exec
- `docker exec -it id bash` → Enter container shell

## 📜 Logs
- `docker logs id` → View logs

## 💾 Volumes
- `docker volume create vol` → Create volume
- `docker run -v vol:/data image` → Mount volume

## 📄 Compose
- `docker-compose up -d` → Start services
- `docker-compose down` → Stop services