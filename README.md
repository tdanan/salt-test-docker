# salt-test-docker
Salt in docker env to test salt functionalities:

### Prerequisites

docker and docker-compose installed

### Build

```
docker-compose -f salt-compose.yml up --build
```

### Check

```
docker exec -it master salt '*' test.ping
```
```
minion:
    True
```


