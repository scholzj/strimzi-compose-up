# Compose file for starting Kafka and Zookeeper using the Strimzi images

This repository contains a Docker Compose YAML file which allows you to start local Zookeeper and Kafka using the broker images.
It uses the Strimzi container images and is currently based on Strimzi 0.38.0 / Apache Kafka 3.6.0.
You can also use the [`./kraft`](./kraft/) subdirectory to run Kafka with the _Kraft_ mode (without ZooKeeper).

After installing Docker / Docker Compose on your machine, run `docker-compose up` to start the Kafka broker. To shut it down, run `docker-compose down`.