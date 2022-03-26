# Part 1

## Exercise 1.3: Secret message
---
- Commands

``` shell
  docker run -d -ti --name secret-message devopsdockeruh/simple-web-service:ubuntu

  docker exec -ti secret-message bash

  tail -f ./text.log
```

- Secret message

``` shell
  Secret message is: 'You can find the source code here: https://github.com/docker-hy'
```