# Docker notes

## Common Command

`docker pull busybox`  
`docker images` list images

`docker run busybox`  
`docker run --rm prakhar1989/static-site`

`docker ps` list container currently run
`docker ps -a` list all container  
`docker run -it busybox sh` interactive tty

`docker rm $(docker ps -a -q -f status=exited)`  
> `-q` only return numeric IDs  
> `-f` filter

`docker container prune`

`docker rmi busybox`

`docker run -d -P --name static-site prakhar1989/static-site`
> `-d` detached mode  
> `-P` publish  
> `--name` name for container

`docker port static-site`

`docker run -p 8888:80 prakhar1989/static-site`

`docker stop static-site`

`docker build -t shine0901/catnip .`

`docker push shine0901/catnip`

## Term

Images, Container, Docker Daemon, Docker Client, Docker Hub

## Type Images

Base Image and Child Image  
Official Image and User Image
