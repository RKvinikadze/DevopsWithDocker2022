# Part 1

## Exercise 1.10: Ports open
---
- Create a Dockerfile for an old Java Spring project

``` powershell
    
    docker build . -t spring-example

    docker run -ti -p 8080:8080 spring-example
```
