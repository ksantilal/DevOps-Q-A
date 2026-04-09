Docker Volume
-------------------------

* Docker volume named volume
* Path volume 

* You can bind or maped your docker container to host.

- `Docker volume ls`
- `Docker volume create mysqldata`
- `docker inspect mysqldata`
- `docker run -d --name mysql --network two-tier -v mysqldata:/var/lib/mysql -e MYSQL_ROOT_PASSWORD=root -e MYSQL_DATABASE=devops mysql`
- `docker rm mysql`
- `docker volume inspect mysqldata`
- `sudo su`
- `cd /var/lib/docker/volumes/mysqldata/_data`
- `ls`

### Persistent volume
* Steps
- `mkdir volumes`
- `cd volumes`
- `mkdir mysql`
- `cd mysql`
- `pwd`

* Now you can go to your projects/two-tier-flask-app/
* remove existing mysql container and create again.
- `docker run -d --name mysql --network two-tier -v /home/ubuntu/volumes/mysql:/var/lib/mysql -e MYSQL_ROOT_PASSWORD=root -e MYSQL_DATABASE=devops mysql`

* it will run and create in that path 
- `cd`
- `cd volumes`
- `mysql`
- `ls`