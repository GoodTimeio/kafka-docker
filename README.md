Fork of [kafka-docker](https://github.com/wurstmeister/kafka-docker)

ATS Middleware Dev Kafka
==========================

Run by:
```sh
docker-compose up -d
```
This will orchestrate the kafka and a zookeeper containers as specified in `docker-compose.yml`.
The `-d` means detach/daemonize the container. Without this command, we wouldn't be able to
enter other commands into the terminal. The foreground would be occupied.

To check the status of containers:
```sh
docker ps
```

To stop the containers:
```sh
docker-compose down
```

If for some reason `docker-compose down` doesn't work, try:
```sh
// stop all the containers
docker stop $(docker ps -qa)

// remove all the containers
docker rm $(docker ps -qa)
```
