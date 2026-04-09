Installations and Setups docker
------------------------------------------

* ssh into instance
- `ssh -i key user instanceid`
* update and upgrade 
- `sudo apt update && sudo apt upgrade -y`
* Install docker 
- `curl -fsSL https://get.docker.com -o install-docker.sh`
- `sudo sh install-docker.sh`
or
`sudo apt install docker.io -y`
* After this installation, a group called as docker is created. all the users who are part of this group can use docker
- `whoami`
- `sudo usermod -aG docker $USER`
* Exit and relogin
or  
- `sudo newgrp docker`
* now execute 
- `docker info`
- `docker images`
- `docker ps`

* Usefull Commands
- `sudo systemctl start docker`
- `sudo systemctl enable docker`
- `sudo systemctl status docker`

### Java Application

* Steps
- [URL]https://github.com/LondheShubham153/simple-java-docker.git
- mkdir projects
- cd projects
- git clone "repo"
- ls and cd project-path
- vi Dockerfile 

* write a dockerfile which will contains set of instructions

```Dockerfile
# pull a base image which gives all required tools and libraries
FROM openjdk:17--jdk-alpine

# create a folder where the app code will be stored
WORKDIR /app

# copy the source code from your HOST machine to your container 
COPY src/main.java /app/main.java

# compile the application code
RUN javac Main.java

# run the application
  it can be overridden
CMD ["java","Main"]

# it can not be overridden 
ENTRYPOINT 

```
- `cat Dockerfile`

* Build the image
- `docker build -t java-app .`
- `docker images`or `docker image ls`
* Run the container
- `docker run java-app`
- `docker ps` or `docker ps -a`
* Explore commands
- `docker run -d -p --name java-app 80:80 java-app:1.0`

### Python Application 
* Steps
* [URL](https://github.com/LondheShubham153/flask-app-ecs.git)
- mkdir projects
- cd projects
- git clone "repo"
- ls and cd project-path
- vi Dockerfile
```Dockerfile
FROM python:3.7

WORKDIR /app

COPY . .

RUN pip install -r requirements.txt

CMD ["python","run.py"]

```
- Esc:wq
- `cat Dockerfile`
* Build the image
- `docker build -t flask-app .`
- `docker images`or `docker image ls`
* Run the container
- `docker run -d -p 80:80 flask-app`
- `docker ps` or `docker ps -a`
* Access app instanceIP:portnumer
- `docker logs containerid`
- `docker attach containerid`
* To enter inside the container
- `docker exec -it containerid bash` 

* Mysql 
- docker pull mysql
- docker run -e MYSQL_ROOT_PASSWORD=root mysql

* enter into the container
* `docker exec -it containerid bash`
- `mysql -u root -p`
- `password - root`
- `show databases`
- `create database devops`
- `exit` 

* nodejs project


