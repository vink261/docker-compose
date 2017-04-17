# docker-compose
### How to use

1. `git clone https://github.com/vink261/docker-compose.git`

2. `cd docker-compose`

3. Start docker -> `docker-machine start [name]`

You may need to `docker-machine env [name]`

4. `docker-compose up -d`

5. `docker-compose ps`

### How to enter container

`docker exec -it [container-name] /bin/bash`
