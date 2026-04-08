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
