# Part 1

## Exercise 1.1: Getting started
---
- Start 3 containers from image that does not automatically exit, detached.

``` shell
  docker container run -d cassandra
  docker container run -d httpd
  docker container run -d redis
```

- Stop 2 of the containers leaving 1 up.

``` shell
  docker container stop 747c4ab3ed35
  docker container stop 891c3b16a10e
```

- The output for docker ps -a which shows 2 stopped containers and one running.

``` shell
  CONTAINER ID   IMAGE       COMMAND                  CREATED          STATUS                            PORTS     NAMES
  747c4ab3ed35   cassandra   "docker-entrypoint.s…"   5 minutes ago    Exited (137) About a minute ago             peaceful_archimedes
  299640e7a507   httpd       "httpd-foreground"       9 minutes ago    Up 9 minutes                      80/tcp    nifty_archimedes
  891c3b16a10e   redis       "docker-entrypoint.s…"   18 minutes ago   Exited (0) About a minute ago               keen_cray
```