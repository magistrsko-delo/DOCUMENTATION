# DOCUMENTATION
All utility, kubernetes, etc.

## Docker utilities

* remove untaged images
``` 
docker rmi $(docker images -f “dangling=true” -q)
```

* docker compose  
``` 
docker-compose up -d  
docker-compose stop
docker-compose pull
```
* docker  
```docker run -d --hostname mag20-rabbit-host  --name mag20-rabbit -p 4369:4369 -p 5671:5671 -p 5672:5672 -p 15672:15672 rabbitmq:management```