# MongoDb-Docker
MongoDb Docker Setup

### Creating a MongoDb container with volume mount

`docker run -d -p <LOCAL_PORT>:27017 -v ~/<LOCAL_ABSOLUTE_PATH>:/data/db --name <IMAGE_NAME> mongo:latest`

```
docker run -d -p 27017:27017 -v ~/MongoDb/db:/data/db --name my-mongodb mongo:latest
```

### Accessing container with bash
`docker exec -it <CONTAINER_NAME> bash`

```
docker exec -it my-mongodb bash
```

### Accesing mongo shell from local machine
`mongo localhost:<MAPED_MONDO_DB_PORT>`

```
mongo localhost:27017
```

### Volume mount
Volume mount is used to preserve data irrespective of docker container. 