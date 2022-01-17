# postgreSQL Docker Compose

## Prerequisites

- Install Docker
- Install Docker Compose

## docker-compose file

[docker-compose.yaml](../postgreSQL/docker-compose.yaml)

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

## Connect to postgreSQL

Enter the running container using below command

```docker
docker exec -it postgreSQL bash
```

Connect to the postgreSQL server using below command

```shell
psql --username postgres
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