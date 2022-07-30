# Part 1

## Exercise 1.10: Ports open
---
- The image devopsdockeruh/simple-web-service will start a web service in port 8080 when given the command "server". From 1.7 you should have an image ready for this. Use -p flag to access the contents with your browser. The output to your browser should be something like: 
*{ message: "You connected to the following path: ...*

``` powershell
    docker run -ti 
    -p 127.0.0.1:8080:8080 
    --name simple-web-service 
    -d devopsdockeruh/simple-web-service server
```