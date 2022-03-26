# Part 1

## Exercise 1.5: Size of images

- Pulling **_devopsdockeruh/simple-web-service:alpine_** and **_devopsdockeruh/simple-web-service:ubuntu_** images.

``` shell
  docker pull devopsdockeruh/simple-web-service:alpine

  docker pull devopsdockeruh/simple-web-service:ubuntu
```

- Comparing the image sizes

``` shell
  docker images

  REPOSITORY                           TAG                                           IMAGE ID       CREATED         SIZE

  devopsdockeruh/simple-web-service    ubuntu                                        4e3362e907d5   2 days ago   83MB

  devopsdockeruh/simple-web-service    alpine                                        fd312adc88e0   2 days ago   15.7MB
```

- Go inside the alpine conitainer and make sure the secret message functionally is the same.

```shell
  docker run --rm -ti --name web-service-alpine -d devopsdockeruh/simple-web-service:alpine

  docker exec -ti web-servie-alpine sh

  tail -f ./text.log
```