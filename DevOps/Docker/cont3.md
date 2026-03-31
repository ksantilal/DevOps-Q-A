## Containerizing applications

* Generally we run serverside components in the containers such as web servers, databases, webstores etc…

### Monolith vs Microservices

* Lets bring up a Website in a container
HTML Refer Here download link

* steps

```bash
mkdir website
cd website
wget https://www.free-css.com/assets/files/free-css-templates/download/page296/little-fashion.zip
unzip little-fashion.zip
mv 2127_little_fashion/ fashion/
# move this folder to html location in webserver 2127_little_fashion
# mv 2127_little_fashion /var/www/html/fashion/
```
* Webservers:
    * apache: /usr/local/apache2/htdocs/
    * nginx: default directory /usr/share/nginx/html

* Create a file called as `Dockerfile`
* add the following
```Dockerfile
FROM nginx:1.27
COPY fashion/ /usr/share/nginx/html/fashion/

```
## Dockerfile

* Dockerfile contains instructions to build the image
* Basic syntax
```bash
<INSTRUCTION 1> <arguments>
<INSTRUCTION 2> <arguments>
..
<INSTRUCTION n> <arguments>
``` 
### Nacessary Instructions

####  _FROM_: 
* This instruction is used to select base image
```
FROM nginx
FROM nginx:1.27
```
* What is amd vs arm platform where are they used?

### ADD
* ADD instruction can copy the file or folder into docker image from host or remote sources (https)
### COPY
* ADD instruction can copy the file or folder into docker image from host or remote sources (https)
* COPY instruction can copy file or folder into docker image from host

* Now add the following
```bash
FROM nginx:1.27
COPY fashion/ /usr/share/nginx/html/fashion/
```

* Now to build the docker image lets use docker build command
```bash
docker image build -t fashion:1.0 .
```

* Now lets view the images
```bash
docker image ls
```

* Now lets build the container with this image
```bash
docker container run -d --name web1 -P fashion:1.0
```
* Note: use this instruction docker container run -d --name web2 -p 80:80 fashion:1.0

