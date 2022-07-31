# Part 1

## Exercise 1.11: Spring
---
- Create a Dockerfile for an old Java Spring project

``` powershell
    
    docker build . -t example-spring

    docker run -ti --name spring-example -p 8080:8080 example-spring
```
