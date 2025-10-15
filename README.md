# Apache_Kafka_Exa
😍😍
Apache Kafka was developed at LinkedIn and was later open-sourced under Apache project. It is a distributed system that processes streams of data in real time, managing millions of events per second. Kafka can be used as a message bus for microservices and gives delivery guarantees: That means if some service goes down, messages are preserved in Kafka so next running instance of application can consume it later when needed.

Various components of Kafka

Brokers: These are servers that store & manage partitions, handling message read/write requests.
Producers: Producers send messages to Kafka topics, choosing a partition based on keys or round-robin distribution.
Consumers: Consumers read messages from Kafka topics, typically as part of a consumer group for parallel processing.
Zookeeper: manages Kafka metadata, leader election, and broker coordination (being replaced by KRaft).
KRaft: Kafka’s built-in metadata management system, replacing Zookeeper for scalability and reliability.
Topic: topic is a logical grouping of messages in Kafka, split into multiple partitions for parallelism.
Partition: Partition is sequence of records within a topic, stored on brokers and consumed independently.
Segment: A segment is a physical file within a partition where Kafka stores messages, rolling over based on size or time (max 1 gb for 1 ).
Offset: A unique identifier for each record within a partition, used to track consumer progress. So that consumer can resume.
😘😘
In kafka, we had many items about all concepts
😁😁
In Kafka, there are three types of clusters:
    Single node: Single broker
    Single node: Multiple Broker
    Multiple node: Multiple Broker
There are three ways to deliver messages:
    Never redelivered: The messages may be lost
    May be redelivered: The messages are never lost
    Delivered once: The message is delivered exactly once
There are two types of log compaction:
   Coarse grained: By time
   Finer grained: By message
