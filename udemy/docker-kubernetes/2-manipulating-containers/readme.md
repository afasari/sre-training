# Manipulating Containers with the Docker Client

## Docker Run

```cli
docker run <image name> <command>

eg.
docker run busybox echo hi there
results.
hi there
```

docker run = docker create + docker start
create = create image file system snapshot
start = execute image startup command

## Docker List Running Containers

```cli
docker ps

docker ps --all // all with history that already stoped
```

## Docker Remove Stoped Containers

```cli
docker system prune
```

will clear docker ps --all

## Docker Logs

```cli
docker logs <container id>
```

## Docker Stop and Kill

```cli
docker stop <container id>
```

send SIGTERM to container, stop the process. it is gracefully shutdown, if now, will run docker kill. recommended.

```cli
docker kill <container id>
```

send SIGTERM to container, kill the process forcefully
