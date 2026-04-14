Docker Compose
-------------------------

### Installation

- `sudo apt-get update && sudo apt-get upgrade -y`
- `sudo apt-get install docker-compose-v2`

* Docker compose tool that can automate.
* It is used to define and run multi-container Docker applications.

### Configuration file Yaml

* Docker compose uses a YAML file to configure the application’s services, networks, and volumes.
* The default file name is `docker-compose.yml`.

* YAML `stads for yet another markup language`

```Yaml
version: '3.8'
services:
  mysql:
    image: mysql
    environment:
      MYSQL_DATABASE: "devops"
      MYSQL_ROOT_PASSWORD: "root"
    ports:
        - "3306:3306"
    volumes:
      - mysqldata:/var/lib/mysql
    networks:
        - two-tier
          

  flask:
  
  web:
    build: .
    ports:
      - "5000:5000"
    volumes:
      - .:/code
    environment:
      FLASK_ENV: development
  redis:
    image: "redis:alpine"

```