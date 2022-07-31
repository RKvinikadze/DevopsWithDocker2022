# Part 1

## Exercise 1.13: Hello, backend!
---
- Create a Dockerfile for the project (example-backend). Start the container with port 8080 published.

When you start the container and navigate to http://localhost:8080/ping you should get a "pong" as response.

``` powershell
    
    docker build . -t example-backend

    docker run -ti --name backend-example -p 8080:8080 example-backend
```
