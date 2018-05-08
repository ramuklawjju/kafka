# kafka
Learning kafka and everything about it

Kafka is - a publish-subscribe-based messaging system that is exchanging data between processes, applications, and servers. 

# Kafka Broker
A Kafka cluster consists of one or more servers (Kafka brokers), which are running Kafka. Producers are processes that publish data (push messages) into Kafka topics within the broker. A consumer of topics pulls messages off a Kafka topic.

# Kafka Topic
A Topic is a category/feed name to which messages are stored and published. Messages are byte arrays that can store any object in any format.

# Kafka topic partition
Kafka topics are divided into a number of partitions, which contains messages in an unchangeable sequence. Each message in a partition is assigned and identified by its unique offset. 

# Partitions allow you to parallelize a topic by splitting the data in a particular topic across multiple brokers

# Consumers and consumer groups
Consumers can read messages starting from a specific offset and are allowed to read from any offset point they choose. This allows consumers to join the cluster at any point in time.

# Apache Kafka Consumer
Consumers can join a group called a consumer group. A consumer group includes the set of consumer processes that are subscribing to a specific topic. Each consumer in the group is assigned a set of partitions to consume from. They will receive messages from a different subset of the partitions in the topic. Kafka guarantees that a message is only read by a single consumer in the group.

# Data/messages are never pushed out to consumers, the consumer will ask for messages when the consumer is ready to handle the message.

# Producer: Application that sends the messages.
# Consumer: Application that receives the messages.
# Message: Information that is sent from the producer to a consumer through Apache Kafka.
# Connection: A connection is a TCP connection between your application and the Kafka broker.
# Topic: A Topic is a category/feed name to which messages are stored and published.
# Topic partition: Kafka topics are divided into a number of partitions, which allows you to split data across multiple brokers.
# Replicas A replica of a partition is a "backup" of a partition. Replicas never read or write data. They are used to prevent data loss.
# Consumer Group: A consumer group includes the set of consumer processes that are subscribing to a specific topic.
# Offset: The offset is a unique identifier of a record within a partition. It denotes the position of the consumer in the partition.
# Node: A node is a single computer in the Apache Kafka cluster.
# Cluster: A cluster is a group of nodes i.e., a group of computers.
