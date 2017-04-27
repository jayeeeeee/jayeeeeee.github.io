---
layout: post
title:  "Getting started with Docker"
date:   2017-04-20 16:00:00 +0800
categories: docker
---
### Docker
[https://www.docker.com/][docker]

[docker]: https://www.docker.com/

### Environment
Windows 10 Home

### Setup

#### Installation
- Win10 Home

    [Docker Toolbox][docker-toolbox]
    
- Win10 Professional or Enterprise
    
    [Docker for windows][docker-download]
    
[docker-toolbox]: https://www.docker.com/products/docker-toolbox
[docker-download]: https://www.docker.com/docker-windows
    
[jmeter-download]: http://jmeter.apache.org/download_jmeter

#### Launch

    Docker Quickstart Terminal

### Offical Tutorials
1. Hello world

    `docker run hello-world`

2.    To be continued...

### Appendix

#### Commands
-   docker

    ```
    docker build [image_name] .  <-Important of this "dot"!
    docker images
    docker run [image_name]
    docker rmi [image_name | image_id]
    docker ps
    docker ps -a
    docker logs [container_id]
    docker exec -it [container_id] bash
    ```
    
-   docker-machine

    ```
    docker-machine ls
    docker-machine ssh [machine_name]   
    docker-machine scp localhost:[file_source_path] [machine_name]:[file_target_directory]
    ```

-   docker stack
    ```
    docker swarm init --advertise-addr [node_ip]
    docker stack deploy --compose-file [docker_compose_file_path] [service_name]
    docker stack rm [service_name]
    ```