# Part 1

## Exercise 1.14: Environment
---
- Start both frontend-example and backend-example with correct ports exposed and add ENV to Dockerfile with necessary information from both READMEs (front,back).

``` 
    build & start frontend
```
``` powershell
    docker build . -t example-frontend

    docker run -ti 
    --name frontend-example 
    -p 5000:5000 
    example-frontend 
```

---

``` 
    build & start backend
```
``` powershell
    docker build . -t example-backend

    docker run -ti 
    --name example-backend 
    -e REQUEST_ORIGIN=http://localhost:5000 
    -p 8080:8080 backend-example
```