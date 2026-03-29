# Installing Docker on Ubuntu Linux

* Execute the following commands to get the latest version of docker 
```bash
sudo apt update
curl -fsSL https://get.docker.com -o install-docker.sh
sudo sh install-docker.sh
```
* Lets add current user to docker group 
```bash
sudo usermod -aG docker <username>
```
* Exit and relogin
* Lets Execute
`docker info`
`docker --version`

## Containerize the application

* This also means we need to create a image (docker image) of our application

### Images

* docker images will have following naming pattern `<name>:<tag>`
* `<name>` represent the image name of your applictaion and `<tag>` is not passed value is `<latest>`
* We can have multiple tags for same image
* In docker hub we have three typs of images 
    * Docker official images
        * this omages have `<name>:<tag>`
        * Examples:
            * nginx
            * alpine
            * openjdk
    * Docker verified publisher images
        * This images have `<publisher>/<name>:<tag>`
        * Examples:
            * jenkins/jenkins
    * Docker Community/Individual images
        * This images have `<username>/<name>:<tag>`
        * Examples:
            * kapilbamania/skate

### How to build iamges

* To build a docker images first know thw manual steps involved in bringing up your application.

* Once you we have steps, then we have two approaches in building images.
    * manual approach which involves creating a container & taking a snapshot (commit)
    * Automatable & repetitive approach as Dockerfile approach.

#### Lets build a docker image to have openjdk 17

* Findout the steps involved in installing openjdk 17 on 
    * ubuntu
    ```bash
    sudo apt update
    sudo apt install openjdk-17-jdk
    java -version
    ```
    * alpine7
    ```bash
    apk update
    apk add --no-cache openjdk17 gcompat
    ```
