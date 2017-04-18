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

### About Virtual Host

You need to set up virtual host ip in file /etc/hosts

1. Confirm your docker-machine IP address

`docker-machine ip [name]` 

Mine is **192.168.99.100**

2. Edit file /etc/hosts in windows

`vi /etc/hosts`

Add

`[YourIpAddress] [YourVirtualDomain]`

[YourVirtualDomain] is set in nginx/nginx_conf/conf.d/virtualhost/**YourVirtualDomain**.conf

Eg:

`192.168.99.100 vinh-test.i-enter.local`
