# Kafka-Docker-Setup

- Clone this repository

- Move inside the cloned directory and execute the following command(Make Sure Docker is running.)

```

docker compose up -d
```

- Now Once the container is Up, use the following command to enter the kafka shell running inside the kafka container

```
docker exec -it -w /opt/kafka/bin broker sh
```
