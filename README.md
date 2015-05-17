## Docker setup for Ghost blogging platform
This is generic Ghost setup with a Ngnix front-end.

### Prerequisites

- Install [Docker](https://docs.docker.com/installation/)
- Install [Compose](https://docs.docker.com/compose/install/)

### Installation
Get Dockerfiles

      $ git clone https://github.com/vitaliemaldur/docker.ghost

Edit Ghost and Ngnix configuration files

      $ vim /path/to/docker.ghost/ghost/config.js
      $ vim /path/to/docker.ghost/ngnix/ghost.conf
      
Start containers

      $ docker-compose up -f /path/to/docker.ghost/docker-compose.yml
