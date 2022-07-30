# Part 1

## Exercise 1.9: Volumes
---
- Image devopsdockeruh/simple-web-service creates a timestamp every two seconds to /usr/src/app/text.log when it's not given a command. Start the container with bind mount so that the logs are created into your filesystem.

``` powershell
    mkdir part1/volumes
    
    touch "$(pwd)/part1/volumes/text.log"

    docker run -ti 
    --name simple-web-service 
    -v "$(pwd)/part1/volumes/text.log:/usr/src/app/text.log" 
    -d devopsdockeruh/simple-web-service
```