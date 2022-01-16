# MongoDB Docker Compose

## Prerequisites

- Install Docker
- Install Docker Compose
- Install [mongosh](https://docs.mongodb.com/mongodb-shell/install/#install-mongosh)

## docker-compose file

[docker-compose.yaml](../mongodb/docker-compose.yaml)

## Run

```shell
docker-compose up
```

To run in detached mode use: 

```shell
docker-compose up -d
```

## Verify

Verify that the containers are running, use:

```shell
docker-compose ps
```

Verify the volume is created, use:

```shell
docker volume ls
```

## Connect to MongoDB

Use the below command to connect to the MongoDB server:

```shell
mongosh --username=root --password=root --host=localhost --port=27017
```

## Stop

To shut down database use:

```shell
docker-compose stop
```

To shut down database and containers use:

```shell
docker-compose down
```