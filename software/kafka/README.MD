##### kafka practice

Create a kafka service, which can be accessible from out off the kubernetes cluster.

- create Zookeeper Pod and Service
```commandline
> kubectl apply -f zookeeper.yaml
```

- create Kafka Pod and Service
> edit the `kafka.yaml` to set correct `KAFKA_ADVERTISED_HOST_NAME` before run below command.
```commandline
> kubectl apply -f kafka.yaml
```