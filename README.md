# Ghost & MySQL with Docker, Kubernetes and Mesos

In this project we will connect a ghost container with a persistent MySQL container.

Prerequisition: Docker version 1.11.x <

#### Create named docker volume
```
docker volume create --name mysql-volume
```

#### Start with Docker Compose
Check the docker-compose file for more documentation
```
$ docker-compose up  -d
```

```
$ docker-compose --file docker-compose-v2.yaml up -d
```


#### Cleanup the running containers
```
docker-compose stop
docker-compose rm -fv
docker volume rm mysql-volume
```
