Docker Networking
-------------------------
* Total seven types of Docker Network
1. Host
2. Bridge (default)
3. None 
* These three are an important

4. User defined Bridge (custom)
5. MACVLAN(docker swarm)
6. Overlay
7. IPVLAN

* Commands to explore docker network
- `docker network ls`
* To create a network
- `docker network create mynetwork -d bridge`

### Two tier application
* [URL]https://github.com/LondheShubham153/two-tier-flask-app.git

* Steps
- `git clone repo`
- `cd repo-path`
- `ls`
- `docker network create two-tier -d bridge`
- `vim Dockerfile`
- `docker build -t two-tier-backend .`
- `docker ps -a`
- `docker run -d --name mysql --network two-tier -e MYSQL_ROOT_PASSWORD=root -e MYSQL_DATABASE=devops mysql`
- `docker run -d -p 5000:5000 --network two-tier- -e MYSQL_HOST=mysql -e MYSQL_USER=root -e MYSQL_PASSWORD=root -e MYSQL_DB=devops two-tier-backend:latest`
- `docker ps -a`
- `docker logs id`
- `docker network inspect two-tier`
- `docker exec -it mysql bash`
- `mysql -u root -p`
- `password - root`
- `use database devops`
- `show databases;`
- `use devops`
- `select * from messages;`

## Give network to containers
* Steps
* Create a network
- `docker network create mynetwork -d bridge`
- `docker network ls`

* Give network to container
* Mysql container 
- `docker run -d --name mysql --network mynetwork mysql -e MYSQL_ROOT_PASSWORD=root -e MYSQL_DATABASE=devops mysql`

* Connect both the container to same network for communicates each other
* Flask-app container 
-  `docker run -d -p 5000:5000 --network mynetwork -e MYSQL_HOST=mysql -e MYSQL_USER=root -e MYSQL_PASSWORD=root -e MYSQL_DB=devops two-tier-backend:latest`

