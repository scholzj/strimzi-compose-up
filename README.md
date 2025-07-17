# Compose file for starting Apache Kafka cluster using the Strimzi container images

This repository contains a Docker Compose YAML file which allows you to start local Apache Kafka cluster.
It uses the Strimzi container images and is currently based on Strimzi 0.47.0 / Apache Kafka 4.0.0.
As Kafka 4.0.0 does not support ZooKeeper anymore, there is only a KRaft based compose file.
If you want to use ZooKeeper, check the [0.45.0 tag](https://github.com/scholzj/strimzi-compose-up/tree/0.45.0) which is based on Strimzi 0.45.0 and Apache Kafka 3.9.0 and still has ZooKeeper support as well.

## Usage

After installing Docker / Docker Compose on your machine, run `docker compose up` to start the Kafka broker. To shut it down, run `docker compose down`.