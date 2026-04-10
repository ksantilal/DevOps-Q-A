Docker
-------------------------
## Introductiion
Docker is a platform that allows developers to easily create, deploy, and run applications in containers. Containers are lightweight, portable, and self-sufficient units that can run consistently across different environments. Docker provides an efficient way to package applications and their dependencies, making it easier to manage and scale applications.

* Docker Image:

* Docker Container: 

* A Dockerfile contains instructions to build an image.
An image is a packaged application with everything it needs to run.
A container is a running instance of that image.
* Dockerfile builds image, and image runs as container.


## Virtulization vs Containerization



## Monolith vs Microservices



* Execute Command to installl always latest vesion of the docker.

``
`curl -fsSL https://get.docker.com -o install-docker.sh
sudo sh install-docker.sh`

- After this installation, a group called as docker is created. all the users who are part of this group can use docker
- Lets add a current user to docker group

`sudo usermod -aG docker <username>`
* Exit and relogin
* now execute `docker info`



