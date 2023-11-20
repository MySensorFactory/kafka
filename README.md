# Kafka

## Description

This project contains all manifests which are required to create Kafka cluster on Kubernetes cluster. Kafka cluster is defined as stateful set with 3 brokers with one zookeeper. 

Because of usage Apache Avro in the platform this project also contains schema registry application.

Every module and Kafka cluster is configured to use exactly once semantics. So publishing/consuming events is transactional.

This application creates necessary topics after cluster startup.
