# Part 1

## Exercise 1.2: Cleanup
---
- Clean the docker daemon from all images and containers.

``` shell
  docker stop 299640e7a507

  docker container prune

  docker image prune -a

```

- The output for docker ps -a and docker images

``` shell
docker ps -a

CONTAINER ID   IMAGE     COMMAND   CREATED   STATUS    PORTS     NAMES

docker images

REPOSITORY   TAG       IMAGE ID   CREATED   SIZE
```