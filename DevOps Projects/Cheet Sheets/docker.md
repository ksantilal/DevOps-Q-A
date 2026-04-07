# Docker Cheat Sheet

- `docker info`
- `docker pull nginx:1.27`

### To build docker image
- `docker image build -t fashion:1.0 .`

* Now lets build the container with this image
- `docker container run -d --name web1 -P fashion:1.0`
- `docker (contaiiner)run -d --name web1 -P nginx:myapp`
- `editor vi, vim, nano` 
- `esc :wq,q!`
- `docker inspect id`
- `systemctl start doker`
- `systemctl enable doker`
- `systemctl status doker`

- `sudo usermod -aG docker user(ubuntu)`
- `docker login -u username` -> login docker
- `chmod +x filename`



## 📦 Images
- `docker build -t name .` → Build image
- `docker images` → List images
- `docker image ls`-> List all Images
- `docker pull image` → Download image
- `docker rmi image` → Remove image
- `docker rmi $(docker images -q)` -> remove all images 
- `docker rm $(docker ps -aq)` -> remove all container

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