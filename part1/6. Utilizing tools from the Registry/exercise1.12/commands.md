# Part 1

## Exercise 1.12: Hello, frontend!
---
- Create a Dockerfile for the project (example-frontend) and give a command so that the project runs in a docker container with port 5000 exposed and published so when you start the container and navigate to http://localhost:5000 you will see message if you're successful.

``` powershell
    
    docker build . -t example-frontend

    docker run -ti --name frontend-example -p 5000:5000 example-frontend
```
