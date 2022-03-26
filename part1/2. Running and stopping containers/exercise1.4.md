# Part 1

## Exercise 1.4: Missing dependencies
---
- Command

``` shell
  docker run --rm -ti --name ubuntu-img ubuntu sh -c 'apt-get update; apt-get install curl; echo "Input website:"; read website; echo "Searching.."; sleep 1; curl http://$website;'
```