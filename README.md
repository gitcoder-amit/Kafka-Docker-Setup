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
- Creating Topic Command but we dont need to remember due to if we are working with Python we just need to find which particular function will does that here we are creating 2 topics using shell

```
./kafka-topics.sh --create --topic sample-topic --bootstrap-server broker:29092   -> 
./kafka-topics.sh --create --topic user-topic --bootstrap-server broker:29092

```

- To List down all the topics

```
./kafka-topics.sh --bootstrap-server broker:29092 --list
```
