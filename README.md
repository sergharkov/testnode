## 1. Install docker in system
### 1.1 For install docker on host have to done steps by manual

[DOCKER INSTALL](https://docs.docker.com/engine/install/)

## 2. Running with docker
### 2.1 build docker image as artifact

```
docker build -t node:01 -f infra/DockerFile .
```
### 2.2 List docker images

```
docker image ls
```

### 2.3 docker up

Running:

```
docker run -d -p 8080:3000  --name PETnode node:01
```
To run in detached mode, use
```
docker run -d
```

### 2.4 list runners docker 

```
docker ps
```

### 2.5 clean docker runs

If you would like to do a clean run (i.e. remove all data in already stopped containers), you can run

```
docker container prune
```

to remove all unused containers

As an alternative you can run

```
docker system prune
```

### 2.6 Http GET app

If you would like to do a clean run (i.e. remove all data in already stopped containers), you can run

```
http://localhost:8080
```
[NODElocallink](http://localhost:8080)
before need open firewall port TCP:8080
