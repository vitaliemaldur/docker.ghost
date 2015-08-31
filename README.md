## Docker setup for Ghost blogging platform
This is generic Ghost setup with a Ngnix front-end.

### Prerequisites

- Install [Docker](https://docs.docker.com/installation/)
- Install [Compose](https://docs.docker.com/compose/install/)

### Themes
Add new themes in the `ghost/themes` folder. You will found two themes there, Casper and Ghostium.

### Persistent data
If you are using default SQLite database, you can found you db file in `ghost/data` directory. It is mapped as
volume in Ghost container to make your db persistent on the host filesystem. 

### Installation
Get Dockerfiles

      $ git clone --recursive https://github.com/vitaliemaldur/docker.ghost

Edit Ghost and Ngnix configuration files

      $ vim /path/to/docker.ghost/ghost/config.js
      $ vim /path/to/docker.ghost/ngnix/ghost.conf

Start containers

      $ docker-compose up -f /path/to/docker.ghost/docker-compose.yml
